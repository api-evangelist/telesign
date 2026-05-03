# Telesign

Telesign provides a comprehensive suite of communications and security APIs enabling businesses to verify phone numbers, send SMS and voice messages, and assess fraud risk. Core offerings include SMS messaging, voice calls, multi-channel verification (OTP/MFA), phone number intelligence (PhoneID), reputation scoring, and silent verification. Telesign serves thousands of enterprises globally for account security, fraud prevention, and customer communications.

**Website:** https://www.telesign.com/

**Developer Portal:** https://developer.telesign.com/enterprise

## APIs

| API | Description |
|-----|-------------|
| [SMS API](openapi/telesign-sms-openapi.yml) | Send SMS alerts, notifications, and OTPs worldwide |
| [PhoneID API](openapi/telesign-phoneid-openapi.yml) | Phone number intelligence for carrier, location, and type data |
| [Verify API](openapi/telesign-verify-openapi.yml) | Multi-channel OTP verification (SMS, voice, WhatsApp, etc.) |
| [Score API](openapi/telesign-score-openapi.yml) | Phone number fraud risk scoring |

## Links

- [Website](https://www.telesign.com/)
- [Developer Portal](https://developer.telesign.com/enterprise)
- [Authentication Guide](https://developer.telesign.com/enterprise/docs/authentication)
- [Status Page](https://status.telesign.com/)
- [Pricing](https://www.telesign.com/pricing/)
- [Terms of Service](https://www.telesign.com/terms-conditions/)

## Capabilities

| Capability | Description |
|------------|-------------|
| [identity-verification.yaml](capabilities/identity-verification.yaml) | Unified phone verification + fraud prevention workflow |

### Shared Definitions

| File | API |
|------|-----|
| [capabilities/shared/sms.yaml](capabilities/shared/sms.yaml) | SMS API |
| [capabilities/shared/phoneid.yaml](capabilities/shared/phoneid.yaml) | PhoneID API |
| [capabilities/shared/verify.yaml](capabilities/shared/verify.yaml) | Verify API |
| [capabilities/shared/score.yaml](capabilities/shared/score.yaml) | Score API |

## Artifacts

| Artifact | Description |
|----------|-------------|
| [apis.yml](apis.yml) | API catalog index |
| [rules/telesign-rules.yml](rules/telesign-rules.yml) | Spectral ruleset |
| [json-schema/telesign-messaging-response-schema.json](json-schema/telesign-messaging-response-schema.json) | SMS response schema |
| [json-schema/telesign-phoneid-response-schema.json](json-schema/telesign-phoneid-response-schema.json) | PhoneID response schema |
| [json-structure/telesign-messaging-structure.json](json-structure/telesign-messaging-structure.json) | Messaging API structure |
| [json-ld/telesign-context.jsonld](json-ld/telesign-context.jsonld) | JSON-LD context |
| [examples/telesign-send-sms-example.json](examples/telesign-send-sms-example.json) | Send SMS example |
| [examples/telesign-phoneid-lookup-example.json](examples/telesign-phoneid-lookup-example.json) | PhoneID lookup example |
| [examples/telesign-create-verification-example.json](examples/telesign-create-verification-example.json) | Create verification example |
| [vocabulary/telesign-vocabulary.yml](vocabulary/telesign-vocabulary.yml) | Domain vocabulary |
