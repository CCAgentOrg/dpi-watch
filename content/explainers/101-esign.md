---
title: "eSign 101: India's Online Electronic Signature Service"
description: "How India's CCA-regulated eSign service authenticates signers and applies verifiable electronic signatures; its legal limits, privacy trade-offs, inclusion barriers, and grievance routes."
date: 2026-10-15
draft: false
tags: ["esign", "electronic-signature", "digital-signature", "cca", "it-act", "aadhaar", "dpi", "digital-inclusion", "india"]
categories: ["DPI Basics"]
author: "CashlessConsumer"
readingTime: "12 min"
---

# eSign 101: India's Online Electronic Signature Service

## What is eSign?

**eSign** is India's online electronic-signature service: an application can connect a signer to an e-KYC-based workflow that obtains a Digital Signature Certificate (DSC) and applies a cryptographic signature to electronic data. The Controller of Certifying Authorities (CCA) describes the service as being delivered through licensed Certifying Authorities (CAs) and integrated into government, business, or other applications through an API. [^1]

That makes eSign different from typing a name, pasting an image of a handwritten signature, or entering an OTP by itself. In the eSign flow, authentication helps establish who is asking to sign; a certificate and cryptographic signature bind that signing event to particular document data. The Information Technology Act, 2000 (IT Act) recognises electronic signatures made in the prescribed manner, but an eSign badge does not by itself make every document or transaction legally valid. The document, the signer's authority and intent, and any other legal formalities still matter. [^2]

### Historical context

The CCA's API catalogue records the first eSign API specification on **15 July 2015**. The Electronic Signature or Electronic Authentication Technique and Procedure Rules, 2015 added an e-authentication technique using Aadhaar e-KYC; a 2019 Gazette amendment added other e-KYC services. In September 2026, the CCA listed version 1.1 of a separate eSign Remote API for remote key storage. These are regulatory and technical milestones, not measures of how many people have signed documents. [^3][^4][^5]

## How it works

A typical one-time eSign transaction has these actors: the **Application Service Provider (ASP)** hosts the service journey and document; the **eSign Service Provider (ESP)** coordinates the signing service; the **CA** issues the signing certificate; and an e-KYC provider authenticates the signer. The CCA says eSign services are currently facilitated by CAs licensed under the IT Act. [^1][^4]

1. The ASP presents a document and starts a signing request. The signer should be able to inspect the exact version before authorising it.
2. The user gives electronic consent for the eSign process and completes the authentication supported by that route. CCA specifications distinguish “Online Aadhaar & Others” from “CA eKYC Account based” APIs; therefore, describing every eSign transaction as Aadhaar-only is too broad. The available method depends on the application and provider. [^3][^4][^5]
3. In the documented one-time-key model, the signing service creates a key pair inside a Hardware Security Module (HSM). The CA issues a short-validity certificate for the signing key, and the private key signs the document's hash (a digital fingerprint). The CCA's eSign page says the document content is not sent in the clear to the eSign signature function, and that the one-time private key is destroyed after use. The authentication and signature steps produce an audit trail. [^1][^5]
4. The signed document is returned through the application. A recipient can validate the cryptographic signature and certificate using suitable PDF or certificate-verification software; changing signed content should cause validation to fail. [^1][^8]

**A separate key-storage mode matters.** The CCA also lists a Remote API for remote key storage, most recently version 1.1 dated 9 September 2026. That is not the same key-lifecycle model as a one-time key destroyed after one signature. If an application offers remote key storage, ask who controls activation, what authentication protects the stored key, and how suspension or revocation works. [^4][^5]

## Key statistics and verified milestones

| Measure | Verified information | What it does—and does not—show |
|---|---|---|
| First eSign API specification | Version 1.0, released 15 July 2015. [^4] | Dates the initial published API specification; it is not a transaction count. |
| Current API families listed by CCA | “Online Aadhaar & Others” API 2.1, released 7 February 2023; “CA eKYC Account based” API 3.3, released 9 December 2020. [^4] | These are distinct API families, so version numbers should not be read as one simple chronological sequence. |
| Remote key-storage API | Version 1.1, released 9 September 2026. [^4] | Confirms a separately documented remote-key option; it does not establish how widely it is deployed. |
| National transaction volume | The current CCA eSign and API pages reviewed for this explainer do not publish a dated, current all-India signing total. [^1][^4] | No current adoption total is asserted here. A missing public counter is a reporting gap, not evidence that the service is unused. |

**Conflicting descriptions resolved:** Older launch material often describes eSign as Aadhaar-only and one-use-key based. The CCA's current API catalogue includes “Others” and CA-account-based e-KYC routes, while its separate Remote API is for remote key storage. The one-time-key privacy claim applies to that one-time model; it should not be generalized to every authentication or key-storage option. [^3][^4][^5]

## Layers classification (L1–L7)

This is DPI Watch's analytical mapping, not an official CCA or government classification.

| Layer | eSign's role |
|---|---|
| **L1 — Policy and purpose** | Government and private services choose where electronic signing can replace paper workflows; the IT Act supplies the legal-recognition framework. [^2] |
| **L2 — Regulation and accountability** | MeitY's CCA licenses and supervises CAs; eSign rules, CCA guidelines, and—where Aadhaar is used—UIDAI law and regulations govern parts of the trust chain. [^1][^3][^6] |
| **L3 — Digital trust rail** | The eSign service coordinates authentication, certificate issuance, and signing between the application, ESP, CA, and e-KYC provider. [^1][^5] |
| **L4 — APIs and cryptographic protocol** | CCA APIs define service integration; public-key certificates, document hashes, HSM controls, and audit records support signing and verification. [^1][^4][^5] |
| **L5 — Applications and access points** | The ASP's website or app presents the document and consent flow. Its design determines what a person sees, can understand, and can correct before signing. [^1][^4] |
| **L6 — Services and use cases** | Government forms, financial onboarding, business workflows, and other services can embed signing; acceptance and any required formalities remain specific to the relevant document and service. [^1][^2] |
| **L7 — Reporting and audit** | A signed file, certificate, transaction identifiers, and time-stamped audit records can support verification and dispute review. The CCA pages reviewed do not provide a public, current national signing-volume series. [^1][^5] |

## Regulatory framework

- **Information Technology Act, 2000:** Sections 3A and 5 provide for electronic signatures and their legal recognition when the prescribed requirements are met; section 10A recognises contracts formed through electronic means. The Act's First Schedule excludes specified document classes—including wills, trusts, powers of attorney, and contracts for sale or conveyance of immovable property—from its electronic-record provisions. Section 9 also does not create a general right to insist that a government office accept an electronic record. Check the law governing the particular document before relying on eSign. [^2]
- **Electronic Signature or Electronic Authentication Technique and Procedure Rules:** The 2015 Rules introduced an e-KYC-based electronic-authentication method. CCA's Gazette index records the 2019 amendment (S.O. 1119(E)) extending the framework to other e-KYC services. CCA's technical specifications and e-authentication guidelines describe how licensed CAs and providers must implement the service. [^3][^5]
- **CCA and Certifying Authorities:** The CCA is the licensing and supervisory authority for CAs under the IT Act. CAs issue Digital Signature Certificates and provide the regulated service; the CCA publishes current CA and eSign-provider information. An application that merely displays a “sign” button is not, by that fact alone, a licensed CA. [^1][^10]
- **Aadhaar rules, when that route is used:** UIDAI's Aadhaar (Sharing of Information) Regulations, updated on 21 August 2025, require consent for Aadhaar e-KYC sharing; restrict use and onward disclosure of identity information; bar requesting entities from storing core biometrics except as specifically permitted; and require an entity collecting an Aadhaar number to state the purpose, whether Aadhaar is mandatory or voluntary, available alternatives, and obtain consent. These duties apply to the Aadhaar route, not automatically to every non-Aadhaar e-KYC method. [^6]
- **Digital Personal Data Protection Act, 2023 (DPDP Act) and Rules, 2025:** The commencement notification is phased. As of **15 October 2026**, the core processing duties and data-principal rights in the 18-month tranche are scheduled to commence on **13 May 2027**, not yet on this explainer's date. Do not describe the whole DPDP rights regime as already operative; check the commencement notification for each provision. Other privacy, confidentiality, Aadhaar, and IT Act obligations may apply in the meantime. [^7][^8]

## Citizen rights analysis

### What the design can improve

- **Lower equipment and paperwork burden:** A remote signing flow can avoid an individual's need to buy and maintain a personal cryptographic USB token or make a separate in-person certificate application. This can make a digital service faster to complete, provided the user's authentication route works. [^1]
- **Document integrity and evidence:** A cryptographic signature can help a recipient detect later changes to the signed data and can provide a certificate and audit record for checking what key signed it. That is useful evidence, but it is not proof that the person understood the document or agreed freely to every term. [^1][^5]
- **More than one identity route is documented:** The CCA's API catalogue lists Aadhaar-and-other and CA-account-based families. This creates scope for alternatives, but a person must check what a particular application actually supports; a catalogue entry does not guarantee an alternative in every service. [^4]

### What deserves scrutiny

- **Consent can be formal rather than meaningful.** A consent click or OTP can record an action without proving the person saw the final document, understood its effect, or had a realistic chance to decline. This is a design and accountability concern, not a measured national failure rate. [^1][^5]
- **A signed hash does not make the whole journey private.** The CCA says its eSign signature function receives a document hash rather than the document in the clear. But the ASP must present or process the document, and the receiving organisation may retain it. The hash-only statement should not be read as end-to-end confidentiality across all participants. [^1]
- **Identity metadata still matters.** The CCA describes recording the e-KYC identifier and maintaining a transaction audit trail. Those records can link identity to the time and context of a signing event; users should be told which participants keep them, for how long, and how to obtain them. [^1][^5]
- **Inclusion is conditional.** Online signing reduces reliance on physical tokens, but a particular route may still require a suitable device, connectivity, accessible document display, a working authentication channel, and an e-KYC record. Failed or inaccessible authentication can turn a nominally paperless route into a barrier. An organisation should explain an accessible alternative, especially for urgent or high-stakes services. [^1][^4]
- **Remote key storage changes the risk question.** A key retained for repeated use is operationally different from a private key created for one signature and immediately destroyed. Users should not assume the one-time deletion safeguard applies to a service using remote storage. [^4][^5]

## Privacy implications

The system separates identity authentication from the signed document's cryptographic payload, which can reduce how much document content reaches the signature service. That is a data-minimisation feature, not a guarantee that every participant sees only a hash. The ASP, the organisation receiving the signed document, the e-KYC provider, ESP, and CA may each process different data under their own role and retention rules. Ask for the exact data-flow and privacy notice for the service you are using. [^1][^5]

For Aadhaar-based e-KYC, UIDAI rules prohibit the requesting entity from storing or sharing core biometrics outside the prescribed exception and limit identity information to the stated purpose. The Aadhaar number itself must not be publicly exposed and should not be retained longer than necessary for the disclosed purpose. These are important constraints, but they do not answer every question about the signed document, provider logs, or other non-Aadhaar e-KYC routes. [^6]

The DPDP Act's future full commencement should not be used as a reason to collect more data now. Until the scheduled provisions commence, users should rely on protections already in force and demand clear notices, minimum data collection, secure handling, and practical complaint routes. [^7][^8]

## Safeguards for users and service operators

- Before entering an OTP or approving authentication, open and read the complete final document; check the recipient, date, amount, obligations, attachments, and every page. Do not sign a blank, partial, or materially different version.
- Confirm that the application names the eSign provider and explains what e-KYC method is being used. Do not disclose an OTP or authentication code to a caller, agent, or chat contact; enter it only in the expected official signing flow. [^1][^4]
- Download and retain the completed signed file, signing confirmation, transaction/reference number, and any consent or authentication receipt. Ask the ASP or CA for the certificate, audit details, and correction or dispute process if something looks wrong. [^1][^5]
- Verify the signature in a suitable PDF reader or certificate tool. A visible signature image alone is not verification; check the certificate issuer, signing identity, validation result, and whether the file reports changes after signing. [^1][^8]
- For an Aadhaar-based flow, use the UIDAI authentication-history and grievance channels if you suspect an authentication you did not initiate. Request that the service provider identify the e-KYC purpose and the data it retains. [^6][^12]
- Service operators should show the final file before consent, clearly identify each participant, minimise personal data, provide accessible authentication and non-digital assistance where needed, and document retention and incident escalation. These are rights-preserving design recommendations grounded in the service's documented multi-party flow. [^1][^5]

## Complaints and grievance redressal

1. **Start with the application that asked you to sign.** Report a wrong, unauthorised, or incomplete signing event to the ASP and ask for the transaction ID, the exact signed file, certificate, audit trail, e-KYC method, and complaint reference.
2. **Escalate a signing-service or certificate issue to the provider/CA.** Use the current CCA directory to identify the responsible licensed CA or eSign provider. The CCA's public guidance says CAs must maintain a complaint-redressal mechanism; the CCA's role does not replace a contract dispute between an ASP and ESP. [^9][^10]
3. **Raise a regulatory complaint with the CCA** for concerns about a CA's licensing or compliance, using the CCA's Public Grievances channel and keeping the complaint number and evidence. [^11]
4. **For Aadhaar authentication or identity-information issues, contact UIDAI** through its grievance portal, helpline **1947**, or `help@uidai.gov.in`; retain the authentication time and service name. [^12]
5. **If a government service refuses an e-signed document,** request the applicable rule and a written reason, since the IT Act does not give users a blanket right to force every government body to accept electronic records. For high-stakes disputes, get advice specific to the document and applicable law. [^2]

## Prime References

[^1]: Controller of Certifying Authorities (CCA), [eSign — Online Electronic Signature Service](https://cca.gov.in/eSign.html).
[^2]: India Code, [Information Technology Act, 2000](https://www.indiacode.nic.in/handle/123456789/18594?view_type=browse).
[^3]: CCA, [eSign Gazette Notifications](https://cca.gov.in/eSign_gazette_notification.html).
[^4]: CCA, [eSign API Specifications](https://cca.gov.in/eSignAPI.html).
[^5]: CCA, [e-authentication guidelines for eSign](https://cca.gov.in/sites/files/pdf/esign/CCA-EAUTH.pdf).
[^6]: UIDAI, [Aadhaar (Sharing of Information) Regulations, 2016, updated 21 August 2025](https://uidai.gov.in/images/The_Aadhaar_Sharing_of_information_regulation_2016.pdf).
[^7]: India Code, [Digital Personal Data Protection Act, 2023](https://www.indiacode.nic.in/handle/123456789/22037?view_type=browse).
[^8]: MeitY, [G.S.R. 843(E), 13 November 2025 — DPDP Act commencement notification](https://www.meity.gov.in/static/uploads/2025/11/c56ceae6c383460ca69577428d36828b.pdf).
[^9]: CCA, [eSign FAQ](https://cca.gov.in/sites/files/pdf/esign/ESIGNFAQ.pdf).
[^10]: CCA, [Digital Signature and Certifying Authority contact information](https://cca.gov.in/digital_signature.html).
[^11]: CCA, [Public Grievances](https://cca.gov.in/Public_Grievances.html).
[^12]: UIDAI, [Grievance Redressal](https://uidai.gov.in/en/contact-support/grievance-redressal.html).

---

*Fact-check date: 15 October 2026. Public CCA materials describe distinct identity and key-management models; this explainer keeps those paths separate and does not infer adoption from API-version dates. It is general information, not legal advice.*
