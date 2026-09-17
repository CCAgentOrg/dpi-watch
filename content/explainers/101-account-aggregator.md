---
title: "Account Aggregator 101: India's Consent Layer for Financial Data"
description: "A comprehensive guide to India's Account Aggregator (AA) framework — the RBI-regulated, consent-based system for sharing financial data, its DEPA origins, the 2025 regulatory overhaul, ecosystem statistics, citizen rights, privacy safeguards, and grievance routes."
date: 2026-09-17
draft: false
tags: ["account-aggregator", "aa", "rbi", "sahamati", "depa", "consent", "open-finance", "dpi", "financial-data", "data-protection", "india"]
categories: ["DPI Basics"]
image: "/images/account-aggregator-101-cover.jpg"
author: "CashlessConsumer"
readingTime: "16 min"
---

# Account Aggregator 101: India's Consent Layer for Financial Data

## What is the Account Aggregator Framework?

The **Account Aggregator (AA) framework** is a Reserve Bank of India (RBI)-regulated, consent-based system that enables individuals and businesses to share their financial data between regulated financial institutions. Account Aggregators are a special class of non-banking financial company — **NBFC-Account Aggregators (NBFC-AA)** — that retrieve, collect, consolidate and present a customer's financial information to the customer or to a regulated **Financial Information User**, based entirely on the customer's explicit, granular, time-bound and revocable consent. Under the governing Directions, the financial information "shall not be the property of the Account Aggregator, and not be used in any other manner." [^1]

The framework is the financial sector's implementation of the **Data Empowerment and Protection Architecture (DEPA)**, published as a draft by **NITI Aayog in August 2020** as a "secure consent-based data sharing framework to accelerate financial inclusion." [^2] Sahamati, the industry alliance behind the ecosystem, describes AA as "the UPI of financial information" — if UPI moved money between any two bank accounts, AA moves verified financial data between any two regulated institutions. [^3]

The regulatory foundation dates to **September 2016**, when RBI first issued Master Directions for NBFC-Account Aggregators; the framework went live for customers on **2 September 2021**, when eight major banks joined the network. [^4][^5] On **28 November 2025**, RBI issued a consolidated **Reserve Bank of India (Non-Banking Financial Companies – Account Aggregator) Directions, 2025**, repealing and replacing the 2016 Master Directions as part of its NBFC regulatory overhaul. [^1] On **5 June 2026**, RBI recognised **Sahamati Foundation** as the **Self-Regulatory Organisation (SRO-AA)** for the ecosystem. [^6]

### Historical Context

| Date | Milestone |
|---|---|
| Sep 2016 | RBI issues Master Directions for NBFC-Account Aggregators [^4] |
| 2019 | First in-principle AA licences granted; closed-user-group testing begins |
| Aug 2020 | NITI Aayog publishes DEPA draft for discussion [^2] |
| 2 Sep 2021 | AA framework goes live with eight banks [^4][^5] |
| Oct 2021 | Scale-Based Regulation places NBFC-AAs in the Base Layer [^7] |
| 19 Aug 2022 | SEBI circular enables depositories and AMCs as Financial Information Providers [^8] |
| 23 Nov 2022 | RBI includes GSTN as a Financial Information Provider (tax data enters the network) [^9] |
| 2022–2024 | PFRDA designates NPS CRAs as FIPs and PoPs as FIUs; CCIL added for Retail Direct Gilt accounts [^10][^7] |
| 2023 | Digital Personal Data Protection (DPDP) Act enacted, embedding a "Consent Manager" modelled on the AA [^11] |
| 12 Mar 2025 | RBI invites applications and issues the Framework for recognising an SRO for the AA ecosystem [^12] |
| 28 Nov 2025 | RBI (NBFC – Account Aggregator) Directions, 2025 consolidate and replace the 2016 Master Directions [^1] |
| 5 Jun 2026 | RBI recognises Sahamati Foundation as SRO-AA [^6] |
| 2 Sep 2026 | Ecosystem crosses 500 million fulfilled consents on the 5th AA Foundation Day [^13] |

## How It Works

### The Three Participants

| Role | What it does | Examples |
|------|--------------|----------|
| **Account Aggregator (AA)** | RBI-licensed NBFC that manages consent and ferries encrypted data between institutions. Cannot store, read, use or own the data; cannot lend or accept deposits. | Finvu, OneMoney, Anumati (Perfios), CAMSfinserv, Protean SurakshAA, NeSL-AA, Setu, TallyEdge, Saafe, NADL [^14][^15] |
| **Financial Information Provider (FIP)** | Regulated entity holding the customer's data; releases it only against a valid consent artefact. Defined in the 2025 Directions to include banks, NBFCs, AMCs, depositories, depository participants, insurers, insurance repositories, Central Recordkeeping Agencies, GSTN and CCIL. | Banks, insurers, mutual fund RTAs, depositories (CDSL/NSDL), NPS CRAs, GSTN [^1] |
| **Financial Information User (FIU)** | Regulated entity that requests data to deliver a service. Any entity "registered with and regulated by any financial sector regulator" qualifies. | Banks, NBFC lenders, stockbrokers, RIAs, insurers, pension funds [^1] |

Sahamati operates the **Central Registry** of ecosystem participants, runs certification of AAs/FIPs/FIUs, and since June 2026 doubles as the RBI-recognised SRO. [^6][^16]

### The Consent-Artefact Data Flow

1. **Link** — the customer registers with an AA app of their choice and links their accounts with each FIP, authenticating directly with the FIP. The AA never sees the customer's banking credentials. [^15]
2. **Request** — an FIU raises a digitally signed **consent request** specifying the data sought, the purpose, the duration, the exact accounts, and an expiry date. Standardised **purpose codes** defined by ReBIT (RBI's tech subsidiary) constrain what the data can be used for. [^17][^18]
3. **Approve or reject** — the customer approves or declines in the AA app. Consent is granular (data type, date range, frequency, expiry) and **revocable** at any time. [^19]
4. **Fetch** — on approval, the AA presents the consent artefact to the FIP, which verifies it, digitally signs the financial data and transmits it **end-to-end encrypted**. The AA routes the encrypted payload without holding a decryption key — it is "data-blind." [^15]
5. **Use** — the FIU decrypts and uses the data strictly for the consented purpose (e.g., loan underwriting). The AA deletes the ephemeral payload after delivery. [^19]

RBI's **reciprocity principle** requires RBI-regulated entities joining as FIUs to also come on board as FIPs where they hold the relevant data — preventing free-riding on the network. [^10]

### What Data Can Move

The 2025 Directions enumerate the permitted categories of "financial information": bank deposits (savings, current, fixed, recurring), NBFC deposits, structured investment products, commercial paper, certificates of deposit, government securities, equity shares, bonds, debentures, mutual fund units, ETFs, Indian Depository Receipts, CIS and AIF units, insurance policies, National Pension System balances, InvIT and REIT units, and **GST returns (GSTR-1 and GSTR-3B)** — with RBI empowered to add more. [^1] RBI-regulated FIUs must first join as FIPs under the reciprocity rule. [^10]

## Key Statistics

*(Figures as of the latest verifiable official reporting — September 2026.)*

| Metric | Value | As of |
|---|---|---|
| Cumulative fulfilled consents | **500+ million** [^13] | 2 Sep 2026 |
| Cumulative consents delivered / data fetches | 45 crore+ consents; 500 crore+ data fetches [^20] | FY26 |
| Financial products/services enabled in FY26 | ~3.8 crore [^20] | FY26 |
| Consents processed daily | 7 lakh+ [^20] | 2026 |
| Personal Finance Management (PFM) users | 5.96 crore (164% CAGR since FY23) [^20] | FY26 |
| Credit facilitated | **₹3.82 lakh crore** across 3.68 crore loans in FY26; 624% growth in home loans/loan-against-property [^21] | FY26 |
| Live regulated entities on network | 1,120 (1,020 FIUs, 176 FIPs) [^22] | Jun 2026 |
| Operational AAs | 17 licensed/operational (8 consumer-facing apps listed by Sahamati) [^22][^14] | 2026 |
| Linked accounts | 294+ million [^22] | Jun 2026 |
| Monthly data shares | 290–295 million [^22][^23] | Jun 2026 |
| FIP composition | 72 banks, 57 insurers, 2 depositories, 2 RTAs, 3 NPS CRAs, GSTN, 6 NBFCs, 40 AMCs via RTAs [^7] | Mar 2026 |
| F&O accounts verified via AA in FY26 | ~67.65 lakh; 70–80% of income verification at leading brokers runs on AA [^20] | FY26 |
| Life insurance policies issued using AA | ~1.51 lakh [^20] | FY26 |

**⚠️ Conflicting figures — read with care:** Sahamati's own dashboard distinguishes consents **raised** (≈1.97 billion) from consent requests **fulfilled** (≈493 million, June 2026) [^23] — a conversion rate of roughly one in four. The gap between consent raised and consent delivered, driven by abandoned journeys and failed linking, is the ecosystem's most contested internal number and predates the current milestone headlines. [^15][^23] Separately, "users" claims vary: the 5.96 crore figure counts users of AA-powered PFM experiences inside FIU apps, not registered AA-app users. [^20]

## Layers Classification (L1-L7)

| Layer | Classification | The AA Framework's Role |
|---|---|---|
| **L1 — Vision & Policy** | Government policy | NITI Aayog's DEPA (2020); financial-inclusion mandate; Ministry of Finance launch advocacy [^2][^4] |
| **L2 — Regulation** | Regulatory framework | RBI (NBFC-AA) Directions 2025 under s.45JA, RBI Act 1934; SRO-AA framework (Mar 2025); SEBI/IRDAI/PFRDA participation circulars; DPDP Act 2023 [^1][^12][^8][^11] |
| **L3 — Digital Rails** | Core infrastructure | The AA switching network itself — consent routing and encrypted data transport between 1,100+ regulated entities [^22] |
| **L4 — APIs & Protocols** | Open standards | ReBIT API specifications; consent artefact standard; purpose codes; Sahamati fair-use consent templates [^17][^18][^19] |
| **L5 — Applications** | End-user apps | Consumer AA apps (Finvu, OneMoney, Anumati, CAMSfinserv, Saafe, NADL, Protean SurakshAA) plus FIU-side journeys inside lender/broker/insurer apps [^14] |
| **L6 — Use Cases** | Sectoral applications | Loan underwriting, account aggregation/PFM, investment portfolio import, F&O income proof, insurance underwriting, GST/MSME lending, collections monitoring [^20][^21] |
| **L7 — Analytics & Intelligence** | Data & insights | Ecosystem metrics via Sahamati dashboards (aggregate, anonymised); FIU-side analytics on consented data; SLA/health monitoring (Saans) [^24] |

The AA framework is an **L3-L4 construct**, like UPI: the public-good core is the consent-and-switching layer, while all user experience sits with licensed private apps and regulated FIUs. It is also the **template for a new L2 category** — the DPDP Act's "Consent Manager" is modelled directly on the AA. [^11]

## Regulatory Framework

**Primary regulation.** The RBI (NBFC – Account Aggregator) Directions, 2025 (RBI/DoR/2025-26/368, dated 28 November 2025), issued under section 45JA of the RBI Act, 1934, govern registration, scope, governance and conduct of NBFC-AAs. Key provisions: [^1]

- Only a **company** with RBI's certificate of registration may do AA business; **net owned fund of at least ₹2 crore**; application via the PRAVAAH portal; fit-and-proper promoters; a robust IT plan; **leverage ratio capped at 7**; in-principle approval valid 12 months. [^1]
- NBFC-AAs **always remain in the Base Layer** of RBI's Scale-Based Regulation, but specified governance paragraphs of the NBFC Governance Directions apply regardless. [^1]
- Board-approved policies are mandatory for **grievance handling, pricing of services, and director fit-and-proper criteria**. [^1]
- The 2016 Master Directions stand repealed and replaced. [^1]

**Sectoral participation.** SEBI's circular of 19 August 2022 brought depositories and AMCs onto the network as FIPs; [^8] RBI added GSTN as an FIP on 23 November 2022; [^9] PFRDA circulars designated NPS CRAs as FIPs and Points of Presence as FIUs. [^10] The 2025 Directions also exempt entities regulated by other financial sector regulators that aggregate only their own sector's customers from RBI AA registration. [^1]

**Self-regulation.** Under RBI's SRO-AA Framework (12 March 2025), the Reserve Bank recognised **Sahamati Foundation** as the ecosystem's SRO on 5 June 2026 — the first formal industry-governance layer for AA, covering conduct standards, member oversight and grievance escalations. [^12][^6]

**Data protection law.** The DPDP Act, 2023 (sections 6(7)–6(9)) creates a registered **Consent Manager** — explicitly modelled on the AA — with operational details in Rule 4 of the DPDP Rules, 2025. Consent Manager registration with the Data Protection Board opens **13 November 2026** (₹2 crore net worth requirement), and penalties reach ₹250 crore for data fiduciaries and ₹50 crore for Consent Managers. [^11][^25][^26] The **overlap between RBI's AAs and the DPB's Consent Managers is formally unresolved** — the Data Protection Board had not been constituted as of mid-2026, and whether existing AAs will be deemed sector-specific Consent Managers remains an open policy question, with potential for parallel enforcement by two regulators. [^27][^28]

## Citizen Rights Analysis

The AA framework confers concrete, enforceable rights on citizens — and one important caveat:

- **Right to granular consent.** Every data request must specify purpose, data types, duration and expiry, and the citizen approves it explicitly. Standardised purpose codes and Sahamati's fair-use consent templates constrain open-ended requests like "share everything." [^17][^19]
- **Right to refuse and revoke.** Consent can be declined or withdrawn at any time; the FIU must stop new fetches on revocation. [^19]
- **Right to data blindness.** The AA cannot read, store, sell or claim ownership of your data — written into the licence conditions themselves. [^1][^15]
- **Right to regulated recipients.** Only entities regulated by a financial sector regulator can receive data as FIUs — unlicensed fintechs must route through regulated partners. [^1][^7]
- **Right to redress.** Board-mandated grievance policies at every AA, RBI Ombudsman escalation, and — prospectively — DPDP Board remedies. (See Complaints section.)
- **⚠️ The consent-gap caveat.** A right on paper is only as good as its exercise: Sahamati's own counters show roughly three-quarters of raised consents are never fulfilled — meaning journeys frequently fail after the citizen has done their part. The citizen's control is real, but so is the friction. [^23][^15]
- **⚠️ Power asymmetry in practice.** Consent screens appear inside FIU journeys (a loan application, a KYC flow), where refusal can mean losing the service. Voluntariness under those conditions is thinner than the architecture implies — a structural critique civil society has raised about consent-based regimes generally. [^11][^27]

## Privacy Implications

- **End-to-end encryption, data-blind switch.** FIPs encrypt data for the FIU's key; AAs relay ciphertext they cannot decrypt and hold no decryption keys. [^15]
- **No storage by design.** AAs are prohibited from retaining customer data; the 2025 Directions make clear the data is never the AA's property. [^1]
- **But the FIU sees everything consented.** Once delivered, data protection depends on the FIU's retention discipline and purpose-limitation compliance — the AA network cannot audit what an FIU does with data after delivery. Post-delivery enforcement is the framework's weakest audit point. [^27]
- **Full financial profile concentration.** As coverage grows across banks, investments, insurance, pensions and GST, a single consent can assemble a near-complete financial dossier. That is the product feature — and the risk. [^1][^20]
- **Consent fatigue and dark patterns.** Consent requested mid-journey, pre-ticked flows or bundled purposes can hollow out genuine choice; standardised templates mitigate but do not eliminate this. [^19][^17]
- **Regime transition uncertainty.** Until the DPDP Consent Manager regime and the RBI AA framework are harmonised, citizens' privacy remedies sit across two regulators with no settled interplay — including potential duplicate proceedings for the same violation. [^27][^28]
- **Self-regulation capture risk.** The ecosystem's SRO is an industry alliance funded by its members (₹50 crore raised from 25+ institutions in April 2026) — pace-of-oversight questions apply wherever the regulator delegates conduct supervision to the regulated. [^29][^6]

## Safeguards

- **Licensing and capital.** RBI-issued Certificate of Registration, ₹2 crore minimum net owned fund, fit-and-proper promoters, leverage cap, Board-level governance committees. [^1]
- **Data-blind architecture.** AAs cannot store, decrypt or own data; cryptographic signing by FIPs guarantees authenticity; end-to-end encryption in transit. [^1][^15]
- **Standardised consent.** ReBIT purpose codes and Sahamati's fair-use template library cap how broadly FIUs can request data. [^17][^19]
- **Certification and registry.** Sahamati's Central Registry and participant certification keep unverified entities off the network; health/SLA dashboards (Saans) expose FIP uptime publicly. [^16][^24]
- **SRO oversight.** Conduct standards, member code of conduct and grievance escalation under RBI-recognised SRO-AA from June 2026. [^6]
- **Ombudsman backstop.** Unresolved service deficiencies can reach the RBI Ombudsman under the Integrated Ombudsman Scheme, 2021. [^30]
- **DPDP penalties (prospective).** Once the Consent Manager regime is operational, violations carry penalties up to ₹250 crore (fiduciaries) / ₹50 crore (Consent Managers), with full enforcement timelines running to May 2027. [^26][^28]

## Complaints & Grievance Redressal

1. **Complain to the AA first.** Every NBFC-AA must maintain a Board-approved customer-grievance policy; raise the issue through the AA app or its customer support with the consent reference ID. [^1]
2. **Escalate to the RBI Ombudsman.** Under the Reserve Bank–Integrated Ombudsman Scheme, 2021 (effective 12 November 2021), if the AA (or FIU/FIP) rejects your complaint or does not reply within 30 days — or you are dissatisfied with the resolution — file free of cost at the RBI's complaint portal (cms.rbi.org.in), via email to the Centralised Receipt and Processing Centre (CRPC, Chandigarh), or by calling 14448. Appeal against an Award lies with RBI's Appellate Authority. [^30]
3. **SRO escalation.** As RBI-recognised SRO since June 2026, Sahamati operates grievance dashboards and can take up participant-conduct complaints; its Saans dashboard also exposes which FIPs are failing consent fulfilment SLAs — useful evidence when a bank keeps stalling your consent. [^6][^24]
4. **DPDP remedies (prospective).** Once the Data Protection Board is functional and the Consent Manager regime activates, privacy-specific complaints — including against consent misuse — will have a dedicated tribunal path with significant penalty power. [^26][^28]

## Prime References

[^1]: https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=12936
[^2]: https://niti.gov.in/sites/default/files/2020-09/DEPA-Book_0.pdf
[^3]: https://medium.com/digital-banking-2030/how-sahamatis-account-aggregator-model-is-redefining-financial-data-ownership-in-india-941b4a931dc9
[^4]: https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=10598
[^5]: https://www.medianama.com/2021/09/223-account-aggregator-ecosystem-launch
[^6]: https://rbi.org.in/Scripts/BS_PressReleaseDisplay.aspx?prid=62870
[^7]: https://casparser.in/blog/state-of-account-aggregator-2026
[^8]: https://www.sebi.gov.in/legal/circulars/aug-2022/participation-as-financial-information-providers-in-account-aggregator-framework_62157.html
[^9]: https://www.pib.gov.in/Pressreleaseshare.aspx?PRID=1882868
[^10]: https://sahamati.org.in/faq
[^11]: https://sahamati.org.in/reconciling-the-account-aggregator-and-consent-manager-frameworks
[^12]: https://www.rbi.org.in/Scripts/BS_PressReleaseDisplay.aspx?prid=59956
[^13]: https://sahamati.org.in/media-article/account-aggregator-crosses-500-million-consents-as-india-marks-5th-aa-foundation-day
[^14]: https://sahamati.org.in/aa-apps/
[^15]: https://sahamati.org.in/what-is-account-aggregator/
[^16]: https://sahamati.org.in/certification/
[^17]: https://sahamati.org.in/purpose-codes
[^18]: https://sahamati.org.in/aa-fair-use-template-library/aa-consent-template-id-ct004-wealth-management-and-or-advisory-services
[^19]: https://www.azbpartners.com/bank/consent-managers-under-indias-dpdp-act-and-dpdp-rules
[^20]: https://bfsi.economictimes.indiatimes.com/news/financial-services/indias-account-aggregator-ecosystem-facilitates-nearly-3-8-crore-financial-services-in-fy26/131958034
[^21]: https://bfsi.economictimes.indiatimes.com/articles/indias-account-aggregator-ecosystem-drives-rs-3-82-lakh-crore-loans-in-fy26/133562445
[^22]: https://www.business-standard.com/finance/news/rbi-recognises-sahamati-foundation-as-sro-for-account-aggregator-ecosystem-126060501286_1.html
[^23]: https://sahamati.org.in
[^24]: https://sahamati.org.in/saans-api-health-dashboard/
[^25]: https://consentos.in/learn/consent-manager-role
[^26]: https://candourlegal.com/dpdp-consent-manager-framework-2026
[^27]: https://www.scconline.com/blog/post/2026/06/26/account-aggregator-consent-manager-paradox-dpdp-rules-fintech-sector
[^28]: https://www.privacyglobal.org/blog/dpdp-act-consent-manager-registration
[^29]: https://sahamati.org.in/media/press-release
[^30]: https://m.economictimes.com/wealth/save/how-to-file-a-complaint-against-rbi-regulated-entity-under-the-integrated-ombudsman-scheme/articleshow/95954959.cms
