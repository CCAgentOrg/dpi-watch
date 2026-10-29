---
title: "Ayushman Bharat Digital Mission 101: India's Digital Health Rails, ABHA and the Consent Question"
description: "A comprehensive, fact-checked guide to the Ayushman Bharat Digital Mission (ABDM) — the ABHA health ID, health facility and professional registries, the HIE-CM consent framework, National Health Claims Exchange, adoption statistics, the Health Data Management Policy, the DPDP overlay, mandatory-ABHA practice, privacy risks, and grievance routes."
date: 2026-10-29
draft: false
tags: ["abdm", "abha", "digital-health", "national-health-authority", "health-data-management-policy", "dpdp", "consent", "nhcx", "uhi", "aarogya-setu", "digital-india", "dpi", "privacy", "india"]
categories: ["DPI Basics"]
author: "CashlessConsumer"
readingTime: "17 min"
---

# Ayushman Bharat Digital Mission 101: India's Digital Health Rails, ABHA and the Consent Question

## What is the Ayushman Bharat Digital Mission (ABDM)?

The **Ayushman Bharat Digital Mission (ABDM)** is India's flagship digital public infrastructure programme for healthcare, implemented by the **National Health Authority (NHA)** — the attached office of the Ministry of Health and Family Welfare that also runs the Ayushman Bharat PM-JAY insurance scheme. [^1][^5] Its stated purpose is to develop "the backbone necessary to support the integrated digital health infrastructure of the country" and to bridge the gap between stakeholders in the healthcare ecosystem — patients, doctors, hospitals, laboratories, pharmacies and insurers — through interoperable digital rails. [^1][^5]

ABDM's best-known component is the **ABHA number** — a 14-digit, randomly generated health identifier that citizens can create **voluntarily** and use to link their health records across facilities. [^9][^15] The government describes ABHA as "a unique identifier like Aadhaar that securely links individuals to the wider health system". [^3] Unlike Aadhaar, ABDM is designed around a **federated** architecture: the NHA does not store citizens' health records; records remain with the healthcare provider ("Health Information Provider" or HIP) that generated them, and move only through **consent artefacts** managed by a Health Information Exchange–Consent Manager (HIE-CM). [^9][^14]

Beyond the ID itself, ABDM is a full ecosystem: national registries of facilities and professionals, a consent-driven records exchange, an open appointment/discovery network (**Unified Health Interface** or UHI — pitched as "like UPI for healthcare"), a claims exchange (**NHCX**), and a citizen app (**Aarogya Setu 2.0** since June 2026). [^3] ABDM is also a major export asset in India's "DPI diplomacy" — the World Bank documents it as a template for nationwide digital health. [^5]

The citizen-rights picture is genuinely two-sided. On paper, participation is voluntary, consent is granular and revocable, and the HDM Policy promises that no one will be denied care for refusing an ABHA. [^9] In practice, medical regulators and state hospitals have made ABHA **de-facto mandatory** for registration, COVID-era records show millions of health IDs were created without meaningful consent, and India's data protection law deliberately declines to give health data any special status. [^16][^17][^18][^27]

### Historical Context

| Date | Milestone |
|---|---|
| 2017 | National Health Policy recommends an integrated digital health system; groundwork begins [^6] |
| 2019 | National Digital Health Blueprint (NDHB) published, proposing a layered digital health ecosystem [^6] |
| 15 Aug 2020 | Prime Minister announces the **National Digital Health Mission (NDHM)**; pilot begins in select Union Territories [^6] |
| 26 Aug 2020 | Draft National Health Data Management Policy released for consultation [^7] |
| Dec 2020 | **Health Data Management Policy (HDM Policy) v1** finalised and published by NHA [^8] |
| 27 Sep 2021 | **ABDM launched nationally** by the Prime Minister (on PM-JAY's third anniversary); NDHM renamed ABDM, Health ID renamed ABHA [^5][^30] |
| 2021 | Controversy over health IDs auto-created through CoWIN during COVID vaccination [^16][^17] |
| 2022 | **Scan & Share** OPD registration service launched [^3] |
| 23 Apr 2022 | Revised draft HDM Policy v2 released for consultation (a finalised v2 has not been published since) [^8] |
| 3 Apr 2024 | CGHS makes ABHA creation/linking part of beneficiary registration [^21] |
| Jun 2024 | **NHCX** (National Health Claims Exchange) goes live; 34 insurers/TPAs live by 21 Jul 2024 [^13] |
| Jun 2024 | National Medical Commission directs ABHA-based registration in medical college hospitals [^18][^19] |
| 14 Nov 2025 | **DPDP Rules 2025** notified, operationalising the Digital Personal Data Protection Act, 2023 in phases [^25][^26] |
| 6 Jul 2026 | PIB: over **104 crore health records** linked to over **93 crore ABHA accounts** [^3] |
| 29 Jun 2026 | **Aarogya Setu 2.0** launched as unified citizen health app and PHR [^3] |
| 26 Oct 2026 | ABDM dashboard: **98,67,69,992** ABHA numbers created [^4] |

## How It Works

### The Building Blocks

| Component | What it is |
|---|---|
| **ABHA number** | 14-digit randomly generated unique health identifier, created voluntarily (via Aadhaar with OTP/demographic authentication, via Driving Licence with offline facility KYC, or via mobile number with later verification). The number itself carries no health data. [^9][^15] |
| **ABHA address** | A self-chosen username in the form `username@abdm` (or another HIE-CM domain like `@sbx`), working like an email address for consent-based exchange. One ABHA number can hold multiple ABHA addresses. [^14][^15] |
| **ABHA card / PHR apps** | Downloadable ABHA card; Personal Health Record (PHR) applications — now including Aarogya Setu 2.0 — through which citizens hold and share records. [^3][^15] |
| **Health Facility Registry (HFR)** | National, verified registry of all health facilities — hospitals, clinics, labs, diagnostic centres, pharmacies, blood banks, public and private. [^3][^11] |
| **Healthcare Professionals Registry (HPR)** | National registry of verified healthcare professionals across all systems of medicine, including AYUSH practitioners. [^3][^10] |
| **HIE-CM (Consent Manager)** | The Health Information Exchange–Consent Manager issues, logs and enforces **consent artefacts**; HIPs (providers) share records only against a valid consent, and every exchange is digitally signed and logged. [^14][^32] |
| **HIP / HIU** | Health Information Providers hold and link records to a care context (each patient encounter); Health Information Users (hospitals, insurers, apps) request records through the gateway with consent. NHA itself stores no patient records. [^14] |
| **UHI (Unified Health Interface)** | An open network for discovering doctors, booking teleconsultations and in-person appointments across apps. [^3] |
| **NHCX (National Health Claims Exchange)** | A FHIR-based gateway for health insurance claims between hospitals, insurers and TPAs, built under ABDM with IRDAI support. [^13] |
| **Aarogya Setu 2.0** | The 2026 revamp of the COVID app into a full citizen gateway: ABHA creation, Scan & Register, Smart Reports (OCR), PM-JAY wallet and private insurance view via NHCX, e-RaktKosh blood availability, UHI bookings, wearable syncing and AI-driven health insights. [^3] |

### The Consent Flow

1. A citizen's records are linked to their ABHA number by the facility that generated them (each encounter becomes a "care context" at the HIP). [^14]
2. A requesting hospital, insurer or app (HIU) asks the citizen — via the HIE-CM — for specific records.
3. The citizen receives a **consent request** specifying who is asking, what data, for what purpose, and for how long; the consent artefact is purpose-bound, time-bound, and revocable at any time through the "My consent" section. [^9][^15][^32]
4. If granted, records travel encrypted from HIP to HIU through the gateway, digitally signed and logged; the NHA never holds the records themselves. [^14]

### Scan & Share

Launched in 2022, **Scan & Share** lets patients scan a QR code at a participating facility to generate a digital OPD queue token, with demographic details pulled from their ABHA into the facility's Health Information System — cutting registration queues without paperwork. [^3]

## Key Statistics (with sources)

⚠️ **Reading the numbers:** ABDM's headline counts move fast and different sources snap at different dates; "records linked" also varies by counting window. Where two official numbers conflict, both are shown.

| Metric | Figure | As of | Source |
|---|---|---|---|
| ABHA numbers created | **98,67,69,992** (~98.67 crore) | 26 Oct 2026 | ABDM-Insights dashboard [^4] |
| ABHA numbers (earlier snapshots) | 93 crore (PIB, 6 Jul 2026); 93.95 crore (JP Nadda); 97.8 crore (NHA video, 1 Sep 2026) | — | [^3][^37][^38] |
| Health records linked | **104+ crore** (PIB); **121 crore** (NHA, 1 Sep 2026) | Jul/Sep 2026 | [^3][^37] |
| ABHA created in FY 2025-26 | 8.79 crore by 28 Jan 2026 | — | peer-reviewed study citing government data [^23] |
| Facilities on HFR | **5.36 lakh** (govt reply, 20 Jul 2026); 5,74,159 (dashboard, 10 Sep 2026) | 2026 | [^11][^12] |
| Professionals on HPR | 10,91,380 registered (10 Sep 2026); dashboard shows ~5.93 lakh "verified" — counting methods differ | 2026 | [^12][^4] |
| Earlier registry counts | HFR 4.18 lakh; HPR 6.79 lakh | 5 Aug 2025 | [^10] |
| Scan & Share tokens issued | **23.21 crore** ABHA-linked tokens | 18 Jun 2026 | [^3] |
| Waiting-time reduction (IIHMR study) | ~1 hour → **2–5 minutes** | 2026 | [^3] |
| Digital Health Incentive Scheme payouts | Hospitals ₹107+ crore; diagnostics/labs/pharmacies ₹2.95 crore; digital solution companies ₹26+ crore | 18 Jun 2026 | [^3][^24] |
| Insurers/TPAs live on NHCX | 34 | 21 Jul 2024 | [^13] |
| ABHA registrations vs OPD footfall | ~20–33% of OPD patients in a 2024–25 OPD study; only 10% platform engagement in a 2021 national survey | 2026 | [^23] |
| Patient trust | 55% comfortable with ABDM data privacy; 49.6% concerned about data misuse | 2026 study | [^23] |

## Layers Classification (L1–L7)

Based on the IndiaStack Layers framework, ABDM occupies the following positions:

| Layer | Classification | ABDM's Role |
|---|---|---|
| **L1 — Vision & Policy** | Government policy | National Health Policy 2017; National Digital Health Blueprint 2019; NDHM announced 15 Aug 2020; ABDM national launch 27 Sep 2021 [^5][^6] |
| **L2 — Regulation** | Regulatory framework | **HDM Policy (Dec 2020)** — a "guidance document", not a statute; DPDP Act 2023 + DPDP Rules 2025 as the data-protection overlay; EHR Standards; sectoral directives (NMC, IRDAI, CGHS); notably **no dedicated ABDM statute exists** [^8][^9][^26][^30] |
| **L3 — Digital Rails** | Core infrastructure | ABHA, HFR, HPR, HIE-CM consent gateway, NHCX, UHI, PHR/Aarogya Setu 2.0 — the federated exchange backbone [^3][^14] |
| **L4 — APIs & Protocols** | Open standards | ABDM Sandbox APIs (ABHA, HIP, HIU, consent), **FHIR R4** record and claim formats, NHCX technical specifications v2.0, ABHA address/HIE-CM domain scheme [^13][^14][^15] |
| **L5 — Applications** | End-user apps | ABHA app/Aarogya Setu 2.0, PHR applications, UMANG, Scan & Share, facility HMS software integrating via M1–M3 milestones [^3][^23] |
| **L6 — Use Cases** | Sectoral applications | OPD/IPD registration, record linkage and portability, insurance claims (NHCX), teleconsultation (UHI/eSanjeevani), PM-JAY wallet, blood-bank discovery (e-RaktKosh), wellness insights [^3] |
| **L7 — Analytics & Intelligence** | Data & insights | ABDM-Insights dashboard; PIB explicitly touts "anonymised health data" for planning, disease surveillance and "powering India's emerging AI ecosystem" [^3][^4] |

ABDM is best read as an **L3–L4 construct** — public rails (identity + registries + consent exchange) onto which hospitals, apps and insurers plug in. Its distinctiveness among DPI components is that the most sensitive personal data category in any citizen's life is the payload.

## Regulatory Framework

### The core problem: policy, not law

ABDM's data-governance backbone remains the **Health Data Management Policy**, finalised in December 2020 — which the policy itself describes as a "guidance document" that "sets out the minimum standard for data privacy protection", to be read alongside applicable law. [^8][^9] A revised draft (v2) was released on 23 April 2022 inviting comments by 21 May 2022; **no finalised v2 has been publicly published since**, leaving the operative policy nearly six years old. [^8] There is **no dedicated statute** for ABDM or health data — Internet Freedom Foundation's consultation critique flagged exactly this: "a weak legal foundation… excessive delegation; a constricted digital consent, confidentiality and privacy framework; over-reliance on an Aadhaar-based authentication system; and vague systems for anonymisation". [^30]

Key HDM Policy commitments on the record: [^9]

- Participation in the ecosystem, and linking of records to ABHA, is **voluntary**.
- **Failure or refusal to use Aadhaar must not result in denial of access** to any health facility or service (voluntary Aadhaar per the Aadhaar Authentication for Good Governance Rules, 2020).
- Records are **individual-owned**; HIPs act as data fiduciaries; consent is specific, informed, purpose- and time-bound. [^2]

### The DPDP overlay

The **Digital Personal Data Protection Act, 2023**, operationalised by the **DPDP Rules, 2025** (notified 13–14 November 2025, G.S.R. 846(E)), now applies to every hospital, insurer, PHR app and NHA itself as data fiduciaries. [^26] Implementation is phased: the four-member **Data Protection Board** stood up in November 2025; **consent-manager registration** opens 14 November 2026; and full substantive compliance (notice, security, breach reporting, data-principal rights, cross-border rules) lands **14 May 2027**. [^25][^26]

Two structural weaknesses matter for health data specifically: [^27][^28]

1. **No "sensitive personal data" category.** The DPDP Act scrapped the IT SPDI Rules' special treatment of medical/health data and applies one uniform standard to all personal data. Extra obligations arise only if a fiduciary is designated a **Significant Data Fiduciary** (Section 10 lets government use "sensitivity of data" as a criterion) — but no general health-data uplift exists.
2. **Wide government exemptions** and the companion amendment to the RTI Act ("no obligation to give any citizen information which relates to personal information") reduce independent oversight of exactly the kind of state-run databases ABDM builds. [^26][^29]

### Sectoral regulation

- **National Medical Commission**: June 2024 direction that all patients in medical college hospitals be registered with an ABHA ID alongside the hospital UHID — tying ABHA adoption to medical-college seat-maintenance assessments. [^18][^19]
- **IRDAI**: regulatory push for insurers/TPAs to onboard NHCX for claims interoperability. [^13]
- **CGHS**: ABHA creation/linking embedded in central government health beneficiary workflows (April 2024). [^21]
- **EHR Standards & sandbox specs**: FHIR R4-based interoperability standards and M1–M3 integration milestones for ABDM-enabled software. [^13][^14]

## Citizen Rights Analysis

### Rights on paper

- **Voluntary participation**: creating an ABHA is optional; the HDM Policy states refusal to use Aadhaar or ABHA cannot cause denial of care. [^9]
- **Granular, revocable consent**: every data request must carry a purpose and duration; consent can be revoked anytime via the "My consent" tab, and every exchange is logged and auditable. [^9][^15][^32]
- **Deletion**: the ABHA Privacy Policy states users "may request deletion of their ABHA account and associated personal data at any time by using the account deletion feature"; temporary deactivation is also available. [^31]
- **DPDP rights** (phasing in through May 2027): access, correction/completion, erasure, grievance redressal, nomination, and the right to complain to the Data Protection Board. [^25][^27]

### Rights in practice — where the paper and the queue diverge

- **Mandatory by directive.** Since June 2024, NMC directives require ABHA-based registration for all OPD and IPD patients in medical college hospitals; [^18][^19] CGHS has embedded ABHA in beneficiary onboarding; [^21] and in January 2026 Jaipur hospitals made ABHA mandatory for OPD, IPD **and emergency** registration. [^20] Clinician testimony and policy commentary report states making ABHA part of outpatient registration with real risks of delay or denial for those without Aadhaar — "on paper of course the Aadhaar card is voluntary, but in the implementation it's mandatory". [^22]
- **Consent already compromised at scale.** The Caravan documented COVID-vaccine beneficiaries assigned unique health IDs without their consent during verification; [^16] SFLC.in research estimates **~40% of 328 million ABHA IDs originated from CoWIN**, "in many cases… automatically generated without any information or consent from the user" when Aadhaar was used for vaccination booking. [^17]
- **Adoption is thinner than the headline.** A 2026 peer-reviewed OPD study found only ~20–33% of walk-in patients registered via ABHA despite facility pushes, with adoption limited by digital literacy, awareness, cost and **privacy distrust** — 49.6% of patients feared data misuse. [^23]
- **No special protection for the most sensitive data.** Health data gets the same legal treatment as an email address under DPDP — no category uplift, no health-specific consent threshold. [^27][^28]

**Net assessment:** the rights architecture is real and, on consent design, genuinely stronger than most Indian DPI consent regimes — but the mandatory-by-default drift across NMC/CGHS/state hospitals has largely hollowed out the "voluntary" promise for anyone using public healthcare, and the CoWIN precedent shows what "voluntary" converges to under programme pressure.

## Privacy Implications

- **Federated ≠ unlinkable.** NHA holds no records (a genuine safeguard), [^14] but the ABHA number — especially when Aadhaar-seeded — functions as a **join key** across every facility, insurer and app that adopts it. The identifier, not the records, is the centralisation risk.
- **Secondary use is the roadmap, not a side effect.** The government's own backgrounder lists "generates anonymised health data" for planning, disease surveillance **and powering India's AI ecosystem** as a benefit. [^3] Anonymisation standards were called "vague" by IFF during policy consultation, [^30] and India has no statutory anonymisation safe-harbour definition for health data.
- **No sensitive-data category + government exemptions + RTI narrowing** = reduced structural checks on state-side processing of the country's health database. [^26][^27][^29]
- **The breach environment is not theoretical.** September 2024: ~31 million Indians' health-insurance data from Star Health surfaced on Telegram; [^17] MediaNama reported exposure of sensitive ABDM dashboard data. [^17] Federated design reduces (but does not eliminate) blast radius, and ABDM's attack surface grows with each integration — Aarogya Setu 2.0 alone adds OCR'd documents, insurance details, wearables and AI-driven biomarker insights to the citizen data trail. [^3]
- **Deletion has a boundary.** Deleting or deactivating ABHA stops future consent-based exchange, but does **not** compel hospitals to delete the clinical records they already hold in their own systems under their own retention obligations. [^31][^32] Opting out of ABDM is not the same as opting out of digitised medicine.

## Safeguards

- **Purpose- and time-bound consent artefacts**, digitally signed, centrally logged, revocable at will — enforced through the HIE-CM rather than hospital goodwill. [^14][^32]
- **Federated storage**: records stay at the generating HIP; NHA stores none. [^9][^14]
- **Verified provider registries** (HFR/HPR) mean citizens can check who they are sharing with; requests come from identified, registered facilities and professionals. [^3][^15]
- **Encrypted, signed exchange** over the gateway with audit trails on every transfer. [^14][^32]
- **DPDP compliance phasing in** (through May 2027): breach notification to affected users, security safeguards, data-retention limits, DPO/SDF duties for large fiduciaries, and an accessible Data Protection Board. [^25][^26]
- **Incentive-scheme compliance conditions**: DHIS payouts are conditioned on adherence to ABDM's data-protection, security and interoperability standards. [^3]

**What is still missing:** a statutory basis for ABDM itself, a finalised post-2022 HDM Policy, health-data-specific DPDP obligations, and enforceable consequences for hospitals that deny care without ABHA. [^8][^20][^22][^30]

## Complaints & Grievance Redressal

| Channel | What it handles |
|---|---|
| **ABDM grievance portal** (abdm.gov.in/grievance) | Register, track grievances and report IT incidents related to ABDM/ABHA services [^35] |
| **Helpline: 14477 / 1800-11-4477** | 24×7 toll-free, multi-language (Hindi, English, Tamil, Telugu and others) — Health ID registration, health records and related grievances [^33] |
| **Email: abdm[at]nha[dot]gov[dot]in** | NHA support; address: 9th Floor, Tower-I, Jeevan Bharati Building, Connaught Place, New Delhi – 110001 [^34] |
| **CGRMS** (cgrms.pmjay.gov.in) | Grievances about Ayushman Bharat PM-JAY treatment/claims [^36] |
| **DPDP route** (phasing in) | Grievance officer of the fiduciary (hospital/insurer/app), then the Data Protection Board portal — fully operational for rights complaints as substantive obligations land by 14 May 2027 [^25][^26] |
| **Consumer commissions / courts** | Denial-of-care disputes; the HDM Policy's no-denial commitment is quotable, though not statute-backed [^9][^22] |

**Practical citizen playbook:**

1. Before granting any consent request, check who is asking (HFR/HPR registration) and the expiry/purpose on the artefact.
2. Review and revoke unused consents from the "My consent" section of your PHR/ABHA app.
3. If opting out: deactivate or delete ABHA via the account settings, and know that existing hospital records remain with the hospitals. [^31][^32]
4. Escalate: helpline → grievance portal (keep the reference number) → DPDP grievance officer/Board as it operationalises.
5. If care is denied or delayed over an ABHA refusal, record the date/facility — that is a policy violation worth reporting, not a personal failing. [^9][^22]

## Prime References

[^1]: https://abdm.gov.in/abdm
[^2]: https://www.niti.gov.in/sites/default/files/2021-09/ndhm_strategy_overview.pdf
[^3]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2281466&reg=3&lang=1
[^4]: https://dashboard.abdm.gov.in/abdm
[^5]: https://documents1.worldbank.org/curated/en/099081723223028498/pdf/P1750750936a760320bfb9066084a6084bf.pdf
[^6]: https://www.niti.gov.in/sites/default/files/2021-09/ndhm_strategy_overview.pdf
[^7]: https://factly.in/review-what-does-the-draft-national-health-data-management-policy-contain
[^8]: https://www.expresshealthcare.in/news/nha-releases-revised-draft-of-heath-data-management-policy/434731
[^9]: https://abdm.gov.in/strapicms/uploads/health_management_policy_bac9429a79.pdf
[^10]: https://sambodhi.co.in/national-digital-health-mission-designing-the-blueprint-for-a-unified-health-ecosystem
[^11]: https://www.medicalbuyer.co.in/centre-creates-health-facility-registry-under-abdm-registers-5-36l-facilities
[^12]: https://zivyaa.co.in/blog/hfr-hpr-registration-guide
[^13]: https://www.pib.gov.in/Pressreleaseshare.aspx?PRID=2037634&reg=48&lang=2
[^14]: https://abdm.gov.in/strapicms/uploads/HIP_HIU_Guidelines_f85df336ec.pdf
[^15]: https://docs.abdm.gov.in/docs/hiecm/v3/getting-started/glossary
[^16]: https://caravanmagazine.in/health/covid-19-vaccine-beneficiaries-were-assigned-unique-health-ids-without-their-consent
[^17]: https://indiastack.in/health
[^18]: https://www.business-standard.com/india-news/abha-id-must-for-patients-in-medical-college-hospitals-how-to-create-one-124060700395_1.html
[^19]: https://www.medianama.com/2024/06/223-nmc-mandating-abha-id-medical-college-patient-registrations
[^20]: https://timesofindia.indiatimes.com/city/jaipur/abha-id-now-mandatory-for-opd-emergency-registration/articleshow/127727998.cms
[^21]: https://dtf.in/wp-content/files/ABHA_Ayushman_Bharat_Health_Account_-_Frequently_Asked_Questions_As_on_CGHS_Website-03.04.2024.pdf
[^22]: https://rthresources.in/conversations-on-health-policy/digitization-of-health-services-part-i-decoding-the-ayushman-bharat-digital-mission-abdm
[^23]: https://pmc.ncbi.nlm.nih.gov/articles/PMC13078079
[^24]: https://ddindia.co.in/2026/07/ayushman-bharat-digital-mission-how-india-is-building-a-paperless-healthcare-ecosystem
[^25]: https://www.scrut.io/post/dpdp-rules
[^26]: https://www.seclore.com/fundamentals/dpdp-rules-2025-compliance-guide
[^27]: https://www.legal500.com/intelligence/india/privacy/personal-data-vs-sensitive-personal-data-understanding-the-legal-difference
[^28]: https://ccgnludelhi.wordpress.com/2024/02/13/personal-health-data-under-the-digital-personal-data-protection-act-2023-private-and-esoteric
[^29]: https://obhanmason.com/blog/the-digital-personal-data-protection-rules-2025-a-new-digital-frontier
[^30]: https://internetfreedom.in/second-times-not-the-charm-health-data-management-policy-misses-the-mark-again
[^31]: https://abdm.gov.in/abha-PRIVACY-POLICY-english
[^32]: https://www.plumhq.com/blog/what-is-abha
[^33]: https://x.com/AyushmanNHA/status/1826529772517949469
[^34]: https://abdm.gov.in/scan-register/contact
[^35]: https://jaagrukbharat.com/ayushman-bharat-digital-mission-6109997
[^36]: https://cgrms.pmjay.gov.in
[^37]: https://www.facebook.com/News18TamilNadu/posts/as-of-1-september-2026-over-978-crore-abha-ids-had-been-created-with-more-than-1/1567200755442107
[^38]: https://ddnews.gov.in/en/ayushman-bharat-digital-mission-emerges-as-one-of-worlds-largest-digital-health-ecosystems-with-over-93-95-crore-abha-ids-j-p-nadda
