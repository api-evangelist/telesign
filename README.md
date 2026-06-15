# Telesign (telesign)

Telesign provides a comprehensive suite of communications and security APIs enabling businesses to verify phone numbers, send SMS and voice messages, and assess fraud risk. Core offerings include SMS messaging, voice calls, multi-channel verification (OTP/MFA), phone number intelligence (PhoneID), reputation scoring, and silent verification. Telesign serves thousands of enterprises globally for account security, fraud prevention, and customer communications.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/apis.yml)

## Tags

- Authentication
- Communications
- Fraud Prevention
- Phone Intelligence
- SMS
- Verification

## Timestamps

- **Modified:** 2026-05-19

## APIs

### Telesign SMS API

Send SMS messages including alerts, notifications, reminders, marketing messages, and one-time passwords to phone numbers worldwide. Messages are classified by type (OTP, ARN, MKT) and provide delivery status tracking via reference IDs.

- **Human URL:** [https://developer.telesign.com/enterprise/docs/sms-get-started](https://developer.telesign.com/enterprise/docs/sms-get-started)
- **Base URL:** `https://rest-ww.telesign.com/v1`

#### Tags

- Alerts
- Messaging
- Notifications
- OTP
- SMS

#### Properties

- [Documentation](https://developer.telesign.com/enterprise/docs/sms-get-started)
- [OpenAPI](openapi/telesign-sms-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/telesign-sms.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/telesign-sms.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Telesign PhoneID API

Retrieve global phone number intelligence including carrier information, geographic location, phone type (mobile, landline, VoIP), and subscriber data. Used for fraud prevention, identity verification, and risk assessment during account creation and transactions.

- **Human URL:** [https://developer.telesign.com/enterprise/docs/phoneid-api-overview](https://developer.telesign.com/enterprise/docs/phoneid-api-overview)
- **Base URL:** `https://rest-ww.telesign.com/v1`

#### Tags

- Carrier Data
- Fraud Prevention
- Identity Verification
- Phone Intelligence
- Risk Assessment

#### Properties

- [Documentation](https://developer.telesign.com/enterprise/docs/phoneid-api-overview)
- [OpenAPI](openapi/telesign-phoneid-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/telesign-phoneid.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/telesign-phoneid.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Telesign Verify API

Multi-channel phone-based verification and MFA. Send one-time passcodes via SMS, voice, WhatsApp, Viber, RCS, or email, and verify codes submitted by end users. Supports password reset, account creation verification, and login MFA flows.

- **Human URL:** [https://developer.telesign.com/enterprise/docs/verify-api-overview](https://developer.telesign.com/enterprise/docs/verify-api-overview)
- **Base URL:** `https://rest-ww.telesign.com/v1`

#### Tags

- Authentication
- MFA
- OTP
- Two-Factor Authentication
- Verification

#### Properties

- [Documentation](https://developer.telesign.com/enterprise/docs/verify-api-overview)
- [OpenAPI](openapi/telesign-verify-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/telesign-verify.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/telesign-verify.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Telesign Score API

Assess fraud risk for phone numbers using reputation scoring based on intelligence, traffic patterns, machine learning, and a global data consortium. Returns a risk level and numeric score with a recommended action (allow, flag, block).

- **Human URL:** [https://developer.telesign.com/enterprise/docs/score-api-overview](https://developer.telesign.com/enterprise/docs/score-api-overview)
- **Base URL:** `https://rest-ww.telesign.com/v1`

#### Tags

- Fraud Detection
- Phone Intelligence
- Risk Scoring

#### Properties

- [Documentation](https://developer.telesign.com/enterprise/docs/score-api-overview)
- [OpenAPI](openapi/telesign-score-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/telesign-score.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/telesign-score.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Telesign Voice API

Send voice messages including OTPs, alerts, and notifications to phone numbers worldwide. Supports text-to-speech message delivery and call status tracking.

- **Human URL:** [https://developer.telesign.com/enterprise/docs/voice-get-started](https://developer.telesign.com/enterprise/docs/voice-get-started)
- **Base URL:** `https://rest-ww.telesign.com/v1`

#### Tags

- OTP
- Telecommunications
- Voice

#### Properties

- [Documentation](https://developer.telesign.com/enterprise/docs/voice-get-started)
- [Postman Collection](collections/telesign-phoneid.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/telesign-phoneid.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/telesign-score.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/telesign-score.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/telesign-sms.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/telesign-sms.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/telesign-verify.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/telesign-verify.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/telesign)
- [Website](https://www.telesign.com/)
- [Developer  Portal](https://developer.telesign.com/enterprise)
- [Authentication](https://developer.telesign.com/enterprise/docs/authentication)
- [Status Page](https://status.telesign.com/)
- [Pricing](https://www.telesign.com/pricing/)
- [Terms of Service](https://www.telesign.com/terms-conditions/)
- [GitHub Organization](https://github.com/TeleSign)
- [Integrations](https://www.telesign.com/partners)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
