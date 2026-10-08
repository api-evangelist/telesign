---
generated: '2026-10-07'
method: generated
name: telesign-send-sms-message
description: Send a transactional, marketing or OTP SMS with the Messaging API and poll or receive its delivery status.
api: openapi/telesign-engage-api-openapi.yml
operations:
- sendSMS
- getSMSStatus
- reportSMSCompletion
source: Grounded in openapi/telesign-engage-api-openapi.yml; operationIds verified verbatim in openapi/.
---

# Send an SMS notification and track delivery

Send a transactional, marketing or OTP SMS with the Messaging API and poll or receive its delivery status.

## Steps
1. `sendSMS` — `POST /v1/messaging` on `https://rest-ww.telesign.com` (form-encoded) with `phone_number`, `message` and `message_type` (`OTP`, `ARN` alerts/reminders/notifications, or `MKT` marketing). Keep the `reference_id`.
2. `getSMSStatus` — `GET /v1/messaging/{reference_id}` to read `status.code` (200 Delivered to handset, 203 Delivered to gateway, 290 Message in progress ...), or receive the same report at your callback URL (`openapi/telesign-engage-callbacks-openapi.yml`).
3. `reportSMSCompletion` — `PUT /v1/verify/completion/{reference_id}` when the message carried an OTP the user completed.

## Rules
- `message_type` decides compliance handling; marketing traffic has its own sender and consent rules.
- No idempotency key: retrying `sendSMS` after a timeout can send twice (`conventions/telesign-conventions.yml`).
- Default SMS limit is 50 TPS Full-service and 1 TPS Self-service; 10019 is the rate-limit error code (`rate-limits/telesign-rate-limits.yml`).
- Callback retries: up to four attempts with 5/10/15 second waits; answer 200 quickly (`asyncapi/telesign-webhooks.yml`).
