---
title: "ONDC 101: India's Open Network for Digital Commerce"
description: "A comprehensive guide to ONDC — the government-backed open protocol network that unbundles e-commerce into interoperable buyer apps, seller apps and logistics, aiming to do for shopping what UPI did for payments."
date: 2026-09-10
draft: false
tags: ["ondc", "dpi", "digital-commerce", "dpiit", "beckn", "e-commerce", "msme", "india"]
categories: ["DPI Basics"]
image: "/images/ondc-101-cover.jpg"
author: "CashlessConsumer"
readingTime: "14 min"
---

# ONDC 101: India's Open Network for Digital Commerce

## What is ONDC?

The **Open Network for Digital Commerce (ONDC)** is a Government of India initiative of the **Department for Promotion of Industry and Internal Trade (DPIIT), Ministry of Commerce and Industry**, designed as population-scale digital infrastructure for commerce. Launched as a pilot in **April 2022**, it promotes open networks for the exchange of goods and services over digital or electronic networks, using open-source methodology, open specifications and open network protocols that are independent of any specific platform. [^1]

ONDC is not an app, not a marketplace and not a regulator. It is best understood as a set of **interoperable specifications and network policies** that let any buyer application discover and transact with any seller application — the way UPI let any UPI app pay any bank account. A buyer on one app can order from a seller onboarded by a completely different seller app, with a third party providing logistics, and payment flowing through any rail. [^2][^3]

The network is built and operated by **ONDC**, a private **Section 8 (non-profit) company** incorporated on **31 December 2021**, incubated at the **Quality Council of India (QCI)** with **Protean eGov Technologies** (formerly NSDL e-Governance) as co-founder. It has an authorized capital of ₹500 crore, with 33 banks, exchanges, depositories and enterprises as investors — including SBI, ICICI Bank, HDFC Bank, Bank of Baroda, NABARD, SIDBI, BSE, NSE, CDSL and NSDL. [^1][^4][^5]

### Historical Context

| Date | Milestone |
|---|---|
| 27 Nov 2020 | DPIIT sets up e-commerce steering committee [^6] |
| 5 Jul 2021 | Nine-member ONDC Advisory Council constituted, chaired by the Union Commerce Minister (members included Nandan Nilekani) [^7] |
| 31 Dec 2021 | ONDC incorporated as Section 8 non-profit company [^4] |
| 29 Apr 2022 | First order on the network — a bunch of coriander delivered in Bengaluru [^2] |
| Apr 2022 | Closed test pilot across Delhi, Bengaluru, Shillong, Coimbatore and Bhopal [^6] |
| 30 Sep 2022 | Network opened to consumers in 16 Bengaluru locations [^6] |
| Mar 2023 | Ride-hailing goes live (Namma Yatri et al.) [^2] |
| Aug 2024 | 100 million cumulative transactions; six-minute paperless loans demonstrated [^2] |
| 13 Jan 2026 | India Post delivers its first ONDC order as a Logistics Service Provider [^8] |
| 25 Jul 2026 | 500 million cumulative transactions [^2] |

## How It Works

Traditional e-commerce is **platform-centric**: the platform controls buyer interface, seller onboarding, logistics and payments in one walled system. ONDC unbundles this value chain into **roles**, connected by open protocols — a **network-centric** model. [^3][^9]

### The Roles (Network Participants)

1. **Buyer Network Participant (buyer app)** — the consumer-facing application where demand originates (e.g., Paytm, Magicpin, PhonePe's Pincode, Ola, Namma Yatri)
2. **Seller Network Participant (seller app)** — onboards sellers/catalogues and makes them discoverable network-wide (e.g., Bitsila, Mystore, Shiprocket, Magicpin)
3. **Logistics Service Provider (LSP)** — fulfils delivery (Delhivery, India Post, Shadowfax, small fleet operators via FleetConnect)
4. **Gateway** — routes search/discovery requests across the network and emits anonymised, aggregated network metrics [^4][^9]

### The Protocol Stack

ONDC's backend is built on the **Beckn Protocol**, an open-source, decentralised commerce protocol. On top of this base layer, ONDC adds a **network extension layer** — domain-specific API contracts, plus governance specifications for registration, grievance redressal (IGM), reconciliation and settlement (RSF), and data policies. The core commercial interactions — discovery, order, fulfilment, post-fulfilment — are standardised as certified open APIs that every participant implements. [^4][^9][^10]

A simplified transaction flow:

1. A buyer searches for a product in **any** buyer app
2. The buyer app's search request is broadcast through the **gateway** to seller apps across the network
3. Seller apps return catalogue results; the buyer app displays them with standardised comparison data
4. The buyer orders and pays inside the buyer app using any payment rail (UPI, cards, wallets, cash-on-delivery)
5. A logistics provider — chosen by seller or buyer — fulfils the order
6. Post-fulfilment, rating, refund and grievance flows run through standardised IGM/RSF specifications [^9][^13]

Because search is network-wide, price discovery happens across all participating apps — the network's answer to platform lock-in and self-preferencing in search results. [^1][^3]

## Key Statistics

*(Network figures as of the latest verifiable official reporting; ONDC publishes a live counter at ondc.org.)*

| Metric | Value | As of |
|---|---|---|
| Cumulative transactions | **500+ million** [^2] | 25 July 2026 |
| Monthly transactions | **~12 million** (4.4M mobility, 7.6M non-mobility) [^11] | July 2026 |
| Peak daily orders | ~430,000 [^11] | July 2026 |
| FY2023 vs FY2026 transactions | 0.2M → 218M [^12] | FY2026 |
| Sellers/service providers onboarded | ~6.4 lakh (640,000) [^11]; 7.6 lakh per ONDC site snapshot May 2025 [^5] | Jul 2025–May 2026 |
| **Active** retail merchants | 200,000+ [^12] | July 2026 |
| Cities live / delivery reach | 609+ cities live; delivery to 1,200+ cities [^11][^19] | 2024–2026 |
| Daily transit tickets booked | 375,000+ across 35+ apps, 9 metro systems + 4 city bus operators [^2] | June 2026 |
| Ride-hailing drivers on network | 1 million+ [^12] | 2026 |
| Credit disbursed / investments via network | ₹375 crore credit; ₹192 crore invested, 29 AMCs live [^2] | June 2026 |
| Institutional investors | 33 banks, exchanges, depositories, enterprises [^2] | 2026 |

**Verified domain-level data points:** In food & beverages, an independent study of network participants put ONDC at 18% market share in Bengaluru and ~3% nationally (July 2024). [^19] India Post joined as a logistics provider in January 2026, extending delivery reach to the postal network. [^8]

**⚠️ Conflicting figures — read with care:** ONDC reports **onboarded** sellers/service providers (~6.4–7.6 lakh), while independent reporting counts **active** retail merchants (200,000+). [^11][^12] The gap between onboarded and actively transacting sellers is the single most contested number about the network; treat "lakh sellers" headlines accordingly. Similarly, "launch" is variously dated to the 2021 incorporation, the April 2022 pilot, or the September 2022 consumer opening — this explainer dates the network's public operation to 2022. [^1][^4][^6]

## Layers Classification (L1-L7)

Based on the IndiaStack layers framework, ONDC occupies:

| Layer | Classification | ONDC's Role |
|---|---|---|
| **L1 — Vision & Policy** | Government policy | DPIIT initiative; Advisory Council; goals of democratising e-commerce and raising e-commerce penetration [^1][^7] |
| **L2 — Regulation** | Regulatory framework | Governed by general law — Consumer Protection Act 2019, E-Commerce Rules 2020, DPDP Act 2023 — plus contractual Network Policy; **no dedicated statute** [^6][^15] |
| **L3 — Digital Rails / Infrastructure** | Core infrastructure | ONDC registry + Beckn Gateways; the switching fabric connecting all participants [^4][^10] |
| **L4 — APIs & Protocols** | Open standards | Beckn Protocol base layer + ONDC network extension specifications (certified open APIs) [^9][^10] |
| **L5 — Applications** | End-user apps | Buyer apps (Paytm, Magicpin, Pincode, Namma Yatri, Ola), seller apps (Bitsila, Mystore, Shiprocket), logistics apps [^4][^5] |
| **L6 — Use Cases** | Sectoral applications | Retail, food & beverages, grocery, fashion, mobility/ride-hailing, metro & bus ticketing, logistics, credit, investments, tourism, agriculture/FPOs, B2B [^2][^5] |
| **L7 — Analytics & Intelligence** | Data & insights | Anonymised aggregated network metrics via gateways; seller scoring/badging; network reputation systems [^4][^6] |

ONDC is distinctive as an **L3-L4 construct** — its public-good core is the protocol and switching layer, while all user experience is deliberately left to private market participants. The state builds the rails; commerce happens on top.

## Regulatory Framework

ONDC operates without a dedicated statute — a deliberate design choice and the network's most-cited governance gap. [^6]

### Applicable Law

- **Consumer Protection Act, 2019 and Consumer Protection (E-Commerce) Rules, 2020**: Every buyer app is an "e-commerce entity" with statutory duties — grievance officer, acknowledgment of complaints within 48 hours, resolution within 30 days. The rules bind each buyer app directly; the network underneath changes nothing about those duties. [^14][^16]
- **Digital Personal Data Protection Act, 2023 (DPDP)**: Buyer apps, seller apps and ONDC itself are data fiduciaries for personal data they process. The DPDP Rules, 2025 (notified 13 November 2025) operationalise consent, notice and erasure duties across the network — materially strengthening a baseline that did not exist when the network launched. [^15]
- **Information Technology Act, 2000**: Intermediary framework and unlawful-content obligations for all apps. [^6]
- **FDI policy**: Marketplace inventory/ownership rules continue to apply to each participant individually. [^17]

### Contractual Governance

- **ONDC Network Policy**: The binding contract between ONDC and every Network Participant, organised into chapters covering participant obligations, Issue & Grievance Management (Ch. 6), Network Data Governance (Ch. 7) and Technology Governance (Ch. 8). ONDC can certify, suspend or terminate participants for breach. [^9]
- **Certified integration**: Participants must pass certification of their protocol adapters before going live. [^10]

### The Governance Gap

The relationship between the Government and ONDC **is not defined by any act of Parliament**. As a private Section 8 company, ONDC falls **outside the ambit of the Right to Information Act, 2005**, and citizens cannot enforce fundamental rights against it through writ petitions under Articles 32/226 as they could against a state authority — while ONDC simultaneously exercises quasi-regulatory powers over participants (certification, suspension, termination). Internet Freedom Foundation and others have flagged this accountability gap as the network's central structural concern. [^6]

## Citizen Rights Analysis

**For buyers:**
- Freedom of choice: any buyer app can reach any network seller — reducing vendor lock-in and enabling price comparison across apps [^3]
- Statutory consumer protections travel with the buyer app (48-hour acknowledgment, 30-day resolution, grievance officer) [^14][^16]
- Network-level escalation to ONDC and ultimately online dispute resolution, with courts always available [^13][^14]

**For sellers:**
- One onboarding through any seller app makes the seller discoverable across all buyer apps — lower customer-acquisition cost than joining each platform separately [^1][^3]
- Commissions on the network have been reported at ~3–5% versus platform commissions several multiples higher, though incentive schemes that subsidised early growth have been progressively cut (up to 75% from Q2 FY2025) [^14][^18]
- **Weaker side of the ledger:** a seller delisted by the network or an app has no independent statutory appeal — remedies run through ONDC's own IGM/contract machinery, and IFF notes ONDC "remains silent" on remedies for delisted sellers. [^6]

**Rights framing:** ONDC redistributes market power toward sellers and multi-homed buyers, but the rights architecture protecting participants is contractual, not constitutional. The citizen's enforceable rights are those under general consumer and data-protection law against each private participant — not rights against the network itself. [^6][^15]

## Privacy Implications

1. **Data siloing by design**: The ONDC strategy paper specifies that buyer personal data stays with the buyer app and seller competitive data stays with the seller app; ONDC does not mandate transaction-level data sharing from participants — a commitment made by the Advisory Council in August 2022. [^6][^9]
2. **But ONDC can still hold personal data**: The Network Data Governance Policy acknowledges ONDC may receive or collect personal data in the course of operations; anonymised aggregate metrics are published network-wide, and re-identification from "anonymised" datasets (pincode + date-of-birth + gender-style combinations) is a documented risk. [^6]
3. **Fragmented consent**: A single order can touch a buyer app, a seller app, a logistics provider and a payment provider. Each is a separate data fiduciary; the buyer's meaningful consent and the ability to exercise deletion rights across the full chain is administratively harder than on a single platform. [^6][^15]
4. **Same-entity both sides**: Large incumbents can operate buyer-side and seller-side apps (and logistics) simultaneously, recreating data-combination practices the network design meant to prevent. [^6]
5. **Changed baseline**: Much critical analysis (including IFF's) predates the DPDP Act's operation. With the DPDP Rules in force since November 2025, participants now have enforceable consent, notice and erasure obligations — the strongest privacy safeguard the network has had. Enforcement capacity, not law, is now the binding constraint. [^15]

## Safeguards

- **Network Policy obligations**: Participants must ensure confidentiality and user privacy in transactions, prohibit unlawful content, and cooperate in complaint resolution [^9]
- **Certified, standardised APIs**: Only certified protocol implementations go live, reducing ad-hoc data handling [^10]
- **Consent-based data exchange**: Transaction-data policies are specified as consent-anchored and purpose-limited, evolving through network policy revisions [^6]
- **Payment Assurance Program**: ONDC operates a payment-protection programme for transactions on the network [^14]
- **IGM + ODR**: Structured, time-bound issue resolution with an online-dispute-resolution backstop [^13]
- **DPDP compliance**: Post-November 2025, statutory consent, notice, grievance and erasure rights apply to every fiduciary in the chain [^15]

## Complaints & Grievance Redressal

ONDC's grievance architecture is two-tiered, on top of each app's own statutory duties:

**Step 1 — Buyer App first.** Every complaint starts with the app the order was placed on. By law the buyer app must acknowledge within **48 hours** and resolve within **30 days** under the Consumer Protection (E-Commerce) Rules, 2020. [^14]

**Step 2 — Escalate to ONDC.** If the buyer app stalls, the buyer (or seller) escalates at ONDC's grievance portal (portal.ondc.org/complaints), quoting the buyer-app ticket number; status is trackable online. [^14]

**Network-level IGM.** Between businesses, ONDC's Issue & Grievance Management framework covers buyer/seller vs network participant, participant vs participant, and participant vs ONDC disputes. Issues first go through automated resolution, then to Grievance Redressal Officers, then to arbitration through ONDC's ODR service providers — with the parties' right to approach courts preserved at every stage. [^13]

**Escalation beyond the network:** Consumer commissions under the Consumer Protection Act, 2019 remain available against the specific e-commerce entity (the buyer app, seller app or logistics provider — whoever caused the harm), since ONDC disclaims being party to the transaction. [^6][^16]

## Prime References

[^1]: https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=2090097 (PIB, Ministry of Commerce & Industry — "Revolutionizing Digital Commerce: The ONDC Initiative", 4 January 2025)
[^2]: https://www.ondc.org/pages/about-us.html (ONDC official — About, timeline, board, 500M milestone 25 July 2026)
[^3]: https://www.ibm.com/think/topics/ondc (IBM — What Is ONDC)
[^4]: https://en.wikipedia.org/wiki/Open_Network_for_Digital_Commerce (Wikipedia — ONDC, Beckn backend, investor details)
[^5]: https://ondc.org (ONDC official — live network counters)
[^6]: https://internetfreedom.in/ondc-an-explainer (Internet Freedom Foundation — ONDC: An Explainer, 10 March 2023)
[^7]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=1732949 (PIB — Advisory Council constitution, July 2021)
[^8]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2215035 (PIB — Department of Posts first ONDC order as LSP, 15 January 2026)
[^9]: https://resources.ondc.org/ondc-network-policy (ONDC Network Policy — IGM, Data Governance, Technology Governance chapters)
[^10]: https://github.com/ONDC-Official/protocol-network-extension (ONDC-Official — Protocol layered architecture: Beckn base + network extension)
[^11]: https://inc42.com/buzz/ondc-records-21-rise-in-transactions-to-12-mn-in-july (Inc42 — July 2026 volumes, seller/city counts)
[^12]: https://www.moneycontrol.com/news/business/ondc-crosses-500-million-transactions-as-govt-backed-network-expands-beyond-e-commerce-into-mobility-public-services-13998058.html (Moneycontrol — 500M milestone, FY23→FY26 trajectory, active merchants)
[^13]: https://ondc-static-website-media.s3.ap-south-1.amazonaws.com/ondc-website-media/downloads/governance-and-policies/a.ONDC%27s%20IGM-%20Explainer-%20v1.0.pdf (ONDC — Issue & Grievance Management explainer)
[^14]: https://www.ondc.org/pages/complaint.html (ONDC official — Complaints: 48-hour/30-day rules, escalation portal)
[^15]: https://www.meity.gov.in/data-protection-framework (MeitY — Digital Personal Data Protection framework; DPDP Act 2023 and Rules 2025)
[^16]: https://consumeraffairs.nic.in (Ministry of Consumer Affairs — Consumer Protection Act 2019 and E-Commerce Rules 2020)
[^17]: https://dpiit.gov.in (DPIIT — FDI policy for e-commerce marketplace entities)
[^18]: https://bfsi.economictimes.indiatimes.com/news/fintech/ondc-monthly-transactions-hit-10-million-in-june-report/111571725
[^19]: https://economictimes.indiatimes.com/tech/technology/ondc-monthly-orders-hit-record-12-million-in-july/articleshow/112270111.cms
