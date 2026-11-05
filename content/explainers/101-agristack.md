---
title: "AgriStack 101: India's Farmer ID, the Digital Crop Survey and the Consent Question"
description: "A comprehensive, fact-checked guide to AgriStack — the farmer-centric Digital Public Infrastructure built under the Digital Agriculture Mission: the Farmer ID and how land buckets are claimed, the Digital Crop Survey and Crop Sown Registry, the AgriStack Consent Manager, Krishi-DSS, adoption statistics, the DPDP overlay, the tenant-farmer exclusion problem, privacy risks, and grievance routes."
date: 2026-11-05
draft: false
tags: ["agristack", "farmer-id", "farmer-registry", "digital-agriculture-mission", "digital-crop-survey", "krishi-dss", "consent-manager", "dpdp", "land-records", "tenant-farmers", "digital-india", "dpi", "privacy", "india"]
categories: ["DPI Basics"]
author: "CashlessConsumer"
readingTime: "18 min"
---

# AgriStack 101: India's Farmer ID, the Digital Crop Survey and the Consent Question

## What is AgriStack?

**AgriStack** is India's Digital Public Infrastructure (DPI) for agriculture — a federated set of registries that, together, answer three questions about every farm household: *who is the farmer, where is the land, and what is growing on it?* [^1][^2] It is the flagship component of the **Digital Agriculture Mission**, an umbrella scheme approved by the Union Cabinet on 2 September 2024 with an outlay of ₹2,817 crore (central share ₹1,940 crore), run by the Ministry of Agriculture and Farmers' Welfare with the state governments, who create and maintain all of AgriStack's core registries. [^3]

AgriStack's best-known component is the **Farmer ID** — a digitally verifiable identity for farmers pitched as "similar to an Aadhaar card". [^3] The Ministry describes AgriStack as "the farmer-centric DPI built as a public good for efficient, easier and faster service and scheme delivery", giving every enrolled farmer a comprehensive profile: identity, land records, crops grown, and assets such as livestock and fisheries. [^1] The system's promise is familiar from India's other DPIs: authenticate once, and scheme benefits, crop insurance, Kisan Credit Card loans and disaster relief flow without repeated paperwork. [^1] The 2026 achievement of its headline target — **11 crore Farmer IDs created by the night of 23 October 2026, five months ahead of the 31 March 2027 deadline** — was announced by the government as a "major milestone in digital agriculture". [^1][^4]

Finance Minister Nirmala Sitharaman has publicly held AgriStack up as "the next UPI" — the intuition being that a verified, interoperable identity-plus-data layer will do for farm services what UPI did for payments. [^5] Whether the analogy holds is exactly where the citizen-rights debate sits: payments data is transactional, but AgriStack's payload is identity + land + crop + benefits — the data that determines whether a rural household is seen as a farmer at all.

### Historical Context

| Date | Milestone |
|---|---|
| 2020–21 | Deliberations on a unified agri-data ecosystem begin; the Ministry's draft **IDEA** (India Digital Ecosystem of Agriculture) architecture proposes "federators, building blocks and frameworks" for farm data [^6] |
| Jun 2021 | IDEA consultation paper published; the plan — piloted with major tech companies on farmer databases — draws national criticism over privacy and exclusion amid the farm-law protests; Reuters reports fears that farmers' data could be passed to private firms under weaker-than-Aadhaar safeguards [^7][^6] |
| 1 Feb 2023 | Union Budget 2023-24 announces **DPI for agriculture** — "an open-source, open standard and interoperable digital public infrastructure" — as a national priority [^3] |
| 2 Sep 2024 | Union Cabinet approves the **Digital Agriculture Mission** (₹2,817 crore; two pillars: AgriStack and Krishi Decision Support System, plus Soil Profile Mapping and DGCES); targets set for 11 crore Farmer IDs in three years and a nationwide Digital Crop Survey; 19 states have signed MoUs, with pilots in six districts (UP, Gujarat, Maharashtra, Haryana, Punjab, Tamil Nadu) [^3] |
| 23 Sep 2024 | Operational Guidelines issued to states for Farmer Registry and DCS implementation [^8] |
| 28 Mar 2025 | 4.86 crore Farmer IDs generated; DCS conducted in 436 districts (Kharif 2024) and 461 districts / 23.9 crore plots (Rabi 2024-25) [^9] |
| 19 Mar 2026 | Farmers Registry crosses **9.20 crore** Farmer IDs [^10] |
| 28 Jul 2026 | Government tells the Rajya Sabha: 10.25 crore Farmer IDs; Rabi 2025-26 DCS covered **648 districts and 31.3 crore plots**; soil survey of 52.38 million hectares integrated with Krishi-DSS; DGCES crop-cutting experiments digitised in 58,994 villages [^11] |
| 23 Oct 2026 | **11 crore Farmer IDs** created, five months ahead of the 31 Mar 2027 deadline; 6 crore+ farmers have received direct benefits through Farmer ID-based service delivery [^1][^4] |

## How It Works

### The Building Blocks

| Component | What it is |
|---|---|
| **Farmer Registry** | The state-run registry of farmers, built on the revenue Records of Rights (RoR). Every enrolled farmer gets a **Farmer ID** — an 11-digit random number generated against Aadhaar, with a digitally verifiable credential. Farmers with land in multiple states get a single ID. [^2][^12][^13] |
| **Land "buckets"** | Before farmers enrol, the Centre's **bucketing tool** groups digitised land parcels by owner — seeding each bucket with Aadhaar using data from PM-KISAN and PMFBY records and the state RoR. A bucket is the digital representation of one landowner's parcel(s) in a village. [^12] |
| **Geo-referenced Village Map Registry** | Village cadastral maps digitised with latitude/longitude — 5.4 lakh of India's ~6.75 lakh villages geo-referenced by mid-2026, with all villages targeted by March 2027. [^5][^11] |
| **Crop Sown Registry** | Created season by season through the mobile-based **Digital Crop Survey (DCS)**: surveyors geo-tag farm plots against the georeferenced maps and record the crop actually sown on each. [^5][^14] |
| **AgriStack Consent Manager (ACM)** | The consent layer through which farmers authorise sharing of their registry data with any external entity — government or private. Sharing happens only against a signed consent artefact. [^2][^12] |
| **UFSI (Unified Farmer Service Interface)** | The open API gateway that lets authorised public- and private-sector apps read registry data — the integration layer that makes AgriStack "the next UPI" in architectural ambition. [^15] |
| **Krishi Decision Support System** | The second pillar of the Mission: integrates satellite, weather, soil, reservoir and groundwater data with scheme data for crop mapping, drought/flood monitoring, and yield-assessment for insurance claims. [^3][^11] |
| **DGCES** | The Digital General Crop Estimation System — digitised crop-cutting experiments for yield estimation (58,994 villages in 2025-26). [^11] |
| **Kisan e-Mitra** | The AI chatbot (launched 21 Sep 2023) for scheme queries and grievances — PM-KISAN, KCC, PMFBY; 11 languages; 93 lakh queries answered as of Dec 2025. [^16][^17] |

### The Farmer Registration Flow

1. **Bucketing**: The Centre's bucketing tool processes the state's digitised land records, groups parcels by owner name and seeds them with Aadhaar (using PM-KISAN/PMFBY data), producing "land buckets" per owner per village. [^12]
2. **eKYC + claim**: The farmer authenticates (Aadhaar biometric/OTP or face authentication) on the state Farmer Registry portal or via a facilitator (CSC/VLE, Krishi Sakhis). Land buckets associated with them are shown automatically; missing plots can be claimed by entering survey/sub-survey numbers. The farmer selects their name on the parcel and signs the claim with **eSign and a consent to be part of AgriStack**. [^12]
3. **Name-match verification**: The software matches the farmer's Aadhaar name against the RoR owner name (and father's/husband's name); low match scores raise rejection risk. State revenue officials approve or reject claims. [^12]
4. **ID issuance**: An Enrolment ID tracks the claim; on approval a **Farmer ID is issued against Aadhaar** — the Farmer Registry application itself does not store Aadhaar numbers; those sit in an encrypted data vault, and the registry stores only the random Farmer ID. [^12]
5. **Crop survey**: Each season, DCS surveyors geo-tag the plot and record the sown crop into the Crop Sown Registry — making the farmer's profile (identity + land + crop) complete. [^5][^14]

The registry **does not confer land ownership**: it dynamically links to the RoR and updates with mutations, but identifies rather than titles. [^13] Its FAQ is explicit that the intent is for the Farmer ID to be used "like Aadhaar for all farmer-related services provided by the Government or by others in the private sector" — e.g., authenticating to a crop-insurance system which auto-populates land and crop data. [^12]

### The Consent Flow

- Data sharing between state registries and any other stakeholder (including the Centre) happens on the **farmer's consent**, exchanged with public/private-key encryption and access tokens issued by the central "network manager". [^12]
- The **AgriStack Consent Manager** issues and logs consent artefacts; sharing with external entities requires explicit farmer consent, and the farmer can log in via eKYC to view their own information. [^12][^2]
- The consent architecture is described by its designers as "blind": the consent manager forwards the signed artefact, after which the data seeker talks to the data provider directly. [^18]

## Key Statistics (with sources)

⚠️ **Reading the numbers:** Farmer ID counts move fast and official snapshots lag; figures below are official government statements at named dates. Where two official counts overlap in time, both are shown.

| Metric | Figure | As of | Source |
|---|---|---|---|
| Farmer IDs generated | 4,85,57,246 (~4.86 crore) | 28 Mar 2025 | PIB / Lok Sabha reply [^9] |
| Farmer IDs | >7.63 crore | early 2026 | PIB [^16] |
| Farmer IDs | >9.20 crore | 19 Mar 2026 | PIB [^10] |
| Farmer IDs | >10.25 crore | 28 Jul 2026 | Rajya Sabha Q.143 statement [^11] |
| Farmer IDs | >10.31 crore | 3 Aug 2026 | Rajya Sabha reply (reported) [^8] |
| Farmer IDs | **11 crore** (target of 11 crore met 5 months early) | night of 23 Oct 2026 | PIB [^1] |
| Farmers receiving direct benefits via Farmer ID | >6 crore | Oct 2026 | PIB [^1] |
| DCS districts — Kharif 2024 | 436 | Mar 2025 | PIB [^9] |
| DCS — Rabi 2024-25 | 461 districts, >23.90 crore plots | Mar 2025 | PIB [^9] |
| DCS — Rabi 2025-26 | 648 districts, >31.3 crore plots | Jul/Aug 2026 | Rajya Sabha statement [^11] |
| Villages geo-referenced | 5.4 lakh of ~6.75 lakh (~80%) | Aug 2026 | Indian Express (government data) [^5] |
| Soil survey (SLUSI, 1:10,000 envisaged for ~142 M ha) | 52.38 million ha mapped | Jun 2026 | Rajya Sabha statement [^11] |
| Digitised crop-cutting experiments (DGCES) | 58,994 villages | 2025-26 | Rajya Sabha statement [^11] |
| Mission outlay | ₹2,817 crore (central share ₹1,940 crore) | approved 2 Sep 2024 | PIB [^3] |
| Maharashtra: disaster relief disbursed using Farmer IDs | >₹14,000 crore to 89 lakh farmers (Kharif 2025 crop losses, ~5 days) | Jul 2026 | Rajya Sabha statement [^11] |
| Chhattisgarh: MSP paddy procurement on Farmer ID + DCS | >32 lakh farmers in a single season | Jul 2026 | Rajya Sabha statement [^11] |
| Kisan e-Mitra chatbot | >93 lakh queries answered; >8,000/day, 11 languages | Dec 2025 | PIB [^16] |
| State-level comparison | Madhya Pradesh 1.04 crore IDs; Maharashtra 1.31 crore IDs (largest) | 19 Mar 2026 | PIB [^10] |

**Context for the 11 crore:** India's last completed Agriculture Census (2015-16) counted **146.45 million (≈14.65 crore) operational land holdings**, and the 2011 Census counted ~11.8 crore cultivators against ~14.4 crore agricultural labourers. [^19] The 11-crore ID target therefore approximates the universe of *landholding* farmer families — not all who cultivate. See the Citizen Rights analysis below for why that gap matters.

## Layers Classification (L1–L7)

Based on the IndiaStack Layers framework, AgriStack occupies the following positions:

| Layer | Classification | AgriStack's Role |
|---|---|---|
| **L1 — Vision & Policy** | Government policy | Budget 2023-24 DPI-for-agriculture announcement; Digital Agriculture Mission approved 2 Sep 2024; "Minimum Government, Maximum Governance" framing for the Farmer Registry [^3][^1] |
| **L2 — Regulation** | Regulatory framework | Operational Guidelines (Sep 2024) and scheme guidelines — administrative instruments, **no dedicated AgriStack statute**; the DPDP Act 2023 + DPDP Rules 2025 are the data-protection overlay; Aadhaar Regulations govern the eKYC/vault layer; state revenue law (RoR, mutation) remains the legal substrate for land [^3][^20] |
| **L3 — Digital Rails** | Core infrastructure | Farmer Registry + land buckets, Geo-referenced Village Map Registry, Crop Sown Registry, the AgriStack Consent Manager, central core (Farmer ID generation, network manager, data vault) [^2][^12] |
| **L4 — APIs & Protocols** | Open standards | **UFSI** open API gateway, token-based authenticated data exchange, IndEA 2.0 (India Digital Ecosystem Architecture) standards — the Farmer ID is a "functional ID based on Aadhaar as per IndEA 2.0" [^13][^15][^12] |
| **L5 — Applications** | End-user apps | State Farmer Registry portals and farmer-facing apps (e.g. `mhfr.agristack.gov.in`, `upfr.agristack.gov.in`), facilitator tools for CSCs/Krishi Sakhis, DCS surveyor apps, Kisan e-Mitra chatbot [^12][^16] |
| **L6 — Use Cases** | Sectoral applications | PM-KISAN delivery, Kisan Credit Card, PMFBY crop insurance, MSP procurement (Chhattisgarh), disaster relief (Maharashtra), input (urea/DAP) distribution controls, AI advisory, UPAg, Bharat Pashudhan, National Fisheries Digital Platform integrations [^11] |
| **L7 — Analytics & Intelligence** | Data & insights | Krishi-DSS (crop maps, drought/flood monitoring, yield assessment), DGCES production estimates, NPSS pest advisories (66 crops, 432+ pest types, 10,000+ extension workers), soil mapping — and government positioning of AgriStack data as a foundation for "AI Kosh" and agri-tech AI [^11][^16] |

AgriStack is best read as an **L3–L4 construct** — state-owned registries and open APIs onto which schemes, banks, insurers and agri-techs plug in. Its distinctiveness among India's DPIs is that the data layer is built on the country's most contested records: land.

## Regulatory Framework

### The core problem: policy, not law

AgriStack has no statute of its own. It is implemented through the Digital Agriculture Mission's administrative sanction, Operational Guidelines issued to states, and MoUs between the Ministry and state governments. [^3][^8] Data governance therefore rests on:

- **The DPDP Act, 2023 and DPDP Rules, 2025** — farmers are Data Principals and the state agencies running registries are Data Fiduciaries. The government's Rajya Sabha statement asserts AgriStack was built "in accordance with the DPDP Act, 2023 and the DPDP Rules 2025" with consent-based collection, encryption and MeitY/CERT-In-compliant security. [^20][^11] The DPDP framework, however, is a general-purpose law: it gives farm data no special status, and compliance is asserted, not independently audited. [^21]
- **Aadhaar Regulations** — Farmer registration uses Aadhaar eKYC; Aadhaar numbers are held in encrypted data vaults per UIDAI-style practice, with registries storing only the random Farmer ID. [^12][^13]
- **State revenue law** — the RoR/mutation system remains the legal foundation; the registry inherits its errors. Indian courts have long held that land records are fiscal documents carrying, at most, a rebuttable presumption — not titles (*Suraj Bhan*; *Sawarni v. Inder Kaur*). [^21]
- **Sectoral scheme rules** — PM-KISAN, PMFBY and KCC guidelines determine how Farmer ID data flows into credit, insurance and income support.

### The consent architecture — and its critique

On paper, the ACM model is strong: explicit, signed consent artefacts, purpose-bound sharing, blind intermediation, and farmer self-service access to their own records. [^12][^18] The critique runs deeper than mechanics: legal commentators argue AgriStack has a **structural consent deficit** — enrollment itself vacuums land, crop and benefit data into the registries, and the farmer's meaningful choice is at the point of sharing, after the data exists and scheme access is conditioned on being registered; commentators argue AgriStack's custodians should be notified as **Significant Data Fiduciaries** under Section 10 of the DPDP Act (which would mandate India-based data protection officers, independent audits and periodic impact assessments). [^21] Critics also flag that much of AgriStack's value — aggregate crop, land and yield data — risks classification as **non-personal data**, a category India's framework treats with lesser protections. [^22]

## Citizen Rights Analysis

### Rights on paper

- **Enrollment with consent**: the farmer signs a consent to join AgriStack (with eSign) as part of the bucket claim. [^12]
- **Data stays with the states**: the registry is federated — "ownership of the data is with the respective States". [^11]
- **No external sharing without consent**: farmer–land linkages are not shared with external entities without explicit, eSign-backed consent; farmers can view their own records via eKYC login. [^12]
- **No title conferred**: the registry "solely identifies farmers" and does not create or extinguish land rights. [^13]
- **Coverage ambition**: the registry is designed to onboard not just landowners but also **cultivators such as tenants and sharecroppers**, and states are taking steps "in accordance with applicable rules" to bring actual cultivators onto the platform. [^10][^1]

### Rights in practice — where the paper and the queue diverge

1. **The tenant-farmer exclusion problem is structural.** The registry is built on RoR — records of *owners*. Oral tenancies and sharecropping arrangements appear in no register, and land records are riddled with unmutated inheritances and stale entries. [^21] Since the ID is "allocated in favour of the land owner to start with", the cultivator who actually farms the plot starts outside the system; the FAQ's own answer is that non-RoR cultivators can be allotted IDs later "in case of death or dispute pending updating in RoR" — a thin reed for a population that, in major agricultural states, constitutes 30–40% of the active farm workforce. [^12][^23] Commentators argue this constructs **wrongful exclusion into the system**, engaging Article 14 (a manifestly arbitrary classification between recorded owners and unrecorded cultivators) and Article 21 (livelihood and dignity) — the same exclusion concern the Supreme Court registered in the Aadhaar judgment, at larger scale and on a less reliable foundational dataset. [^21]
2. **De-facto conditionality.** Farmer ID-based delivery is rapidly becoming the default channel for schemes: Chhattisgarh has institutionalised it for MSP procurement; Maharashtra for disaster relief and credit access; and PM-KISAN linkage to AgriStack has caused payment disruptions while states clean up land records — with farmers caught in eKYC and name-match failures seeing installments silently stop. [^11][^23] As with ABDM and Aadhaar, a nominally voluntary identity becomes functionally mandatory at the point of need. [^21]
3. **Verification is the state's certainty, not the farmer's.** Name-match scoring between Aadhaar and RoR names determines whether a farmer's claim succeeds; common-name collisions and low match scores produce rejections that the farmer must then fix through the grievance system and the patwari. The burden of legacy record-keeping errors lands on the data subject. [^12]

## Privacy Implications

- **A comprehensive profile by design.** AgriStack deliberately integrates identity, land, crop, assets (livestock, fisheries) and benefits availed into one profile per farmer — the exact dataset banks, insurers, input suppliers and agri-techs need for credit-scoring, risk-pricing and marketing. [^1][^11] The UFSI API gateway makes that profile programmatically reachable by authorised private parties. [^15]
- **Aadhaar linkage at the core.** The Farmer ID is generated against Aadhaar and Aadhaar seeding of land buckets uses PM-KISAN/PMFBY data; while applications store only the Farmer ID, the linkage lattice is Aadhaar-based end to end. [^12][^13]
- **Weaker safeguards than Aadhaar's.** The IDEA-era criticism — that farm data would flow to private firms without Aadhaar-grade statutory protection — has largely carried over to AgriStack: the DPDP Act gives agricultural data no special category status, and aggregate farm data risks falling into the lesser-protected non-personal bucket. [^7][^22]
- **Surveillance and profiling risk.** Plot-level crop data every season, combined with subsidy, insurance and credit trails, enables fine-grained monitoring of rural households; IT for Change and others argue the collective interests of farming communities are not reducible to individual consent, and that "data is relational" — a framing that individual consent artefacts cannot capture. [^24]
- **Breach blast radius.** Identity + land records + benefit flows in one linked lattice is a high-value target; without an independent audit regime (SDF status) or a dedicated statute, liability for a breach rests on general DPDP provisions. [^21][^22]

## Safeguards

What exists, as claimed by official sources:

- **Federated, state-owned data** — registries created and maintained by states; central core generates IDs and tokens but the data resides in state servers. [^11][^12]
- **Aadhaar not stored in the application** — encrypted data vaults hold Aadhaar; registries store only the 11-digit random Farmer ID. [^12]
- **Consent-gated external sharing** — explicit eSign-backed consent via the ACM; encrypted exchange with public/private keys and token-based access. [^12][^11]
- **No title effects** — the registry identifies but does not confer ownership; corrections follow the mutation process. [^13]
- **DPDP compliance asserted** — government statements assert alignment with the DPDP Act/Rules, MeitY cybersecurity guidelines and CERT-In directions. [^11][^20]
- **Grievance machinery in the registry** — an in-app grievance module with ticketing, helpdesks, and target turnaround for claim disputes. [^12]

What is missing or unverified: independent data audits and DPIAs (no SDF notification), a statutory basis for the registries, published breach disclosures, and an accessible route for tenant cultivators that does not depend on the same RoR machinery that excludes them. These are flagged as open concerns, not established failures. [^21]

## Complaints & Grievance Redressal

| Channel | Details |
|---|---|
| **Farmer Registry grievance module** | Every state registry application has an in-app grievance-raising module; the farmer files a grievance and receives a number. Bucket-claim disputes are expected to be resolved within ~10–15 days via state revenue officials (patwari-level corrections). [^12] |
| **State/district helpdesks** | Registration and claim issues route to state helpdesks, which resolve or escalate to the AgriStack team — e.g. Maharashtra helpdesk 020 25712712; Odisha Krushi Samrudhi toll-free 155333. [^12][^25][^26] |
| **Kisan e-Mitra (AI chatbot)** | Voice-enabled chatbot for PM-KISAN, KCC and PMFBY queries and grievances; 11 languages; >8,000 queries/day; >93 lakh queries answered as of Dec 2025. Built with Wadhwani AI as the Ministry's grievance-redressal chatbot, launched 21 Sep 2023. [^16][^17][^27] |
| **Kisan Call Centre** | Toll-free 1800-180-1551 (also 1551), 6 AM–10 PM all days, in 22 local languages — the long-standing Ministry helpline since 2004. [^28] |
| **PM-KISAN grievance system** | Scheme-level grievance module on the PM-KISAN portal for payment/eKYC failures — the most common failure mode in Farmer ID-linked delivery. [^23] |
| **DPDP Act remedies** | As Data Principals, farmers can complain to the registered Data Fiduciary (state registry agency) and, for unresolved breaches, to the Data Protection Board under the DPDP Act 2023. [^20] |
| **CPGRAMS** | The central public-grievance portal remains the fallback for systemic complaints against state agriculture departments. |

## Prime References

[^1]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2327905 — PIB, Ministry of Agriculture & Farmers Welfare, "11 Crore Farmer IDs Created Five Months Ahead of Schedule", 24 Oct 2026
[^2]: https://agristack.gov.in — AgriStack official portal (Ministry of Agriculture & Farmers Welfare)
[^3]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2051719 — PIB, "Digital Agriculture Mission: Tech for Transforming Farmers' Lives" (Cabinet approval, outlay, components, targets, pilots), 4 Sep 2024
[^4]: https://www.drishtiias.com/daily-updates/daily-news-analysis/india-achieves-11-crore-farmer-ids-under-digital-agriculture-mission — Drishti IAS, "India Achieves 11 Crore Farmer IDs", 27 Oct 2026 (independent confirmation of date and deadline)
[^5]: https://indianexpress.com/article/explained/agristack-sitharaman-next-upi-10528472 — The Indian Express Explained: "The 'next UPI': What is AgriStack?" (registry components, DCS targets, village-map coverage)
[^6]: https://csd.columbia.edu/sites/default/files/content/docs/ICT%20India/Papers/ICT_India_Working_Paper_68.pdf — Columbia University ICT India Working Paper #68, "India Digital Ecosystem of Agriculture and Agristack: An Initial Assessment" (IDEA history and concerns)
[^7]: https://www.reuters.com/legal/litigation/indias-digital-database-farmers-stirs-fears-about-privacy-exclusion-2021-06-24 — Reuters, "India's digital database for farmers stirs fears about privacy, exclusion", 24 Jun 2021
[^8]: https://vassarlabs.com/agristack-vs-state-agri-dpi-untangling-indias-national-and-state-digital-agriculture-layers — Vassar Labs, "AgriStack vs State Agri-DPI" (Rajya Sabha data cross-check; operational guidelines date)
[^9]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2117390 — PIB, "Digital Identities to Farmers" (4.86 crore IDs; DCS district/plot counts), 1 Apr 2025
[^10]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2244626 — PIB, "AgriStack's Farmers Registry Crosses 9.20 Crore Farmer IDs Nationwide" (tenant/sharecropper onboarding provision; state-wise table), 24 Mar 2026
[^11]: https://sansad.in/getFile/annex/271/AS143_IyRN0d.pdf?source=pqars — Rajya Sabha Starred Question 143, "Rollout of AgriStack and Digital Agriculture Mission", statement due 31 Jul 2026 (federated ownership, DPDP/CERT-In compliance claims, Maharashtra/Chhattisgarh deployments, DGCES, soil survey)
[^12]: https://agristack.gov.in/assets/registries/farmerRegistry/farmer_registry_faqs.pdf — AgriStack Farmer Registry FAQs (bucketing, Aadhaar vault, consent, name-match, grievance mechanism)
[^13]: https://www.microsave.net/2025/11/12/agristack-a-dpi-approach-to-transform-indian-agriculture — MSC, "AgriStack: A DPI Approach to Transform Indian Agriculture", 12 Nov 2025 (IndEA 2.0 functional ID, data vault, no-title principle)
[^14]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2296209 — PIB, "Implementation of AgriStack and Digital Agriculture Mission" (DCS 648 districts/31.3 crore plots Rabi 2025-26), 7 Aug 2026
[^15]: https://issca.icrisat.org/scalable-solutions/digital-public-infrastructure-for-agriculture-agristack — ICRISAT ISSCA, "Digital Public Infrastructure for Agriculture – AgriStack" (UFSI, Consent Manager, registry architecture)
[^16]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2227914&reg=48&lang=2 — PIB, "7.63 crore Farmer IDs; NPSS; Kisan e-Mitra 93 lakh queries", (Dec 2025 data release)
[^17]: https://apolitical.co/navigator/case-studies/kisan-e-mitra-indias-voice-enabled-ai-support-for-farmers — Apolitical case study: "Kisan e-Mitra: India's voice-enabled AI support for farmers" (launch 21 Sep 2023, query volumes)
[^18]: https://www.linkedin.com/posts/rajeev-chawla-ias_162a301b_while-dpdp-act-defines-what-is-personal-data-activity-7510926175142146048-SAXr — Rajeev Chawla IAS (AgriStack architect), description of the blind AgriStack Consent Manager
[^19]: https://agcensus.da.gov.in/acindiamethod.html — Agriculture Census of India (operational holdings methodology; 14.65 crore holdings per All-India Report 2015-16)
[^20]: https://www.meity.gov.in/data-protection-framework — MeitY, Digital Personal Data Protection Act 2023 and DPDP Rules 2025
[^21]: https://www.livelaw.in/articles/farmer-data-point-agristack-consent-deficit-dpdp-act-555490 — LiveLaw, "Farmer As Data Point: AgriStack's Consent Deficit And DPDP Act" (SDF argument, Article 14/21 exclusion analysis, land-records-not-titles)
[^22]: https://ohrh.law.ox.ac.uk/the-digitisation-of-agriculture-in-india-how-agristack-infringes-informational-privacy — Oxford Human Rights Hub, "The Digitisation of Agriculture in India: How AgriStack Infringes Informational Privacy" (Puttaswamy, NPD lesser-protection concern)
[^23]: https://www.impriindia.com/insights/policy-update/a-relook-at-the-pm-kisan-2018-scheme — IMPRI, "A Relook at the PM-KISAN" (eKYC exclusion, AgriStack linkage disruptions, tenant/labourer exclusion estimates)
[^24]: https://itforchange.net/sites/default/files/add/ITFC_The%20Digital%20Ecosystem%20Opportunity%20for%20Indian%20Agriculture_.pdf — IT for Change, "The Digital Ecosystem Opportunity for Indian Agriculture" (collective/relational data critique)
[^25]: https://mhfr.agristack.gov.in — Maharashtra Farmer Registry portal (state helpdesk number)
[^26]: https://odfr.agristack.gov.in — Odisha Farmer Registry portal (Krushi Samrudhi helpline 155333)
[^27]: https://www.wadhwaniai.org/empowering-millions-of-indian-farmers-with-instant-ai-chatbot-support — Wadhwani AI, Kisan e-Mitra grievance-redressal chatbot partnership
[^28]: https://agriwelfare.gov.in/sites/default/files/KCC%20WEBSITE.pdf — Department of Agriculture & Farmers Welfare, Kisan Call Centre (1800-180-1551)
