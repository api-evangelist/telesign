---
generated: '2026-10-07'
method: generated
name: telesign-send-sms-otp
description: Send a one-time passcode by SMS with the SMS Verify API, check its delivery status, and report whether the end user entered the right code.
api: openapi/telesign-sms-verify-api-openapi.yml
operations:
- sendSMSVerifyCode
- getSMSVerifyStatus
- reportSMSVerifyCompletion
source: Grounded in openapi/telesign-sms-verify-api-openapi.yml; operationIds verified verbatim in openapi/.
---

# Send and complete an SMS one-time passcode

Send a one-time passcode by SMS with the SMS Verify API, check its delivery status, and report whether the end user entered the right code.

## Steps
1. `sendSMSVerifyCode` — `POST /v1/verify/sms` (form-encoded) with `phone_number` in E.164 digits. Let Telesign generate the code, or pass your own `verify_code`. Keep the `reference_id` from the response.
2. Ask the user for the code they received.
3. `getSMSVerifyStatus` — `GET /v1/verify/{reference_id}` with `verify_code` to have Telesign compare the code and read `verify.code_state` (VALID / INVALID / UNKNOWN / EXPIRED) and `status.code` (200 Delivered, 290 Message in progress, 207 Error delivering ...).
4. `reportSMSVerifyCompletion` — `PUT /v1/verify/completion/{reference_id}` once the user is verified, so the transaction is counted as a completion.

## Rules
- Authenticate with Basic (Customer ID / API Key) or Telesign Digest; see `authentication/telesign-authentication.yml`.
- There is no idempotency key: a retried `sendSMSVerifyCode` sends a second SMS (`conventions/telesign-conventions.yml`). Retry only on a transport failure with no response.
- Read `status.code` and `errors[].code`, never the HTTP status alone; -40007 is a rate limit (default 50 TPS for Full-service, 1 TPS for Self-service, `rate-limits/telesign-rate-limits.yml`).
- Delivery reports can also arrive at your callback URL (`openapi/telesign-sms-verify-api-callbacks-openapi.yml`), signed with HMAC-SHA256 in `Authorization` / `X-TS-Authorization`.
