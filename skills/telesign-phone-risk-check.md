---
generated: '2026-10-07'
method: generated
name: telesign-phone-risk-check
description: Look up a phone number with Phone ID for carrier, type and identity signals, then score it with the Intelligence Cloud API before letting an account through onboarding.
api: openapi/telesign-detect-api-openapi.yml
operations:
- submitPhoneNumberForIdentity
- submitPhoneNumberForIntelligenceCloud
source: Grounded in openapi/telesign-detect-api-openapi.yml; operationIds verified verbatim in openapi/.
---

# Check a phone number before onboarding

Look up a phone number with Phone ID for carrier, type and identity signals, then score it with the Intelligence Cloud API before letting an account through onboarding.

## Steps
1. `submitPhoneNumberForIdentity` — `POST /phoneid/{complete_phone_number}` on `https://rest-ww.telesign.com/v1` with the add-ons you are entitled to (for example `contact`, `phone_type`, `number_deactivation`). Read `phone_type.description` (VOIP, MOBILE, LANDLINE ...) and the carrier.
2. `submitPhoneNumberForIntelligenceCloud` — `POST /intelligence/phone` on `https://detect.telesign.com` (`openapi/telesign-intelligence-cloud-api-openapi.yml`) with the phone number and `account_lifecycle_event` (create, sign-in, transact, update, delete) to get a risk score and recommendation.
3. Decide: allow, step up to an OTP (`telesign-send-sms-otp`), or block.

## Rules
- Do not call `submitPhoneNumberForIntelligence` (`POST /score/{complete_phone_number}`): it is the deprecated on-prem Intelligence endpoint (`lifecycle/telesign-lifecycle.yml`).
- Phone ID and Intelligence default to 150 TPS per account (`rate-limits/telesign-rate-limits.yml`).
- Both are reads; nothing to reverse. Each call is billed per transaction (`plans/telesign-plans-pricing.yml`).
