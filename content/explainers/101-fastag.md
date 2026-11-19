---
title: "FASTag 101: India's RFID Toll Rails, the Annual Pass and the Movement-Data Trail"
description: "A comprehensive guide to FASTag and the National Electronic Toll Collection (NETC) programme — IHMCL/NHAI operations, NPCI's clearing rails, RFID standards, the Annual Pass, cash-removal rules, adoption statistics, citizen rights, the National Transport Repository's privacy implications, safeguards and grievance routes."
date: 2026-11-19
draft: false
tags: ["fastag", "netc", "npci", "ihmcl", "nhai", "toll-collection", "rfid", "mlff", "annual-pass", "ntr", "dpdp", "privacy", "dpi", "india"]
categories: ["DPI Basics"]
image: "/images/fastag-101-cover.jpg"
author: "CashlessConsumer"
readingTime: "16 min"
---

# FASTag 101: India's RFID Toll Rails, the Annual Pass and the Movement-Data Trail

## What is FASTag?

**FASTag** is a passive RFID sticker affixed to a vehicle's windscreen that lets toll user fee be collected electronically while the vehicle passes a plaza — without stopping for cash. It is the consumer-facing face of the **National Electronic Toll Collection (NETC) programme**, a payments initiative of the **Ministry of Road Transport and Highways (MoRTH)** and the **National Highways Authority of India (NHAI)**, implemented by **Indian Highways Management Company Limited (IHMCL)**, an NHAI-promoted company, with the **National Payments Corporation of India (NPCI)** operating the central clearing system. [^1][^2][^3]

Three facts anchor its public significance. First, scale: over **98% of user fee collection on National Highways now flows through FASTag**, making it one of India's highest-penetration digital payment rails. [^1] Second, architecture: NETC is a **four-party payment system** — issuer bank, acquiring bank at the plaza, NPCI as central clearing house, and the plaza operator — so no FASTag transaction can occur without all three payment participants; the government describes this as a transparency safeguard, since every deduction is informed to the user and recorded centrally. [^1] Third, data: every crossing generates a timestamped, plaza-specific, vehicle-linked record, and MoRTH's **National Transport Repository (NTR)** policy now consolidates FASTag data with vehicle-registration, driving-licence, challan and accident databases — a fusion with significant surveillance potential that has drawn sustained constitutional criticism. [^4][^5]

FASTag is interoperable across issuers: a tag from any of the **~40 live member banks** works at any NETC plaza, [^17] and in 2026 the **'OneTag'** facility (launched at the Global Fintech Fest) let users change issuer banks while retaining the physical tag, on the model of mobile-number portability. [^6][^7]

### Historical Context

| Date | Milestone |
|---|---|
| Jun 2010 | MoRTH constitutes a committee headed by **Nandan Nilekani** to design the national ETC programme [^2] |
| 2012 | IHMCL incorporated to implement ETC infrastructure and operations [^3] |
| 4 Nov 2014 | NETC programme launched; NETC Procedural Guidelines first issued Feb–Apr 2016 [^8][^3] |
| Dec 2017 | FASTag mandated on sale of all new vehicles sold in India [^8] |
| 2017–18 | One dedicated FASTag lane provisioned at NH fee plazas; NETC clearing moved from four cycles to **two cycles a day** (Jan 2018) [^2][^3] |
| 15 Dec 2019 | FASTag made mandatory on all National Highway fee-plaza lanes; non-FASTag vehicles entering a FASTag lane charged **double fee** [^8][^9] |
| 15/16 Feb 2021 (midnight) | Mandate extended to **all category M & N vehicles**; all NH fee-plaza lanes declared "FASTag lanes" — hybrid/cash lanes discontinued [^10][^11] |
| 1 Apr 2021 | FASTag made mandatory for new third-party motor insurance under amendments to the Central Motor Vehicles Rules, 1989 [^11] |
| 2024 | **'One Vehicle, One FASTag'** enforced from 1 Feb 2024: only the most recently issued tag per vehicle remains operational; earlier tags deactivated/blacklisted; NPCI's June 2024 circular mandates issuer re-KYC of existing tags, with non-compliant tags to be blacklisted [^8][^12] |
| 15 Aug 2025 | **FASTag Annual Pass** launches for private non-commercial car/jeep/van: ₹3,000 for one year or 200 NH fee-plaza crossings [^13] |
| 15 Nov 2025 | National Highways Fee Rules, 2008 amended: a vehicle without valid FASTag entering a FASTag lane pays **2× fee in cash, 1.25× if paid via UPI** [^14] |
| 1 Feb 2026 | NHAI scraps the mandatory Know-Your-Vehicle (KYV) process for new car/jeep/van FASTag issuance, after user complaints about activation delays [^15] |
| 1 Apr 2026 | Annual Pass fee revised to **₹3,075** for FY 2026-27 [^1] |
| 10 Apr 2026 | **Cash discontinued at NH toll plazas**; UPI at 1.25× fee becomes the only fallback for vehicles without valid FASTag [^16] |
| May–Aug 2026 | First six **Multi-Lane Free Flow (MLFF)** barrier-free plazas go live — Choryasi (Surat, 1 May), Mundka (Delhi, 11 May), Daulatpura and Manoharpura (Jaipur), Gharaunda (Haryana), Shahjahanpur (Rajasthan) [^2][^1] |
| 2026 | **'OneTag'** issuer portability launched at the Global Fintech Fest; ~13 crore tags issued, ~6 crore active [^6] |
| Sep 2026 | NPCI reports 130.33 million cumulative tags, 40 live member banks; monthly toll-and-parking volume of 337.34 million transactions worth ₹7,096.35 crore [^17] |

## How It Works

### The Four Participants

| Role | What it does |
|------|--------------|
| **Issuer entity (bank)** | Sells and activates the FASTag to the customer, links it to a prepaid wallet or a savings/current/credit account, does KYC, maintains the customer's balance and handles complaints and refunds. [^1][^3] |
| **Acquiring bank (plaza side)** | Contracts with the toll plaza, collects transaction files from the plaza's Toll Management System (TMS), and acquires the toll transaction into the NETC network for settlement. [^1][^3] |
| **NPCI (central clearing)** | Owns and operates the NETC system: the **NETC Switch** (routes transactions to members), the **NETC Mapper** (national repository of NETC FASTag IDs, used by plazas to look up a tag's vehicle class and exception status) and the **NETC Real-time Clearing & Settlement system (NRCS)**, which nets and settles between members twice daily. [^3] |
| **Plaza operator / IHMCL** | Runs lanes, readers and the TMS; IHMCL — implementing ETC infrastructure on NHAI's mandate across **477 fee plazas** allocated to it — coordinates issuers, acquirers and STQC-certified system integrators. [^2] |

### The Transaction Flow

1. **Vehicle approaches** a NETC lane; the overhead reader interrogates the windscreen tag. The lane/TMS checks the tag ID format and its status on the **NETC Mapper**, including exception lists. [^3]
2. **Fee calculation** by vehicle class received from the Mapper; the transaction is sent online by the acquirer to the NETC system — the guidelines require transactions to reach the ETC system **within 15 minutes** of initiation; transactions beyond 15 minutes (up to 8 hours) may be sent with liability on the toll operator if the user's account has insufficient balance, and the issuer may then raise a chargeback. [^3]
3. **Clearing and settlement** twice a day: NRCS nets debit/credit obligations between issuer and acquirer members; disputes are settled in the first cycle, and NPCI gives the **final verdict** on unresolved disputes — while explicitly preserving the user's right to take the dispute to a consumer court or the banking ombudsman. [^3]
4. **User notification**: the deducted fee is communicated to the user (SMS/app) and recorded centrally. [^1]

### The Tag and Its Standards

NETC FASTags are **passive UHF RFID** tags conforming to the open standards **ISO 18000-6C** and **EPC Class 1 Gen 2** (India's regulatory band, roughly 865–868 MHz), with data encoding per GS1 standards and a tamper-evident construction — a tag removed from the windscreen cannot be reused. This is distinct from the 5.8 GHz DSRC technology used by ETC systems in China and Japan. Tags are vehicle-specific and non-transferable, with a physical validity of around five years. [^3][^18]

### Accounts, KYC and Exception Lists

- A FASTag can link to a **prepaid wallet** or directly to a bank account. Wallets are prepaid instruments governed by RBI's PPI framework, so minimum-KYC wallets carry balance caps (₹10,000) while full-KYC wallets do not; issuer banks perform KYC at onboarding. NPCI's June 2024 circular (NPCI/2024-25/NETC/001) required issuers to re-verify customers ("re-KYC") under the One Vehicle One FASTag programme, with non-compliant tags to be blacklisted. [^3][^12] From **1 February 2026** NHAI discontinued the additional Know-Your-Vehicle documentary process for new car/jeep/van FASTags. [^15]
- The NETC Mapper maintains **exception lists**: the **blacklist** (tag not accepted at any plaza — applied for incomplete KYC, duplicate tags on one vehicle, vehicle-class mismatch, or on request of law enforcement/Government/RBI), the **low-balance list** (balance below a threshold), and related statuses. A blacklisted tag's vehicle must pay by another mode; only the bank that added a tag to the blacklist can remove it. [^3]

### Tolling Models and Exemptions

- **Point-based (open) tolling**: each plaza crossing is one charge; **closed tolling** charges on entry-exit pairs over a distance. Fees vary by vehicle class. [^3]
- **Exemptions** exist under Rule 11 of the fee rules for dignitaries' vehicles and accompanying government security vehicles, emergency services and other notified categories, handled via specially issued tags. [^11]
- The **Annual Pass** (details below) overlays the standard fee schedule for eligible private vehicles. [^13]

### The Annual Pass (2025–26)

The Annual Pass, effective 15 August 2025, allows free passage for **private non-commercial car/jeep/van** at designated **NH and National Expressway fee plazas** for one year or **200 crossings**, whichever is earlier, on payment of ₹3,000 (FY 2025-26) / **₹3,075 (FY 2026-27)**. It is activated only through the **Rajmarg Yatra app or the NHAI website**, on an existing, properly affixed, non-blacklisted FASTag linked to a valid registration number (chassis-registered tags are ineligible). Key mechanics worth knowing as a user: [^13]

- **Counting**: at point-based plazas each crossing counts — a return trip is two crossings; in closed tolling one entry-exit pair is one crossing. [^13]
- **Scope**: at state-highway or state-managed expressway plazas the pass does not apply; the tag operates as a regular FASTag and normal fees apply. [^13]
- **Compliance risk**: commercial use of a pass-tagged private vehicle causes **immediate deactivation without notice**; the pass is non-transferable. [^13]
- **Wallet exclusion**: the pass fee cannot be paid from the FASTag wallet balance — it must be paid through the app's payment options. [^13]
- **Consent clause**: activation constitutes consent for the Rajmarg Yatra app to retrieve the user's registered mobile number from the issuing bank for SMS alerts — a small but real data-sharing event riders accept implicitly. [^13]
- After 200 crossings or one year, the tag **automatically reverts** to a normal FASTag. [^13]

### Barrier-Free Tolling: MLFF and the GPS Question

India's next tolling stage is **Multi-Lane Free Flow (MLFF)**: vehicles pay while moving at highway speed, identified by RFID (FASTag) readers, ANPR cameras and LiDAR/radar-based classification, with no lanes or gates. The first MLFF contract was signed in August 2025 with ICICI Bank for **Choryasi (Surat)**, which went live on 1 May 2026; six plazas were live by 1 August 2026. [^2] The government's July 2026 list shows 17 plazas awarded for MLFF, with bids invited for 104 more; IHMCL's annual report records 16 as awarded as of its date — the counts differ slightly across official sources. [^1][^2]

Notably, a fully **GPS/GNSS-based tolling** system — which would track vehicles continuously rather than at plaza checkpoints — has been **held back**: in Parliament, the government recorded that its Apex Committee and a High-Level Empowered Committee of industry and academia "in view of security and privacy considerations, breach and overall operational control" recommended **further deliberations** before GPS-based barrier-free tolling, and the state instead chose RFID+ANPR MLFF. [^1] Privacy advocates had long warned that GNSS tolling would amount to continuous movement monitoring. [^19]

## Key Statistics

| Metric | Value | Period / Source |
|---|---|---|
| Cumulative tags issued | **130.33 million (~13 crore)** | Sept 2026, NPCI monthly statistics [^17] |
| Active tags | ~6 crore | 2026, NPCI 'OneTag' release [^6] |
| Live issuer member banks | 40 | Sept 2026, NPCI [^17] |
| NETC share of NH user fee | >98% | Jul 2026, PIB (Govt in Parliament) [^1] |
| FY 2025-26 ETC transactions | 47,817 lakh (~4.78 billion) | IHMCL ETC Transaction Reports (NH+MoRTH+SH plazas) [^20] |
| FY 2025-26 ETC collection | **₹82,342 crore** (~14% up YoY) | IHMCL ETC Transaction Reports [^20] |
| FY 2024-25 ETC transactions / collection | 41,638 lakh / ₹72,390 crore | IHMCL ETC Transaction Reports [^20] |
| FY 2016-17 (baseline) | 236 lakh / ₹661 crore | IHMCL ETC Transaction Reports [^20] |
| Sept 2026 monthly volume & value | 337.34 million transactions / ₹7,096.35 crore (toll+parking, NPCI scope) | NPCI via Medianama [^17] |
| Average daily volume / value (Sept 2026) | 11.25 million / ₹236.55 crore | NPCI via Medianama [^17] |
| Average daily collection, NH+MoRTH plazas | ₹187.64 crore (Mar 2026); single-day high ₹213.80 crore (28 Feb 2026) | IHMCL Annual Report 2025-26 [^2] |
| Toll plazas on NETC | ~1,160 (Mar 2026), up from ~300 in 2016 | Mint report [^21] |
| Annual Pass: passes sold / transactions | 83.3 lakh passes; 71.1 crore transactions (Jul 2026); ~20% of FASTag transaction volume | IHMCL Annual Report 2025-26 [^2] |
| Annual Pass: Government figure | >77 lakh passes; 63 crore transactions (Jun 2026); ~33% of car/jeep/van ETC transactions | PIB, 22 Jul 2026 [^1] |
| Duplicate tags closed under One Vehicle One FASTag | >1.5 crore | IHMCL Annual Report 2025-26 [^2] |
| MLFF barrier-free plazas | 6 live; 17 awarded; bids for 104 more | IHMCL AR / PIB Jul 2026 [^2][^1] |

*Scope note:* NPCI's monthly statistics count NETC payment transactions including parking; IHMCL's series counts fee collected at NH, MoRTH and state-highway plazas. The two are related but not identical — use each against its own baseline.

## Layers Classification (L1-L7)

This is DPI Watch's analytical mapping, not an official government, NHAI or NPCI taxonomy.

| Layer | Classification | FASTag's role |
|---|---|---|
| **L1 — Vision & policy** | Infrastructure policy | Eliminate toll-plaza congestion and cash leakage; MoRTH/NHAI's barrier-free tolling goal, now pursued through MLFF rather than GPS-based tracking. [^1][^2] |
| **L2 — Regulation** | Rules and accountability | National Highways Fee Rules, 2008 (fees, double-fee and 1.25× UPI penalties, cash removal), CMVR 1989 amendments (vehicle mandate, insurance linkage), NPCI's binding NETC Procedural Guidelines, RBI PPI/KYC rules for wallets, DPDP Act 2023 for personal data. [^14][^16][^11][^3][^12] |
| **L3 — Digital rails** | Core infrastructure | NPCI's NETC Switch, NETC Mapper and NRCS clearing/settlement; plaza-side RFID readers, ANPR and Toll Management Systems; IHMCL's national implementation across 477 plazas. [^3][^2] |
| **L4 — APIs & protocols** | Interfaces and standards | Open RFID standards (ISO 18000-6C / EPC Gen 2), GS1 tag encoding, NETC message and clearing specifications, Mapper lookups; FASTag–VAHAN integration for toll-evasion e-notices. [^3][^4] |
| **L5 — Applications & access points** | User-facing systems | Issuer bank apps/websites and point-of-sale channels, e-commerce issuance via UPI apps, the Rajmarg Yatra app and NHAI site for the Annual Pass, ~1,160 plazas nationwide, plus parking and fuel-adjacent uses. [^6][^13][^21] |
| **L6 — Use cases** | Payment services | Highway/expressway toll, Annual Pass, state-highway tolls, parking, exemptions for notified categories; enforcement use (e-notices) is a distinct, contested use. [^13][^4][^11] |
| **L7 — Analytics & oversight** | Monitoring and reporting | IHMCL publishes plaza-level ETC reports and an annual impact assessment; NPCI publishes monthly product statistics; the NTR aggregates crossing data for government access — the layer where oversight is thinnest. [^20][^17][^4] |

## Regulatory Framework

- **National Highways Fee (Determination of Rates and Collection) Rules, 2008** — the fee rules under which tolls are set and penalties apply. Amendments effective **15 November 2025** codified that a vehicle entering a FASTag lane without a valid functional FASTag pays **twice the fee in cash**, or **1.25× via UPI**; a further amendment ended cash acceptance at NH plazas from **10 April 2026**, making UPI-at-1.25× the sole fallback. [^14][^16]
- **Central Motor Vehicles Rules, 1989 amendments** — FASTag mandatory for all category M & N vehicles from 15/16 February 2021; mandatory for new third-party insurance from 1 April 2021. [^10][^11]
- **NPCI NETC Procedural Guidelines** (current version 2.1, Dec 2025) — contractually binding on all members: participant roles, clearing cycles, exception lists, chargeback and dispute windows, KYC/AML obligations. [^3]
- **RBI prepaid instrument (PPI) and KYC directions** — govern FASTag wallets, balance caps under minimum KYC, and re-KYC duties; NPCI's June 2024 circular operationalised re-KYC for tags. [^12]
- **Motor Vehicles Act, 1988, Sections 25A and 62B; Section 136A** — statutory basis for the national registers (VAHAN/SARATHI) and electronic road-safety monitoring into which FASTag data is ingested via the NTR. [^4]
- **Digital Personal Data Protection Act, 2023 and DPDP Rules, 2025** — notified 13/14 November 2025 with a phased 18-month rollout; core obligations (notice, consent, erasure, breach reporting, SDF duties) bite around **May 2027**. Section 17 carve-outs for law-enforcement functions remain the principal weakness for transport data. [^22][^4]
- **Judicial validation** — the Bombay High Court rejected a PIL challenging the FASTag mandate and double-fee, holding the scheme aimed at efficient road travel and not violative of fundamental rights; the Centre had filed an affidavit arguing the mandate does not breach freedom of movement. [^15]

## Citizen Rights Analysis

**The right to pay is narrowing.** FASTag began as one option among several; it is now effectively the only toll payment channel on National Highways. From 15 November 2025 the non-tagged vehicle's choice was priced (2× cash, 1.25× UPI), and from 10 April 2026 cash was removed outright. For the digitally excluded — people without smartphones, UPI, bank accounts or a compliant tag — highway travel now carries a structural penalty rather than a payment choice. The UPI fallback exists, but at a punitive 1.25× rate that functions as a compliance tax, not a service. [^14][^16]

**Blacklisting is consequential and unevenly explained.** A blacklisted tag silently fails at plazas and triggers double fees; the causes (incomplete re-KYC, duplicate tags, class mismatch) are administrative and often invisible to the user until the fine is paid. The One Vehicle One FASTag programme deactivated older tags en masse from February 2024 — over 1.5 crore duplicate tags have been closed — a system-hygiene measure, but one executed against users who received little individual notice. [^3][^8][^2]

**Refunds are a right, but the burden sits on the user.** Wrong deductions must be disputed by the customer with the issuer bank; NETC guidelines oblige members to process disputes and preserve NPCI's final-verdict role, and explicitly preserve the user's right to consumer courts and the banking ombudsman. In practice timelines vary by bank — some banks commit provisional refunds for small disputed amounts within 2 working days, but investigated disputes commonly take 20–30 working days. [^3][^23][^24]

**Annual Pass conditions deserve reading before purchase.** Commercial use deactivates the pass without notice; state-highway travel isn't covered; crossings count both ways; and activation includes consent for the Rajmarg Yatra app to pull your mobile number from your bank. None of these is hidden, but all matter. [^13]

**The movement-data question is the structural one.** Every FASTag crossing is a location-and-time record for a registered vehicle. MoRTH's NTR policy lets law-enforcement agencies obtain "complete access" to NTR data on the strength of DPDP Section 17 exemptions — no warrant, no judicial authorisation, and (per civil-society analysis) no requirement to record queries. Citizens cannot know who has accessed their travel history. [^4] The government's own committees slowed GPS-based continuous tolling on privacy grounds — an implicit admission that movement surveillance is a real risk — while plaza-level ANPR+RFID tolling proceeds. [^1]

## Privacy Implications

- **Trip-chain construction.** A sequence of toll crossings, each with timestamp, plaza and vehicle class, reconstructs an individual's travel on tolled roads. Under the NTR policy this data sits alongside VAHAN owner-details, SARATHI licences, challans and accident records — enabling retrospective tracing of a vehicle's journeys and its owner in one query. [^4]
- **Law-enforcement access without judicial process.** The NTR policy grants mandated agencies complete access, invoking DPDP Act Sections 7(c) and 17(c); IFF's analysis argues this fails the *Puttaswamy* proportionality test — there is no limitation on scope, no oversight, and no purge obligation after a request expires. [^4]
- **Bulk exports.** Approved recipients can receive bulk data on password-protected hard disks or via SFTP with incremental refreshes, and — unlike time-boxed API access — the bulk pathway has no explicit validity period. India has been here before: MoRTH's 2019 bulk data-sharing policy, under which ~₹111 crore was earned selling VAHAN/SARATHI access to ~170 entities, was **withdrawn in June 2020** citing privacy concerns. The NTR revives bulk capability with fewer time-bound controls. [^4]
- **Consent via Aadhaar OTP is exclusionary.** Private-sector access to NTR personal data requires consent captured through an Aadhaar-authenticated OTP tied to the mobile number on record — meaning residents without Aadhaar-linked numbers must update their records before consent is even possible, and refusing has opaque consequences for services built on such consent. [^4]
- **ANPR adds a plate-and-image layer.** MLFF barrier-free tolling reads number plates with cameras and AI at highway speed, adding image-based identification to RFID reads and expanding the evidentiary surface available at plazas. [^2][^1]
- **Indefinite retention.** No NTR provision requires deletion of FASTag crossing data; the repository is treated as permanent. The DPDP Act's erasure principle is not operationalised for these flows. [^4]
- **What's protected, partially.** Public dashboards and open-data uploads of NTR/FASTag data are to be anonymised under NDSAP; the public NTR portal exposes limited fields behind OTP with a daily cap. These apply to *outward-facing* releases — identified government and bulk flows do not carry equivalent technical de-identification requirements. [^4]

## Safeguards

- **Architectural transparency in payment**: the three-participant rule (acquirer + NPCI + issuer) means no FASTag deduction occurs outside the clearing system, and every fee is notified to the user and recorded centrally — a control against off-system collection. [^1]
- **Binding member rulebook**: NETC Procedural Guidelines govern exception lists, transaction timelines, chargebacks and disputes across all banks, with NPCI as final arbiter and statutory escalation to consumer courts and the banking ombudsman preserved. [^3]
- **Manual Transaction Policy**: IHMCL accounts for and verifies every manual (non-electronic) transaction, targeting the historic leakage point of toll collection. [^2]
- **Audit and hosting conditions for data access**: NTR API/portal recipients need annual CERT-In-empanelled security audits, India-only hosting, IP whitelisting/MFA, logging and breach-notification duties, with debarment and penalties for violations. [^4]
- **Judicial and committee friction as safeguard**: the Bombay HC upheld the mandate but on efficiency grounds; the Apex Committee's privacy-driven pause on GPS tolling shows institutional review can slow the most invasive designs. [^15][^1]
- **Tamper-evident tags and dedup**: tags are non-reusable once removed, and One Vehicle One FASTag has closed >1.5 crore duplicate tags, reducing spoofing and double-billing vectors. [^18][^2]

**Open gaps**: no judicial warrant or query-logging requirement for law-enforcement access to crossing data; no retention limit or purge mechanism in the NTR policy; no individual notice regime for blacklisting beyond bank-level communication; and the DPDP regime's core obligations only bite from around May 2027, with Section 17 carve-outs intact. [^4][^22]

## Complaints & Grievance Redressal

1. **Wrong or double deduction — go to your issuer bank first.** Report promptly with date, plaza and amount; banks raise chargebacks into the NETC dispute process. Timelines are bank-specific: Kotak, for example, refunds disputed amounts up to ₹1,000 within 2 working days with a 20-day settlement window, while industry-wide investigated disputes commonly resolve in 20–30 working days. [^3][^23][^24]
2. **NHAI/IHMCL routes** — the 24×7 toll-free **1033** National Highways helpline (fee-free, launched 7 March 2018), the dedicated **falsededuction@ihmcl.com** email, and complaint lodging through the **Rajmarg Yatra app** are the government-designated channels for user-fee complaints, including Annual Pass glitches. [^1][^2]
3. **Blacklist or activation problems — the issuing bank again.** Only the bank that added a tag to the blacklist can remove it; for re-KYC or vehicle-linkage fixes, the issuer is the competent counterparty, and NETC's Mapper status is the record to query. [^3]
4. **Escalation** — if the issuer does not resolve, NPCI's final-verdict role applies within NETC, and the NETC guidelines explicitly preserve the user's right to the **consumer court** and the **banking ombudsman**; under the Reserve Bank – Integrated Ombudsman Scheme you may escalate to RBI's CMS portal if the regulated entity replies unsatisfactorily or not within 30 days (file within 90 days thereafter). [^3][^25]

## Prime References

[^1]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2287760
[^2]: https://ihmcl.co.in/wp-content/uploads/2026/10/ANNUAL-REPORT-2025-26.pdf
[^3]: https://ihmcl.co.in/wp-content/uploads/2025/12/NETC_PG_V2.1.pdf
[^4]: https://internetfreedom.in/data-highways-rights-roadblocks-an-explainer-on-the-national-transport-repository/
[^5]: https://parivahan.gov.in/sites/default/files/policy/data-sharing-policy.pdf
[^6]: https://www.npci.org.in/uploads/NPCI_Press_Release_Honble_Union_Minister_Shri_Nitin_Gadkari_Launches_One_Tag_to_Enable_NETC_FAS_Tag_Portability_at_Global_Fintech_Fest_2026_678a7af202.pdf
[^7]: https://economictimes.indiatimes.com/topic/fastag-annual-pass
[^8]: https://en.wikipedia.org/wiki/FASTag
[^9]: https://sg.finance.yahoo.com/news/fastag-rule-tell-why-important-133000993.html
[^10]: https://www.thehindu.com/news/national/fastag-mandatory-from-february-15-midnight-vehicles-sans-tag-to-pay-double-toll-fee/article61751342.ece
[^11]: https://nhai.gov.in/nhai/sites/default/files/mix_file/FAQ-FASTag.pdf
[^12]: https://avantiscdnprodstorage.blob.core.windows.net/legalupdatedocs/32834/NPCI_issued_the_Guidelines_for_New_Customer_Onboarding_and_Re_KYV_process_Jun212024.pdf
[^13]: https://ihmcl.co.in/wp-content/uploads/2025/08/FAQ-Annual-Pass_12.08.25-3.pdf
[^14]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2174761
[^15]: https://m.economictimes.com/topic/fastag-mandatory
[^16]: https://www.cnbctv18.com/auto/cash-toll-payments-end-april-10-upi-allowed-at-1-25x-fee-without-fastag-ws-el-19882115.htm
[^17]: https://www.medianama.com/2026/10/223-fastag-transactions-sept-2026-npci/
[^18]: https://tollguru.com/fastag-india
[^19]: https://www.medianama.com/2021/08/223-gps-based-toll-collection-status-3/
[^20]: https://ihmcl.co.in/etc-transaction-reports
[^21]: https://www.linkedin.com/posts/livemint_the-creation-of-indian-highways-management-activity-7496127041390411777-JGkU
[^22]: https://www.cyrilshroff.com/wp-content/uploads/2025/11/Client-Alert-DPDP-Rules-Nov-2025.pdf
[^23]: https://www.kotak.bank.in/en/help-center/cards/fastag/toll-related/qns-5.html
[^24]: https://auto.timesofindia.com/news/cars/fastag-wrong-deduction-how-to-raise-a-complaint-and-get-a-refund/articleshow/135600616.cms
[^25]: https://cms.rbi.org.in
