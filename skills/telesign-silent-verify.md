---
generated: '2026-10-07'
method: generated
name: telesign-silent-verify
description: 'Run a Silent Verify: initiate a verification for a device on a mobile data connection, have the device open the returned URL, then finalize to learn whether the SIM matches the phone number.'
api: openapi/telesign-silent-verify-api-openapi.yml
operations:
- createSilentVerifyRequest
- getSilentVerifyStatus
source: Grounded in openapi/telesign-silent-verify-api-openapi.yml; operationIds verified verbatim in openapi/.
---

# Verify a phone silently over the mobile network

Run a Silent Verify: initiate a verification for a device on a mobile data connection, have the device open the returned URL, then finalize to learn whether the SIM matches the phone number.

## Steps
1. `createSilentVerifyRequest` — `POST /silent/initiate` on `https://verify.telesign.com` with the end user's `phone_number`. The response carries a `reference_id` and a verification URL.
2. On the device, open the verification URL over the mobile data connection (not Wi-Fi) so the carrier can attest the SIM.
3. `getSilentVerifyStatus` — `POST /silent/finalize` with the `reference_id` to read the verification result.

## Rules
- Only Basic authentication is declared for this contract (`authentication/telesign-authentication.yml`).
- Default rate limit is 10 TPS per account for Full-service (`rate-limits/telesign-rate-limits.yml`); error code 10019 means the limit was exceeded.
- There is no cancel operation; an unfinished verification simply expires (`conventions/telesign-conventions.yml`).
