---
title: "Digi Yatra 101: India's Facial-Recognition Airport Rails and the Accountability Gap Behind Them"
description: "A comprehensive guide to Digi Yatra and the Digi Yatra Central Ecosystem — MoCA policy and the DigiYatra Foundation's Section-8 structure, self-sovereign identity enrolment, DYBBS face verification at entry, security and boarding, the 24-hour purge rule and its exceptions, adoption statistics, the Data Evolve vendor litigation, the Kerala High Court's data-protection orders, DPDP compliance timeline, safeguards and grievance routes."
date: 2026-11-26
draft: false
tags: ["digiyatra", "facial-recognition", "frt", "biometrics", "aviation", "moca", "aai", "digiyatra-foundation", "dyce", "dpdp", "privacy", "kerala-hc", "delhi-hc", "data-evolve", "dpi", "india"]
categories: ["DPI Basics"]
image: "/images/digiyatra-101-cover.jpg"
author: "CashlessConsumer"
readingTime: "15 min"
---

# Digi Yatra 101: India's Facial-Recognition Airport Rails and the Accountability Gap Behind Them

## What is Digi Yatra?

**Digi Yatra** is India's biometric-based digital passenger processing system for airports: a **Facial Recognition Technology (FRT)** platform, promoted by the **Ministry of Civil Aviation (MoCA)**, that lets domestic passengers clear terminal entry, security check and boarding gates by presenting their face instead of a boarding pass and physical identity document. It is implemented by the **Digi Yatra Foundation (DYF)** — a not-for-profit **Section 8 joint-venture company** majority-owned by five private airport operators — which operates the **Digi Yatra Central Ecosystem (DYCE)**. [^1][^2][^3]

Three facts anchor its public significance. First, scale: the government reports **over 11 crore (110 million) passenger journeys by more than 2.65 crore registered users across 39 domestic airports** as of November 2026, with average airport entry processing time cut from 15 seconds to 5 seconds — making Digi Yatra one of the world's largest deployed FRT systems for civilians. [^4][^5] Second, architecture: Digi Yatra follows a **decentralised, self-sovereign-identity model** on paper — the passenger's Digi Yatra ID travel credential (a signed bundle of validated ID data plus face biometric) is stored in an encrypted wallet on the passenger's own phone, and only a temporary face token is shared with the departure airport for the journey. [^1] Third, governance: the ecosystem is operated by a **private company that is not answerable under the Right to Information Act**, its founding technology vendor was dropped after its founder was arrested in a ₹36.53-crore fraud case with the system's source code, cloud credentials and data-ownership fought over in the Delhi High Court, and India's data-protection law (DPDP) still has **no fully functional enforcement board** — a combination that keeps Digi Yatra under sustained judicial and civil-society scrutiny. [^6][^7][^8][^9]

### Historical Context

| Date | Milestone |
|---|---|
| Aug 2018 | MoCA releases the first **Digi Yatra Policy** for biometric processing of passengers; enrolment conceived around a centralised "Digi Yatra ID" with Aadhaar as default identity [^10] |
| 2019 | **DigiYatra Foundation** incorporated as a Section 8 not-for-profit joint venture: **AAI 26%**, with Delhi (DIAL), Mumbai (MIAL), Bengaluru (BIAL), Hyderabad (GHIAL) and Cochin (CIAL) airports jointly holding the remaining **74%**; custodian of the Passenger ID validation process and builder of DYCE [^3] |
| 2021 | **Updated Digi Yatra Policy** — decentralised architecture, encrypted wallet on passenger device, 24-hour face purge at airports, and a value-added-services consent framework [^1][^11] |
| 1 Dec 2022 | App-based launch at **Delhi, Varanasi and Bengaluru** airports by the then Civil Aviation Minister [^12][^13] |
| Apr 2023 | Expanded to **Vijayawada, Kolkata, Hyderabad, Pune** (7 airports); ~1.74 million users in the first six months [^12][^14] |
| Jun 2023 | Crosses **1 million users**; Delhi T3 begins app-less processing using airline data [^13] |
| Aug 2023 | Six more airports — **Mumbai, Ahmedabad, Kochi, Lucknow, Jaipur, Guwahati** — take the count to 13 [^15] |
| Oct–Nov 2023 | Andhra Pradesh police uncover **₹36.53 crore** e-challan fraud; Data Evolve Solutions CEO **Avinash Komireddy arrested (Nov 2023)** — Data Evolve was the startup that built the Digi Yatra ecosystem and app after winning a NITI Aayog Atal Innovation Mission challenge in 2021 [^16][^6] |
| Jan 2024 | Internet Freedom Foundation publishes **"Resist Surveillance Tech, Reject Digi Yatra"**; MoCA tells lawmakers "all data is stored in mobile of passenger" [^7][^17] |
| Mar 2024 | DYF severs ties with Data Evolve; researcher @kingslyj shows **old app versions transmitted passenger data to Data Evolve's AWS endpoint**; Delhi High Court (CS(Comm) 265/2024) grants DYF an ad-interim injunction and orders handover of source code, credentials and platform control, calling Digi Yatra critical infrastructure [^16][^17][^6] |
| Apr 2024 | Old app deactivated ("bricked") and users force-migrated to a new app under DYF's own developer domain; DYF CEO denies any central storage of passenger data [^13][^18] |
| 21 Feb 2024 | **45.8 lakh downloads; 1.45 crore passengers** enrolled-and-travelled cumulatively [^14] |
| Jul 2024 | Coverage reaches **28 airports (~90% of India's air traffic)** [^14] |
| Jul 2024 | NITI Aayog's National AI Strategy team study on Digi Yatra (published via press) flags **undefined deletion rules for non-biometric data**, calls for opt-in value-added services, cybersecurity audits and FRT bias standards [^19][^20] |
| Nov 2025 | Delhi HC **frames issues for trial** in DYF v. Data Evolve — including who owns the Digi Yatra Central Ecosystem and **who owns passenger data**; Data Evolve alleges KPMG cloned the app and deployed it at 28 airports beyond the licensed 4 [^6] |
| 13–14 Nov 2025 | **DPDP Rules, 2025 notified** (G.S.R. 846(E)): Data Protection Board provisions in force; substantive data-fiduciary obligations deferred to May 2027 [^21][^22] |
| 5 Mar 2026 | **Kerala High Court issues notice** to DYF and the Union on a PIL by C.R. Neelakandan (W.P.(PIL) No. 15 of 2026) alleging DPDP-non-compliant handling of passenger data, including onward commercial sharing [^23][^24] |
| Mar 2026 | Court observes **Aadhaar should not be mandatory** for registration; DYF confirms Aadhaar or Driving Licence accepted; bench expects **Voter ID** to be considered [^25][^8] |
| 30 May 2026 | **10 crore journeys, 2.4 crore downloads, 38 airports** (PIB); 27 more airports promised by next year; greenfield airports Navi Mumbai, Jewar and Bhogapuram to be fully Digi Yatra-enabled; 11 languages in-app with 11 more planned [^4] |
| 7 Oct 2026 | Kerala HC disposes the PIL, recording that **"privacy of citizens is being compromised"**, directs the Union to make the **Data Protection Board functional within 8 weeks**, and expects Digi Yatra compliance with the DPDP Act and DPDP Rules, 2025 [^8][^26] |
| 1 Nov 2026 | **International trials begin** at seven airports — Delhi, Mumbai, Bengaluru, Hyderabad, Chennai, Kochi and Amritsar — for Indian nationals with e-passports on select Air India and IndiGo flights, running through Nov–Dec 2026; official count rises to **2.65 crore users, 11 crore journeys, 39 domestic airports**, with 25 more domestic airports planned for 2027 [^5][^27] |

## How It Works

### The Three Actors

| Actor | Role |
|------|------|
| **DigiYatra Foundation (DYF)** | Section 8 not-for-profit JV (AAI 26%; five private airport operators 74%). Custodian of the Passenger ID validation process; develops and operates the **Digi Yatra Central Ecosystem (DYCE)** — enrolment, authentication, consented profile sharing, and the app. As a private company, DYF is **outside the RTI Act's scope**. [^3][^6] |
| **Airports (via DYBBS)** | Each airport runs the **Digi Yatra Biometric Boarding System (DYBBS)** — face-capture kiosks and e-gates at terminal entry, security check and boarding. The airport receives the passenger's face token + boarding-pass data only for the journey. [^1] |
| **Passenger's device** | The Digi Yatra ID travel credential — validated identity data plus face biometric — is stored in an **encrypted wallet on the passenger's phone** under the decentralised design; the passenger shares a copy with the departure airport per flight. [^1] |

### Enrolment (one-time)

1. **Register** on the Digi Yatra app (Android/iOS) with a mobile number and OTP — the Aadhaar-linked number is recommended for smooth verification. [^2]
2. **Verify identity** using **DigiLocker** or **Aadhaar** (offline XML / eKYC); a driving licence is also accepted. Following the Kerala High Court's observation, DYF told the court that Aadhaar is not the only accepted document and the bench expects Voter ID to be considered. [^2][^25][^8]
3. **Take a selfie** with liveness detection; the live face is matched against the reference photo from the validated ID. On success, the **Digi Yatra ID travel credential** is created and stored in the app wallet. If selfie-matching fails or the chosen ID lacks a digital database, the app issues a QR flag for **one-time physical ID validation by CISF** at the airport. [^1]
4. **Consent is layered**: consent for face-biometric sharing with airport checkpoints is integral; **value-added services** (ecosystem partners) and **marketing/promotional profiling by airports** require separate, independent opt-in consent with a **one-click opt-out** in the app. [^1]

### The Travel Day

1. **Share credential**: the passenger uploads the boarding pass in the app and shares it (with the face token) with the departure airport. [^2]
2. **Entry e-gate**: the passenger scans the boarding-pass barcode at the gate; the camera captures the face; DYBBS validates the boarding pass with the airline's departure-control system and matches the face. On success, the gate opens. [^1]
3. **Security check and boarding**: the face alone authenticates the passenger at the security checkpoint face-pod and the boarding e-gate; boarding-pass scans are progressively eliminated across checkpoints. [^2][^28]
4. **Purge**: facial data **cannot be stored by the airport beyond the passenger's transit** and must be purged from DYBBS **24 hours after the flight's departure**. A **day-of-travel enrolment** option exists at the airport for unregistered passengers, valid for that journey only, with biometrics purged after travel. [^1]

### The Small Print (from the official policy)

Three clauses qualify the privacy promise, straight from MoCA's Digi Yatra Policy: [^1]

- **Purge settings are changeable**: DYBBS "shall have an ability to change the data purge settings based on security requirements on a need basis."
- **Travel logs persist**: passenger travel logs *without* the biometric "shall be stored for the purpose of audits as per the mandate from Govt. of India."
- **Government access**: "Any Security Agency, GOI or other Govt. Agency may be given access to the passenger data based on the current/existing protocols prevalent at that time."

For international travel, biometric capture "(Face, Iris, Fingerprints) … will be as mandated by the Govt. of India as per existing protocols" — relevant now that international trials are live. [^1][^5]

## Key Statistics

| Metric | Value | Date & Source |
|---|---|---|
| Registered users | **2.65 crore (26.5 million)** | Nov 1, 2026 — MoCA release [^5] |
| Cumulative journeys | **11 crore (110 million)** across 39 domestic airports | Nov 1, 2026 — MoCA release [^5][^27] |
| App downloads | **2.4 crore** (iOS + Android) | May 30, 2026 — PIB [^4] |
| Earlier trajectory | 45.8 lakh downloads; 1.45 crore passengers | Feb 2024 — PIB [^14] |
| Airport coverage | 39 domestic airports; **25 more planned in 2027** | Nov 1, 2026 — MoCA release [^5] |
| Entry processing time | **15 → 5 seconds** (government claim) | May 30, 2026 — PIB [^4] |
| Language support | 11 languages; 11 more planned | May 30, 2026 — PIB [^4] |
| International trials | 7 airports, e-passport holders, Air India + IndiGo | Nov–Dec 2026 — MoCA release [^5] |
| Greenfield airports | Navi Mumbai, Jewar, Bhogapuram to be fully Digi Yatra-enabled | May 30, 2026 — PIB (Minister statement) [^4] |
| Traffic context | Daily domestic traffic below 2 lakh (2014) to 5 lakh+; official projection of 50 crore annual passengers by 2030 | May 30, 2026 — PIB (Minister statement; projection) [^4] |

Unverified claim, flagged: the Play Store listing separately shows **10M+ downloads** for the current app, consistent with but not equal to the 2.4-crore cumulative figure across both old and new apps. [^18]

## Layers Classification (L1-L7)

This is DPI Watch's analytical mapping, not an official government or MoCA taxonomy.

| Layer | Classification | Digi Yatra's role |
|---|---|---|
| **L1 — Vision & policy** | Infrastructure policy | MoCA's "Ease of Flying" agenda: paperless, contactless passenger processing; Digi Yatra Policy 2018 (centralised concept) superseded by the 2021 decentralised policy; scale-up tied to projected 50-crore-passenger-by-2030 growth. [^10][^1][^4] |
| **L2 — Regulation** | Rules and accountability | No anchoring statute — a standalone ministry policy; Aadhaar Act 2016 for eKYC; IT Act/ITAA 2000/2008 cited as the legacy privacy baseline; **DPDP Act 2023 + DPDP Rules 2025** (phased, full obligations May 2027); judicial oversight from Delhi HC (vendor/ownership) and Kerala HC (data protection, identity choice). [^1][^21][^22][^8][^11] |
| **L3 — Digital rails** | Core infrastructure | DYCE operated by a private Section 8 JV; DYBBS face-verification infrastructure at each airport; encrypted wallet credential on passenger devices; CISF as the manual-validation fallback. [^3][^1] |
| **L4 — APIs & protocols** | Interfaces and standards | Self-sovereign-identity credential model; DigiLocker/Aadhaar eKYC integration; face-token sharing between app and departure airport; IATA Resolution 792 barcoded boarding pass compatibility; airline departure-control-system (DCS) validation hooks. [^1][^2] |
| **L5 — Applications & access points** | User-facing systems | Digi Yatra app (Android/iOS, 11 languages, multilingual expansion); airport entry e-gates, security face-pods, boarding e-gates; day-of-travel enrolment kiosks; airport helpdesks. [^4][^1] |
| **L6 — Use cases** | Identity services | Terminal entry, security check, boarding for domestic passengers; **international departures (trials, Nov–Dec 2026)**; value-added services (cab/hotel/lounge offers) permitted under opt-in — a use contested by privacy researchers. [^5][^1][^11] |
| **L7 — Analytics & oversight** | Monitoring and reporting | Travel logs retained "for audits as per the mandate from Govt. of India"; policy clauses permit government/security-agency access; **no published independent security audit, no RTI exposure, and no statutory grievance mechanism in the policy** — the layer where oversight is thinnest. [^1][^11][^19] |

## Regulatory Framework

- **Digi Yatra Policy (MoCA), 2018 and 2021** — the sole governing instrument: architecture, consent framework, 24-hour purge, travel-log retention, value-added-services rules. It prescribes no penalties, no independent auditor and no grievance mechanism; it cites the IT Act 2000/ITAA 2008 and Aadhaar Act 2016 as the applicable privacy baseline. [^10][^1][^11]
- **Aadhaar (Targeted Delivery of Financial and Other Subsidies, Benefits and Services) Act, 2016** — legal basis for Aadhaar-based eKYC in enrolment; DYF's ecosystem would require UIDAI AUA/KUA licensing or subscription if Aadhaar authentication is used, per the 2018 policy. [^1][^10]
- **Digital Personal Data Protection Act, 2023 and DPDP Rules, 2025** — notified 13–14 November 2025 (G.S.R. 846(E)). In force now: definitions, Data Protection Board establishment provisions, rule-making powers, and the Section 44(3) RTI amendment. **Consent Manager registration opens 13 November 2026; full substantive obligations (notice, consent, erasure rights, breach reporting, penalties up to ₹250 crore) commence 13 May 2027.** Until then, the Kerala HC has directed the Board be made functional within 8 weeks of its 7 October 2026 order, and expects Digi Yatra compliance with the Act and Rules. [^21][^22][^8]
- **Right to Information Act, 2005 — the exemption problem**: DYF is a private Section 8 company, so RTI does not apply to it directly; RTI queries route to MoCA/AAI, which have pointed petitioners back to the Foundation. [^6][^13]
- **Puttaswamy v. Union of India (2017)** — the constitutional privacy standard (legality, necessity, proportionality). Analysts argue Digi Yatra currently fails the legality limb (no statute), and that convenience alone cannot justify the privacy intrusion (necessity/proportionality). The voluntary nature of the service is central to any proportionality defence — which is why any move to mandatory use would trigger the Puttaswamy tests directly. [^11][^19]
- **Judicial supervision, live**: Delhi HC, *Digi Yatra Foundation v. Data Evolve Solutions Pvt. Ltd.*, CS(Comm) 265/2024 — March 2024 ad-interim injunction restoring platform control to DYF and ordering handover of source codes and credentials; issues framed for trial in November 2025 include ownership of DYCE and of passenger data. Kerala HC, *C.R. Neelakandan v. Union of India*, W.P.(PIL) No. 15 of 2026 (decided 7 Oct 2026, 2026:KER:77409) — Data Protection Board functional within 8 weeks; Aadhaar non-mandatory; Voter ID to be considered; DPDP compliance expected. [^6][^8][^25][^26]

## Citizen Rights Analysis

**1. Voluntary — in principle, and courts are watching it stay that way.** The policy states enrolment "will be completely voluntary" with an opt-out and profile deletion at any time. [^1] Researchers caution that consent to a state-linked facial-recognition service is structurally weakened: citizens' deference to government requests, and the fact that individuals cannot meaningfully assess the threats of face-based identification, make consent a defective safeguard — "for Digi Yatra to be truly voluntary… the current model of implementation needs an overhaul." [^13] If use ever becomes mandatory in effect, the Puttaswamy legality-necessity-proportionality tests apply squarely. [^19]

**2. Identity choice exists but is narrow.** Aadhaar and driving licence are accepted; the Kerala HC has recorded that Aadhaar must not be mandatory and expects Voter ID acceptance. There is currently **no fully ID-less option** — a government-issued credential anchors the credential. [^25][^8][^2]

**3. Data-principal rights are promised, not yet enforceable.** Erasure, correction and consent-withdrawal rights under the DPDP Act become operative **13 May 2027**; until then, deletion depends on the app's own flows and DYF's privacy policy (effective 27 October 2024). [^21][^22][^29] The Data Protection Board — the enforcement forum — is being constituted under judicial pressure, not yet hearing complaints. [^8]

**4. Accountability is asymmetric.** The state promotes Digi Yatra; a private foundation runs it; the RTI Act reaches neither directly. Civil-society RTI requests to AAI have been answered by pointing to DYF. [^13][^6] For a system holding biometric-linked credentials of 2.65 crore citizens, this is the single largest structural rights gap.

**5. Your face is your credential — and your exposure.** A face cannot be re-issued like a card. Exclusion errors (failed matches at e-gates) have been a persistent concern of FRT deployments globally; India's policy answers this with the CISF manual-validation fallback, but publishes no error-rate or demographic-bias data. The NITI Aayog study team explicitly asked for **FRT bias standards** and an identified standards body — still outstanding. [^1][^19][^20]

## Privacy Implications

- **"Data stays on your phone" is the design, not the proof.** MoCA's April 2023 statement claimed no central storage of PII; the founder-CEO of the company that actually built the ecosystem described authentication taking place **on AWS cloud**; The Ken's investigation found the device-only claim unlikely to hold in full; and in March 2024 a researcher demonstrated the old app transmitting passenger data to Data Evolve's AWS endpoint. DYF's CEO denies any data residing outside passenger phones or the Foundation. These accounts have never been reconciled by an independent audit. [^11][^16][^6][^18]
- **The 24-hour purge has carve-outs.** Purge settings are changeable "based on security requirements"; travel logs (identity + movement, minus the biometric) are retained for government-mandated audits; and government/security agencies may access passenger data "based on existing protocols." The biometric purge is narrow; the metadata trail is not. [^1]
- **Value-added services create a commercialisation path.** The 2021 policy allows ecosystem partners to offer services (cab, hotel, lounge) and allows airports to build marketing profiles — under separate opt-in consent. Privacy researchers and the Kerala PIL both flag this as the doorway for onward sharing of passenger data. [^1][^11][^23]
- **International expansion widens biometric capture.** The policy contemplates face, iris and fingerprints for international travel "as mandated by GoI protocols" — the Nov 2026 trials are the first step. Spain's data-protection authority shut down facial-recognition boarding at the country's airports and fined Aena €10 million in November 2025 over an inadequate impact assessment; Italy suspended FRT boarding trials at Milan; the global regulatory direction is tightening while India scales up. [^1][^5][^30]
- **Vendor concentration risk is proven, not hypothetical.** A single startup held the source code, cloud credentials and domain control of a critical biometric platform serving crores of passengers; separating it required emergency judicial intervention. The trial over who owns the codebase — and the passenger data — is pending. [^6][^17]

## Safeguards

**Built into the system (as designed):**

- Strictly voluntary enrolment; **opt-out and profile deletion at any time** from the app. [^1]
- **24-hour face purge** from airport DYBBS after flight departure; day-of-travel enrolments valid only for that journey. [^1]
- **Separate, independent consent** for value-added services and marketing profiling, with a **one-click opt-out**; marketing profiling requires explicit consent. [^1]
- **Encrypted wallet** storage of the Digi Yatra ID on the passenger's device; only a temporary face token shared per journey. [^1]
- **Liveness detection** during selfie enrolment; CISF physical-ID fallback for failed matches. [^1]
- Post-2024 migration to an app published under **DYF's own developer identity**, after the vendor split. [^13][^18]

**Emerging from courts and law:**

- **Kerala HC orders (2026)**: Aadhaar not mandatory; Voter ID to be considered; Data Protection Board functional within 8 weeks; DPDP Act + Rules compliance expected. [^25][^8]
- **Delhi HC supervision** of the vendor dispute, with ownership of DYCE and passenger data formally framed for trial. [^6]
- **DPDP Rules, 2025 phased obligations**: Consent Managers from 13 Nov 2026; notice, consent, erasure, breach-reporting duties and penalties up to ₹250 crore from 13 May 2027. [^21][^22]

**What a citizen can do today:**

- Enrol only if the convenience is worth it — the paper boarding pass + physical ID path remains fully valid at every airport.
- **Decline the value-added-services and marketing consents** during registration; they are separate toggles.
- Prefer the **driving licence** over Aadhaar if you want to minimise Aadhaar exposure (court-recorded as accepted).
- **Delete your profile** from the app after travel if you enrol selectively; the policy promises deletion on opt-out. [^1]
- Keep proof of any deletion request; until May 2027 there is no statutory erasure remedy, only the policy promise and DYF's privacy policy. [^29][^21]

## Complaints & Grievance Redressal

The Digi Yatra Policy itself prescribes **no grievance mechanism and no penalties** — a gap critics have repeatedly flagged. [^11] Working routes today:

1. **DigiYatra Foundation customer care**: **customercare@digiyatrafoundation.com** (app/language feedback and issues); app-support contact **dyceadmin@digiyatrafoundation.com**; developer phone **+91 74111 47575** per the Play Store listing. [^18][^29]
2. **Airport helpdesks and helplines** — MoCA has published airport-specific Digi Yatra helplines (e.g. Delhi: 0124-4797311; Bengaluru: 080-22012001); failed e-gate matches route to CISF manual verification. [^31][^1]
3. **AirSewa portal/app (MoCA)** — the ministry's official passenger-grievance channel for all aviation services, named by the Minister alongside Digi Yatra. [^4]
4. **DPDP route**: once the **Data Protection Board** is functional (Kerala HC deadline from the 7 Oct 2026 order), complaints about passenger-data handling can go to the Board; substantive data-principal rights are enforceable from **13 May 2027**. [^8][^21]
5. **RTI route**: queries about the programme to **MoCA/AAI** (DYF is outside RTI); expect partial answers, as civil-society petitioners have. [^13]
6. **Courts**: the constitutional route remains open — the Kerala and Delhi High Court proceedings were both initiated or shaped by petitioners and litigants, not by any regulator. [^8][^6]

## Prime References

[^1]: https://www.civilaviation.gov.in/sites/default/files/2023-07/Digi%20Yatra%20Policy%20%28DIGI%20YATRA%29.pdf
[^2]: https://www.newdelhiairport.in/digi-yatra
[^3]: https://pib.gov.in/PressReleasePage.aspx?PRID=1842408
[^4]: https://pib.gov.in/PressReleasePage.aspx?PRID=2267024
[^5]: https://www.newindianexpress.com/india/2026/Nov/01/digi-yatra-begins-international-passenger-trials-at-seven-airports-2
[^6]: https://internetfreedom.in/digiyatra-who-owns-your-data
[^7]: https://www.biometricupdate.com/202404/digi-yatra-sidelines-legacy-facial-recognition-app-maker-amid-data-breach-rumors
[^8]: https://www.thehindu.com/news/national/kerala/privacy-of-citizens-being-compromised-says-kerala-hc-directs-centre-to-make-data-protection-board-functional-in-eight-weeks/article71571131.ece
[^9]: https://www.firstpost.com/explainers/digiyatra-storing-passenger-data-controversy-13760590.html
[^10]: https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=1548561
[^11]: https://www.theindiaforum.in/technology/digi-yatra-service-or-surveillance
[^12]: https://www.business-standard.com/companies/news/facial-recognition-platform-digi-yatra-downloads-cross-1-million-mark-123062200844_1.html
[^13]: https://en.wikipedia.org/wiki/Digi_Yatra
[^14]: https://www.impriindia.com/insights/policy-update/digiyatra-2022-biometric-boarding
[^15]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=1947913
[^16]: https://www.thehindu.com/sci-tech/technology/digi-yatra-foundation-drops-app-maker-after-data-breach/article68093722.ece
[^17]: https://digitalstatecraft.substack.com/p/what-the-digiyatra-case-teaches-us
[^18]: https://play.google.com/store/apps/details?id=org.digiyatra.org
[^19]: https://www.thehindu.com/news/national/digi-yatra-policy-must-clarify-data-deletion-rules-privacy-concerns-study/article68355749.ece
[^20]: https://www.biometricupdate.com/202407/digi-yatra-needs-more-individual-control-over-data-privacy-niti-aayog-argues
[^21]: https://static.pib.gov.in/WriteReadData/specificdocs/documents/2025/nov/doc20251117695301.pdf
[^22]: https://dpdpactindia.in/dpdp-compliance-timeline
[^23]: https://www.medianama.com/2026/03/223-kerala-high-court-issues-notice-pil-data-privacy-violations-digi-yatra
[^24]: https://www.livelaw.in/high-court/kerala-high-court/digi-yatra-data-protection-concerns-kerala-high-court-seeks-response-of-centre-digi-yatra-foundation-525518
[^25]: https://www.moneylife.in/article/aadhaar-should-not-be-mandatory-for-registering-on-digiyatra-kerala-high-court-remarks/81069.html
[^26]: https://24law.in/story/make-data-protection-board-functional-within-8-weeks-kerala-high-court-flags-privacy-concerns-over
[^27]: https://etedge-insights.com/technology/innovation/digi-yatras-international-expansion-raises-a-bigger-question-about-passenger-data
[^28]: https://csmia-mumbai.adaniairports.com/en/airport-facilities/digiyatra
[^29]: https://digiyatrafoundation.com/privacy-policy
[^30]: https://the-ken.com/newsletter/make-india-competitive-again/digiyatra-is-an-exception-that-proves-the-rule-on-indias-data-privacy
[^31]: https://x.com/MoCA_GoI/status/1614660095228665861
