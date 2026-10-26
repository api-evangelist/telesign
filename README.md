# Telesign (telesign)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
