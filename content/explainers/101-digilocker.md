---
title: "DigiLocker 101: India's Digital Document Wallet and Verification Rails"
description: "A comprehensive guide to DigiLocker — MeitY's digital document platform, its legal equivalence under the IT (Digital Locker Facilities) Rules 2016, issuer–requester architecture, adoption statistics, citizen rights, privacy safeguards, and grievance routes."
date: 2026-10-01
draft: false
tags: ["digilocker", "digital-documents", "meity", "negd", "digital-india", "aadhaar", "rule-9a", "meripehchaan", "entity-locker", "dpi", "data-protection", "india"]
categories: ["DPI Basics"]
image: "/images/digilocker-101-cover.jpg"
author: "CashlessConsumer"
readingTime: "15 min"
---

# DigiLocker 101: India's Digital Document Wallet and Verification Rails

## What is DigiLocker?

**DigiLocker** is a secure, cloud-based platform for the issuance, storage, sharing and verification of digital documents and certificates, operated by the **National e-Governance Division (NeGD)** under the **Ministry of Electronics and Information Technology (MeitY)** as a flagship initiative of the Digital India programme. Its stated aim is the "Digital Empowerment" of citizens by providing access to authentic digital documents in a personal digital document wallet. [^1] Every issued document in the system is digitally signed by its issuing authority, and — critically for citizens — such issued documents are "deemed to be at par with original physical documents" under **Rule 9A** of the Information Technology (Preservation and Retention of Information by Intermediaries Providing Digital Locker Facilities) Rules, 2016. [^1][^3]

DigiLocker is more than a personal file store. Its value comes from a statutory equivalence (digital documents that government offices, police, banks and airlines must accept), an issuer–requester architecture that pulls documents directly from the original issuing authority's repository, and an OAuth 2.0-based consent framework through which citizens share documents with verifiers. [^2][^3][^12] The platform also powers **MeriPehchaan**, the National Single Sign-On service, and its business-side sibling **Entity Locker** (launched January 2025) extends the same rails to companies, MSMEs, trusts and societies. [^15][^26]

### Historical Context

| Date | Milestone |
|---|---|
| 10 Feb 2015 | Beta version of Digital Locker released [^28] |
| 1 Jul 2015 | National launch by the Prime Minister under the Digital India programme [^8][^28] |
| 2015–16 | Original application (developed under a Union–Maharashtra MoU) transferred to NeGD, which re-imagined it from a file store into a document-exchange infrastructure [^9] |
| 21 Jul 2016 | IT (Preservation and Retention of Information by Intermediaries Providing Digital Locker Facilities) Rules, 2016 notified (G.S.R. 711(E)) [^2] |
| 8 Feb 2017 | Rule 9A inserted by G.S.R. 111(E) (retrospective from 21 Jul 2016), establishing legal equivalence of issued documents [^3] |
| Aug–Dec 2018 | MoRTH advisories + G.S.R. 1081(E) amend Rule 139 of the Central Motor Vehicles Rules: driving licences, registration certificates and related documents in DigiLocker/mParivahan accepted at par with originals [^13][^14] |
| 20 Jan 2025 | MeitY launches **Entity Locker** for business and organisational documents [^15] |
| 2 Jun 2025 | Revised, DPDP-aligned Terms of Use published (privacy-focused, user ownership, children's data clause) [^11] |
| 2025–26 | DigiLocker-based verification extended to high-risk bank transactions (from 1 Apr 2026) and CKYC 2.0 onboarding [^19][^27] |
| 12 Aug 2026 | Parliament informed: 72.43 crore registered users; 5,437 document types/services [^4] |

## How It Works

### The Three Participants

| Role | What it does | Examples |
|------|--------------|----------|
| **Issuer** | Registered government department, agency or body that pushes digitally signed e-documents directly into a subscriber's locker, each carrying a unique Uniform Resource Identifier (URI). | CBSE and state education boards, UIDAI, state transport departments (via VAHAN), EPFO, income tax/PAN authorities, universities, police (FIR copies) [^1][^26] |
| **Requester** | Entity that verifies a citizen's documents, with the citizen's consent, through DigiLocker's APIs instead of demanding photocopies. | Banks and NBFCs (KYC), railways and airlines (ID checks), employers, universities, telecom operators, insurance companies [^1][^26][^27] |
| **Platform (NeGD/DigiLocker)** | Operates the repository, access gateway and consent machinery; signs up issuers and requesters; maintains the national statistics. Does not read, process or analyse stored content under its Terms of Use. | digilocker.gov.in, mobile apps, MeriPehchaan SSO, Entity Locker [^1][^11] |

### Registration and Authentication

A user registers with a valid Indian mobile number, Driving Licence, PAN or Aadhaar number and verifies via OTP; the Terms of Use state that Aadhaar is used **voluntarily** by users for authentication. [^11] In practice, fetching *issued* documents — the whole point of the platform — requires Aadhaar-based linking, since issuers key their repositories to the Aadhaar number. Multi-factor authentication uses mobile OTP or biometrics, and DigiLocker also issues an **Aadhaar Verifiable Credential** so citizens can share only the specific fields a verifier needs. [^1][^12]

### Issued vs Uploaded Documents — The Distinction That Matters

- **Issued documents** are pulled from the registered issuer's own repository into the user's account as machine-readable, digitally signed records with a URI. Only these carry the Rule 9A statutory equivalence: when a requester accesses them via the URI, they are "deemed to have been shared by the issuer directly in electronic form." [^3]
- **Uploaded documents** are scans the user stores in the free 1 GB personal space (10 MB per file) and can self-attest using the **eSign** facility. These are convenience copies — they do **not** automatically acquire the "at par with original" status. [^1][^2][^10]

### The Consent-Based Sharing Flow

1. **Issue** — the issuer creates a digitally signed e-document (Digital Signature Certificate) and pushes it to the subscriber's DigiLocker account with a unique URI. [^12]
2. **Request** — a requester (say, a bank doing KYC) triggers a DigiLocker verification during a citizen's onboarding flow.
3. **Consent** — the citizen explicitly approves sharing specific documents; the request is authenticated over **OAuth 2.0**, with consent enforced via PKI-based signatures. Every consent event is logged. [^11][^12]
4. **Fetch** — the requester retrieves the document through the API; because the URI points to the issuer's repository — the "single source of truth" — verification against the live original happens automatically. [^3]
5. **Revoke** — via the **"My Consent" dashboard**, citizens can see which apps have access, set time limits, and cancel access with one click; revocation instantly invalidates stored tokens. [^8]

### MeriPehchaan and Entity Locker

**MeriPehchaan** (National Single Sign-On) uses DigiLocker's identity rails to let citizens log into participating government services with one set of credentials; its requester API specification was updated to v2.4 in September 2026, signalling active development. [^26] **Entity Locker**, launched 20 January 2025, gives companies, MSMEs, trusts and societies a document wallet registered against GSTN/PAN/CIN-DIN/MSME identifiers, with issuers including PAN, GST, Udyam and FSSAI authorities. [^15]

## Key Statistics

*(Figures as of the latest verifiable official reporting — July–October 2026.)*

| Metric | Value | As of |
|---|---|---|
| Registered users | **72.43 crore (724+ million)** [^4] | 31 Jul 2026 |
| Document types/services on platform | **5,437** (661 Central Government; 4,776 State Government) [^4] | 31 Jul 2026 |
| Document-access transactions | ~72.86 crore over the preceding three years [^4] | Jul 2023–Jul 2026 |
| Cumulative issued documents | **900+ crore** (platform counter); 850+ crore reported by PIB in June 2026 [^5][^6] | 2026 |
| Issuer organisations | ~2,900 issuers; 1,000+ organisations integrated [^7] | 2026 |
| Issuers per major state (example) | Rajasthan: 125+ issuers [^5] | 2026 |
| Free storage | 1 GB (10 MB per uploaded file) [^10] | current |
| UMANG (sibling platform) | 11.66 crore users; ~2,575 services; ~798 crore transactions in 3 years [^4] | 31 Jul 2026 |
| CSC access network | 4,07,122 Common Service Centres at Gram Panchayat level [^4] | 30 Jun 2026 |
| International | DigiLocker-specific MoUs with Cuba, Kenya, UAE and Laos within 23–24 country India Stack agreements; SOP published for countries co-developing national digital document wallets [^16][^17][^18] | Feb–Jun 2026 |

**⚠️ Conflicting figures — read with care:** the "issued documents" count varies by snapshot and source — PIB reported **850+ crore** in June 2026, [^6] the Digital India Corporation page showed **8.1 billion** (~810 crore), [^7] and the platform's live homepage counter reads **900+ crore**. [^5] These are reconcilable as different dates/counting rules but should never be quoted as one number. Similarly, "users" means *registered* accounts (72.43 crore); no official figure discloses *active* users — a registered-but-dormant account still counts in the headline.

## Layers Classification (L1-L7)

| Layer | Classification | DigiLocker's Role |
|---|---|---|
| **L1 — Vision & Policy** | Government policy | Digital India programme (July 2015); paperless governance and "Digital Empowerment" vision; DPI export diplomacy [^8][^17] |
| **L2 — Regulation** | Regulatory framework | IT Act 2000 (ss. 6A, 10A, 87(2)); IT (Digital Locker Facilities) Rules 2016 + Rule 9A amendment 2017; sectoral rules (e.g., CMVR Rule 139 amendment G.S.R. 1081(E)); DPDP Act 2023 as the emerging data-protection overlay [^2][^3][^13] |
| **L3 — Digital Rails** | Core infrastructure | The DigiLocker platform itself: national document repository, issuance and verification rails, Aadhaar-linked authentication, MeriPehchaan SSO [^1][^26] |
| **L4 — APIs & Protocols** | Open standards | Issuer API spec v1.13 (May 2024), Requester API spec v1.12, MeriPehchaan API spec v2.4 (Sep 2026); OAuth 2.0; URI + XML certificate standards; eSign; API Setu partner gateway [^12][^26] |
| **L5 — Applications** | End-user apps | DigiLocker web + Android/iOS apps, WhatsApp chatbot, mParivahan document display, Entity Locker web app, DigiLocker Drive premium storage [^11][^15] |
| **L6 — Use Cases** | Sectoral applications | Traffic-check production of DL/RC, bank/fintech KYC (RBI accepts DigiLocker documents as OVDs), education records (CBSE mark sheets, APAAR/Academic Bank of Credits), EPFO services, railway/airport ID, insurance underwriting, high-risk bank-transaction verification from Apr 2026 [^13][^19][^20][^27] |
| **L7 — Analytics & Intelligence** | Data & insights | National statistics Power BI dashboard, verification/consent audit logs, issuer-side document analytics [^1][^4] |

DigiLocker is best read as an **L3-L4 construct** like UPI: a public-good core (repository + issuance + consent rails) with user experience delivered by the platform's own apps and by thousands of requester integrations.

## Regulatory Framework

**Primary legal basis.** The IT (Preservation and Retention of Information by Intermediaries Providing Digital Locker Facilities) Rules, 2016, notified on 21 July 2016 (G.S.R. 711(E)) under the IT Act, 2000, provide for a Digital Locker Authority and licensed locker service providers. [^2] **Rule 9A**, inserted by Notification G.S.R. 111(E) dated 8 February 2017 (retrospectively effective from 21 July 2016), is the load-bearing provision: issuers may issue and requesters must accept digitally signed documents shared from a subscriber's DigiLocker account *at par with physical documents*, and access via the URI is deemed direct sharing by the issuer. [^3] MeitY has confirmed in Parliament that documents available via DigiLocker "are to be treated at par with original physical documents" under Rule 9A. [^3]

**Sectoral adoption law.** The Ministry of Road Transport and Highways amended **Rule 139 of the Central Motor Vehicles Rules** via G.S.R. 1081(E) dated 2 November 2018, enabling production of registration certificates, insurance, fitness, permits, driving licences and PUC certificates in electronic form, with a standard operating procedure (17 December 2018) directing enforcement agencies to validate documents presented through DigiLocker or mParivahan. [^13][^14]

**Data protection law.** The **Digital Personal Data Protection Act, 2023** and the DPDP Rules notified in November 2025 set the emerging overlay: consent must be free, specific, informed and unambiguous; children's data requires verifiable parental consent; and a registered **Consent Manager** regime activates by **13 November 2026**. DigiLocker's June 2025 Terms of Use are visibly DPDP-aligned (user ownership, logged consent, children's clause), but whether DigiLocker itself will be designated a Consent Manager — or will remain a document rails distinct from the DPDP consent machinery — has not been formally resolved. [^11][^23]

**Financial-sector recognition.** RBI's KYC framework accepts DigiLocker-fetched issuer-signed documents as Officially Valid Documents, and **CKYC 2.0** formally integrates DigiLocker with the Central KYC Records Registry, making DigiLocker a structural part of onboarding infrastructure. From **1 April 2026**, banks are required to trigger DigiLocker-based verification for transactions flagged as high-risk, adding a document-verification layer beyond OTPs. [^19][^27]

## Citizen Rights Analysis

DigiLocker confers concrete rights — and contains a quiet asymmetry:

1. **Right to legal equivalence.** For issued documents, citizens hold a statutory right to have digital documents accepted at par with originals by any authority, backed by Rule 9A and sector-specific rules. When a traffic officer or bank refuses a DigiLocker licence, the citizen is on legally solid ground — MoRTH's own SOP directs enforcement staff to validate such documents. [^3][^13][^14]
2. **Ownership and control.** The Terms of Use state users "retain complete ownership of all content" they upload, store, share or transmit; NeGD "does not access, read, or interpret the data stored by users"; and no fees may be charged for accessing issued documents. [^11]
3. **Consent rights.** Every fetch and share requires explicit consent; consent details are logged and governed by applicable data-protection laws; the My Consent dashboard allows inspection, time-limits and instant revocation. [^8][^11]
4. **Deletion and exit.** Users can delete their account and data at any time, and appeal or seek judicial review of any restriction or enforcement action against their account. [^11]
5. **Children's protections.** DigiLocker does not knowingly collect personal data of under-18s without verifiable parental or guardian consent. [^11]

**The caveats citizens should know:**

- **Voluntary in text, near-mandatory in practice.** Aadhaar is "voluntary" under the Terms, yet issued documents — the platform's core value — require Aadhaar linking, and government programmes repeatedly convert DigiLocker-adjacent systems into de facto mandates. CBSE made the DigiLocker-linked APAAR ID compulsory for Class 10 and 12 board-exam registration, prompting rights-group criticism that a nominally voluntary ID was made unavoidable; the Odisha High Court directed the government to amend the model consent form so parents can actually refuse. [^20][^21]
- **Equivalence does not cover uploads.** The "at par with original" guarantee applies only to *issued* documents; a citizen showing a self-uploaded scan has no statutory protection. [^3]
- **Kin cannot inherit the locker.** There is no nomination facility; on a user's death, family access to documents in the account is not provided for — a long-standing gap flagged publicly. [^21]
- **Digital access is now a fundamental right — DigiLocker presumes it.** The Supreme Court's 30 April 2025 judgment recognised digital access as part of the right to life (Article 21) after e-KYC exclusions; DigiLocker's dependence on smartphones, OTPs and connectivity means exclusion risks fall on precisely the populations DPI claims to serve — migrant workers, the elderly, and those with name mismatches across databases. [^22]

## Privacy Implications

- **A single high-value repository.** DigiLocker aggregates the state's paper trail on a citizen — identity, education, property, health, employment — behind one Aadhaar-linked login. It has no known public breach, but the concentration itself is the risk surface, and it sits inside the wider Aadhaar-authentication ecosystem.
- **Metadata is inspectable; content needs judicial authorisation.** The Terms of Use permit inspection of *metadata* (file names, sizes, timestamps, URIs) for compliance, with access to user content only "after proper judicial authorization" — DigiLocker states it does not proactively monitor content. The line between metadata and content in a document vault deserves citizen scrutiny. [^11]
- **Consent logs are retained**, and authentication logs are retained "as provided under law" — necessary for auditability, but another trail linking citizen to every verification. [^11]
- **Function creep is observable, not hypothetical.** A platform built for document storage now verifies high-risk bank transactions, feeds CKYC 2.0 onboarding, and powers national single sign-on. Each extension is individually defensible; collectively they expand DigiLocker's role in citizen surveillance infrastructure without a dedicated statutory framework beyond the 2016 Rules. [^19][^26][^27]
- **Ecosystem coupling.** DigiLocker is one of the services tied to a citizen's phone number in the new telecom verification regime — Internet Freedom Foundation has flagged how face-scan SIM verification (Telecommunications (User Identification) Rules, 2026) interlocks with Aadhaar e-KYC, DigiLocker and welfare access, so a failed biometric can cascade across services. [^22]
- **Minors' education records.** APAAR and the Academic Bank of Credits flow academic records into DigiLocker from childhood; researchers have raised profiling and surveillance concerns about centralised education repositories and minors' data without mature safeguards. [^20]
- **Data localisation.** The Terms commit that confidential user data "will not be stored or processed outside India." [^11]

## Safeguards

- **Statutory equivalence with built-in authenticity**: only digitally signed issued documents qualify; the URI links requesters to the issuer's repository as the single source of truth, making forged-document fraud structurally harder. [^3][^12]
- **Certified security management**: DigiLocker operates an ISMS compliant with **ISO/IEC 27001:2022**; documents are signed with Digital Signature Certificates; requesters integrate via OAuth 2.0 with PKI-authenticated consent; the platform runs behind a WAF with load-balancer monitoring (ALB/ELK), multi-zone backups, timed log-outs and JWT session tokens. [^8][^12]
- **Independent audits**: regular security audits by CERT-In empaneled agencies; periodic compliance audits covering security policies, technology and contracts under applicable law. [^11][^12]
- **Consent machinery**: granular, revocable, logged consent with PKI enforcement and the My Consent dashboard. [^8][^12]
- **Localisation + no content processing**: data stays in India; the platform commits not to read, process or analyse stored content. [^11]
- **Service guarantees**: issued documents are free; 1 GB storage is free; premium add-ons (DigiLocker Drive) are optional and separately priced. [^11]
- **What is still missing**: a nomination/inheritance mechanism, a formal privacy-breach notification regime tied to the (not-yet-constituted) Data Protection Board, and an independent oversight structure for a platform whose rulebook — the 2016 Rules — predates the DPDP era. [^11][^23]

## Complaints & Grievance Redressal

1. **DigiLocker support portal.** Raise and track a ticket at support.digilocker.gov.in (covers DigiLocker and Entity Locker); users may also write to helpdesk@negd.in. [^24]
2. **Helpline.** DigiLocker's published helpline number is **10505**; partner/issuer coordination runs through digilocker-partners@negd.in. [^25]
3. **Wrong or mismatched document?** Complain to the *issuing authority* (RTO, board, university, EPFO) — DigiLocker only mirrors the issuer's repository; fixing the source fixes the locker.
4. **Refusal to accept a DigiLocker document.** Cite Rule 9A (and for vehicle documents, MoRTH's Rule 139 amendment + validation SOP); escalate to the refusing organisation's grievance officer and, if needed, CPGRAMS (pgportal.gov.in) against the department concerned. [^3][^13]
5. **Account suspension or enforcement action.** The Terms of Use grant a right to appeal and seek judicial review. [^11]
6. **Privacy complaints (prospective).** Once the Data Protection Board is functional and the Consent Manager regime activates on 13 November 2026, DPDP-specific remedies — with substantial penalty power — become available for consent violations. [^23]

## Prime References

[^1]: https://www.digilocker.gov.in/web/about/about-digilocker
[^2]: https://cdn.digilocker.gov.in/assets/img/digi_locker_rules_and_amendment.pdf
[^3]: https://indiankanoon.org/doc/8414178
[^4]: https://www.sarkaritel.com/digilocker-72-43-crore-users-umang-11-66-crore-users
[^5]: https://www.digilocker.gov.in
[^6]: https://x.com/PIBShimla/status/2072165973201932734
[^7]: https://dic.gov.in/digilocker
[^8]: https://negd.gov.in/blog/digilocker-the-digital-briefcase-for-indias-authentic-e-documents
[^9]: https://www.ucl.ac.uk/bartlett/sites/bartlett/files/2025-10/The%20DigiLocker%20Story.pdf
[^10]: https://en.wikipedia.org/wiki/DigiLocker
[^11]: https://www.digilocker.gov.in/web/about/tos
[^12]: https://www.digilocker.gov.in/web/security-architecture
[^13]: https://parivahan.gov.in/sites/default/files/NOTIFICATION%26ADVISORY/17th%20Dec%202018.pdf
[^14]: https://www.pib.gov.in/newsite/PrintRelease.aspx?relid=181696
[^15]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2094574
[^16]: https://www.news18.com/india/indias-digital-push-goes-global-24-nations-embrace-india-stack-upi-digilocker-ws-l-10241876.html
[^17]: https://tele.net.in/india-inks-pacts-with-23-countries-for-cooperation-on-dpi
[^18]: https://cf-media.api-setu.in/resources/DigiLocker_International_SOP_09062026.pdf
[^19]: https://www.financialexpress.com/life/technology-digilocker-2026-update-from-april-1-heres-how-to-use-it-for-verifying-high-risk-bank-transactions-4181757
[^20]: https://www.biometricupdate.com/202508/decision-to-mandate-use-of-student-id-for-board-exams-in-india-prompts-criticism
[^21]: https://forum.internetfreedom.in/t/regarding-digilocker/626.html
[^22]: https://internetfreedom.in/when-kyc-becomes-a-barrier-supreme-courts-stand-for-digital-inclusion/
[^23]: https://www.legal500.com/en/intelligence/india/privacy/consent-managers-are-india's-next-big-opportunity-here's-the-faq-you-need
[^24]: https://support.digilocker.gov.in
[^25]: https://www.digilocker.gov.in/web/partners/help-and-support
[^26]: https://apisetu.gov.in/digilocker
[^27]: https://www.befisc.com/fintechsherlock/digilocker-kyc-verification-india
[^28]: https://blog.mygov.in/digital-locker-scheduled-to-be-launched-on-1st-july-2015-by-the-hon-prime-minister
