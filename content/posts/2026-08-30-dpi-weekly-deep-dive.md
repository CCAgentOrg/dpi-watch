---
title: "DPI Weekly Deep Dive — UPI at 10: From Domestic Juggernaut to BRICS Digital Rail | Week of August 24–30, 2026"
date: 2026-08-30T09:00:00+05:30
draft: false
tags: ["DPI", "Digital India", "Deep Dive", "Weekly", "Analysis", "UPI", "BRICS", "CBDC", "Cross-Border Payments", "NPCI", "International Expansion"]
categories: ["Weekly Deep Dive"]
description: "On UPI's tenth anniversary, India is leveraging its domestic payment juggernaut to build a cross-border digital payment architecture for the BRICS bloc — linking fast payment systems and CBDCs in a bid to reshape global settlement rails."
image: ""
---

# DPI Weekly Deep Dive — UPI at 10: From Domestic Juggernaut to BRICS Digital Rail | Week of August 24–30, 2026

## Executive Summary

On August 25, 2026, the Unified Payments Interface completed a decade of operations — transforming from an experimental inter-bank switch processing 373 transactions in its first month to the world's largest real-time payment system, now handling 23.66 billion transactions a month. The milestone week coincided with a strategic inflection point: RBI Governor Sanjay Malhotra publicly confirmed that BRICS nations are actively discussing linkages between their fast payment systems — including India's UPI, Brazil's Pix, and Russia's Mir — alongside their respective Central Bank Digital Currencies (CBDCs).

The convergence is deliberate. India hosts the 18th BRICS Summit in New Delhi on September 12–13, and the cross-border digital payments agenda has emerged as one of the bloc's most concrete deliverables. With 23 MoUs signed for DPI cooperation, 11 countries now accepting UPI, and the Finance Minister's September 1–2 pre-summit meeting set to hammer out practical mechanisms, this is not aspirational rhetoric — it is an infrastructure build-out in progress.

The takeaway: UPI's domestic success was always a means to an end. The end is a globally interconnected, non-dollar-denominated settlement architecture where India's payment rails become the interoperable backbone for emerging economies.

## The Story in Depth

### Context

The Unified Payments Interface was launched on August 25, 2016, by the National Payments Corporation of India (NPCI) under the regulatory oversight of the Reserve Bank of India. Built as an open API layer over the existing Immediate Payment Service (IMPS), UPI introduced a single, interoperable interface for peer-to-peer and peer-to-merchant payments through virtual payment addresses (VPAs) and QR codes.

The early years were slow. In FY 2016–17, UPI processed just 1.78 crore (17.8 million) transactions worth ₹0.07 lakh crore. The system competed with established mobile wallets (Paytm, MobiKwik) and the inertia of cash. Two developments changed the trajectory: the government's demonetisation of high-value currency notes in November 2016, which created an acute demand for digital alternatives, and the subsequent zero-MDR (Merchant Discount Rate) policy that made UPI the cheapest acceptance method for merchants.

By FY 2025–26, annual transaction volume had surged to 24,162 crore — a 13,000-fold increase over a decade. Transaction value reached approximately ₹314 lakh crore, representing a more than 4,000-fold rise. The IMF has formally acknowledged UPI as the world's largest real-time payment system by transaction volume, accounting for roughly 49% of all global real-time digital transactions. India now processes more real-time digital transactions than the United States, the European Union, and China combined.

### What Happened This Week

The week of August 24–30, 2026, marked three converging developments:

**1. UPI's 10th Anniversary (August 25).** Prime Minister Modi described it as "a major turning point in India's digital payments journey." The Ministry of Finance released comprehensive statistics: 741 banks live on UPI (up from 21 at launch), 55.49 crore onboarded users, and a record July 2026 figure of 2,365.8 crore transactions worth ₹29.87 lakh crore. NPCI data showed July 2026 as the highest monthly volume in UPI's history. The P2M (Person-to-Merchant) segment has decisively overtaken P2P, reflecting deep merchant penetration — particularly in tier-2 and tier-3 cities.

**2. BRICS Cross-Border Payment Linkages Confirmed (August 26).** Speaking at the annual FIBAC conference, RBI Governor Sanjay Malhotra stated: "There is a lot of work which is being done over there. Various methods, various options are on the table, but it is still at the discussion stage, including CBDC and linkages of fast payment systems." This was the first public confirmation from the RBI governor that UPI-Pix-Mir interconnection is under active discussion. The statement aligned with India's January 2026 proposal — reported by Reuters — to place CBDC interconnection on the BRICS summit agenda.

**3. BRICS Summit Preparations Intensify (August 27–29).** Government sources confirmed that 10 partner nations have been invited to the September 12–13 summit. The finance track meeting, chaired by Finance Minister Nirmala Sitharaman on September 1–2, will focus on practical mechanisms for cross-border digital payments and local currency settlements. The BRICS Think Tank Network for Finance held its annual conference on August 25 in New Delhi. The External Affairs Ministry highlighted that India has signed 23 MoUs with countries for cooperation on India Stack/DPI.

### Why It Matters

The domestic UPI story is well-documented. What makes this week significant is the explicit coupling of UPI's proven domestic scale with a geopolitical infrastructure play.

Currently, cross-border retail payments between BRICS nations typically flow through the SWIFT network, correspondent banking chains, and dollar intermediary clearing. The cost of a retail cross-border remittance averages 4–6% globally, according to the World Bank — and can exceed 10% for certain BRICS corridors. India's proposition is straightforward: replace this with direct system-to-system links between national fast payment rails.

If UPI-Pix (India-Brazil) interoperability becomes operational, a Brazilian importer could pay an Indian exporter in real time by scanning a UPI QR code, with settlement occurring in local currencies through pre-arranged FX protocols. No SWIFT message. No correspondent bank. No 3–5 day settlement window. The proposed CBDC layer adds another option: bilateral digital currency settlement that bypasses conventional forex markets entirely.

This is not purely economic. With 85% of intra-BRICS trade now settled outside the US dollar (up from 65% two years ago), and Russia and China already at 90%, the digital payments interconnection is part of a broader strategic decoupling from dollar-denominated infrastructure. India's framing is careful — the RBI has explicitly stated its efforts are "not aimed at promoting de-dollarisation" — but the infrastructure effect is the same.

## Technical Deep Dive

### UPI's Architecture

UPI operates as a central switch operated by NPCI. The architecture follows a hub-and-spoke model:

- **Payment Service Providers (PSPs):** Banks and licensed third-party apps (PhonePe, Google Pay, Paytm, BHIM) that provide the user-facing interface. There are currently 741 live banks.
- **NPCI Central Switch:** Routes transactions between PSPs using ISO 20022 messaging standards. Handles authentication, settlement, and reconciliation.
- **Remitter and Beneficiary Banks:** The actual account-holding institutions that debit and credit accounts.

A UPI transaction flow: User initiates payment via VPA/QR → PSP sends request to NPCI switch → NPCI validates and routes to beneficiary's PSP → Beneficiary bank credits the account → NPCI facilitates settlement between banks through the RBI's settlement window.

### International Linkage Model

NPCI International Payments Limited (NIPL), a wholly-owned subsidiary established in April 2020, handles international expansion. The linkage model varies by country:

- **Bilateral QR Linkage (Nepal, Sri Lanka, Cambodia, Maldives):** UPI connects to the local national QR standard (Fonepay in Nepal, LankaQR in Sri Lanka, KHQR in Cambodia, Favara in Maldives). Indian tourists scan local QR codes; settlement occurs through banking correspondent arrangements.
- **Network-to-Network Linkage (Singapore):** UPI is linked with PayNow, Singapore's fast payment system operated by MAS. This enables cross-border P2P transfers between Indian and Singaporean bank accounts using mobile numbers.
- **Direct Merchant Integration (UAE, France, Qatar, Mauritius):** NIPL partners with local payment processors (Network International in UAE, Lyra in France) to enable Indian UPI apps at local merchant POS terminals.

### BRICS Interconnection: Proposed Architecture

The BRICS interconnection would operate at a different scale. The proposed model, as discussed in ORF's August 2026 research paper on BRICS SME financing and APTIPLUS's editorial analysis, involves:

1. **Common Technical Standards:** Harmonised messaging protocols (building on ISO 20022) that allow UPI, Pix, and Mir to understand each other's transaction formats.
2. **Bilateral FX Settlement Windows:** Pre-negotiated currency swap lines between BRICS central banks that provide liquidity for real-time currency conversion at the point of transaction.
3. **CBDC Interconnection Layer:** A parallel rail where digital currencies (e-rupee, digital yuan, digital real) can settle directly without conversion to any third currency.

The technical complexity is significant. UPI settles in INR, Pix in BRL, Mir in RUB. Real-time cross-currency settlement requires either a multi-currency clearing house or pre-funded bilateral settlement accounts. The CBDC layer simplifies this — if both sides hold each other's digital currency, settlement is a ledger entry — but requires CBDCs to be fully operational, which none currently are.

### RBI Payments Vision 2028 Alignment

The RBI's Payments Vision 2028, published in March 2026, explicitly prioritises cross-border payment efficiency and a streamlined single-window authorisation process for cross-border payment operators. It also mandates ISO 20022 for FI-to-FI cross-border payments. These regulatory foundations are prerequisites for the BRICS interconnection.

## Government Perspective

For the Modi government, UPI's internationalisation serves multiple objectives simultaneously.

**Economic diplomacy:** Each UPI linkage agreement is bundled into broader DPI cooperation MoUs that cover Aadhaar-style digital identity, DigiLocker document verification, and data exchange platforms. India has signed 23 such MoUs. The 12th BRICS Communications Ministers meeting in Pune this week highlighted that "50% of the world's digital transactions happen in India" — a statistic being weaponised in trade negotiations.

**Export of governance tech:** India Stack Global, launched during the G20 Presidency in 2023, serves as the repository and distribution platform for India's DPI solutions. The Global DPI Repository, hosted under India's G20 legacy, has India contributing the highest number of DPI solutions. Countries like Peru are adopting UPI-like systems; Cambodia and Maldives have linked their national QR codes directly to UPI.

**Summit deliverable:** With the BRICS summit two weeks away, the government needs concrete outcomes. Cross-border payment linkages — unlike geopolitical statements on West Asia or reform of multilateral institutions — are technically achievable and photographable. A UPI-Pix linkage announcement, or a BRICS digital payment interoperability framework, would be a tangible deliverable.

**Revenue model:** The coming introduction of merchant MDR (Merchant Discount Rate) on UPI transactions, as discussed in last week's deep dive, creates a commercial incentive for international expansion. If UPI generates transaction fees domestically, the same fee model can be extended to cross-border corridors — potentially making NIPL a revenue-generating entity rather than a cost centre.

## Citizen Impact

For ordinary Indians, the BRICS payments interconnection has both immediate and medium-term implications.

**Immediate — Cheaper remittances and travel payments:** Indian workers in the UAE, Singapore, and Qatar can already use UPI for merchant payments. Linkages with more countries reduce dependence on expensive money transfer operators. The World Bank estimates that reducing remittance costs to 3% (from the current 5%+ average) would put an additional $4 billion annually in the pockets of Indian diaspora families.

**Medium-term — Cheaper imports and exports:** If an Indian SME can receive payment from a Brazilian buyer directly via a UPI-like interface, the elimination of intermediary banking fees and FX spreads could meaningfully reduce the cost of cross-border trade. This is particularly significant for the estimated 63 million MSMEs in India, many of which are priced out of international trade by payment friction.

**Caveats — Real vs. Paper Infrastructure:** As independent reviews have noted, there is a meaningful gap between announced UPI partnerships and working, merchant-accepted infrastructure. In several countries, UPI "works" only at a limited number of tourist-facing merchants. OTP delivery issues (Indian SIM cards not receiving OTPs abroad) remain a persistent complaint. The BRICS interconnection faces the same adoption gap: a system-to-system linkage is meaningless if merchants and consumers on both sides don't use it.

## Global Context

India is not alone in pushing cross-border fast payment interconnection, but it is the most aggressive.

- **European Union:** SEPA (Single Euro Payments Area) provides a model for standardised cross-border payments within a currency union. The EU is also exploring connections with non-EU instant payment systems.
- **ASEAN:** Six ASEAN payment networks signed an MoU in October 2025 to establish a global standards body for non-card instant retail payments. Bank Indonesia has publicly targeted QRIS-UPI linkage completion by end-2026.
- **Brazil:** Pix, Brazil's instant payment system launched in 2020, processes over 4 billion transactions monthly. A Pix-UPI linkage would connect two of the world's three largest real-time payment systems.
- **China:** The digital yuan (e-CNY) is being positioned for international use, with Chinese commercial banks reportedly allowed to pay interest on digital yuan holdings to boost adoption.

The BIS Innovation Hub's multi-jurisdictional CBDC projects (mBridge, Dunbar, Project Icebreaker) have already demonstrated technical feasibility for cross-border digital currency settlement. India's BRICS proposal builds on these proofs of concept but adds a political-economy dimension: these are not central bank experiments but commitments between heads of state.

## Looking Ahead

**September 12–13 — BRICS Summit, New Delhi:** The primary event to watch. A formal announcement on UPI-Pix-Mir interconnection, or at minimum a framework agreement, would be the most significant outcome. The September 1–2 finance ministers' meeting will preview what is achievable.

**Q4 2026 — UPI QRIS Linkage:** Bank Indonesia's target for connecting Indonesia's QRIS with UPI. If achieved, this would add the world's fourth-largest country (by population) to UPI's international network.

**FY 2026–27 — MDR Introduction:** The reintroduction of merchant fees on UPI, approved by Parliament, will reshape the domestic economics of UPI. How this affects international corridors — where NIPL may charge fees from day one — is worth monitoring.

**2027 — UPI 20 Billion Monthly Transactions:** NPCI's publicly stated target. At current growth rates (30% volume YoY), this is achievable within 12–18 months.

**Beyond 2027 — BRICS Digital Payment Corridor:** If the summit produces a framework, the 2027–2028 period will see technical implementation, pilot corridors, and gradual merchant onboarding. Full operationalisation across all BRICS members is a 3–5 year project.

## Sources

- [PIB: UPI completes 10 glorious years, emerges as world's largest real-time payments platform](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2302664)
- [The Hindu: UPI completes 10 years, clocks nearly 13,000-fold rise in transaction volume](https://www.thehindu.com/business/Economy/upi-completes-10-years-clocks-nearly-13000-fold-rise-in-transaction-volume/article71384088.ece)
- [ET Now: BRICS Summit 2026 — 10 partner nations invited; digital currency, West Asia and trade talks on radar](https://www.etnownews.com/news/brics-summit-2026-10-partner-nations-invited-digital-currency-west-asia-and-trade-talks-on-radar-say-sources-article-155994424)
- [Reuters: India's central bank proposes linking BRICS' digital currencies](https://www.reuters.com/world/india/indias-central-bank-proposes-linking-brics-digital-currencies-sources-say-2026-01-19)
- [CoinDesk: India's central bank proposes a plan to create digital-currency link among BRICS nations](https://www.coindesk.com/markets/2026/01/19/india-s-central-bank-proposes-a-plan-to-create-digital-currency-link-among-brics-nations)
- [The Digital Banker: BRICS looks to build new corridors for cross-border payments](https://thedigitalbanker.com/brics-looks-to-build-new-corridors-for-cross-border-payments)
- [NPCI: UPI Product Statistics](https://www.npci.org.in/product/upi/product-statistics)
- [DD India: UPI at 10 — How India's homegrown payment system transformed the way the country transacts](https://ddindia.co.in/2026/08/upi-at-10-how-indias-homegrown-payment-system-transformed-the-way-the-country-transacts)
- [Cyril Amarchand Mangaldas: UPI Goes Global — The Regulatory Reckoning Ahead](https://corporate.cyrilamarchandblogs.com/2026/05/upi-goes-global-the-regulatory-reckoning-ahead)
- [IBTimes India: UPI now live in 8+ countries; 23 MoUs signed for DPI](https://www.ibtimes.co.in/upi-now-live-uae-singapore-bhutan-nepal-sri-lanka-france-mauritius-qatar-23-mous-signed-897758)
- [ORF: Unlocking SME Financing for BRICS Economies (PDF)](https://www.orfonline.org/public/uploads/upload/20260825102233.pdf)
- [APTIPLUS: Why is BRICS emerging as an engine of global growth?](https://aptiplus.in/daily-editorials/why-is-brics-emerging-as-an-engine-of-global-growth-and-why-is-it-important-for-india)
- [Nifty Trader: India's e-Rupee has crossed ₹28,000 Cr — Now comes the global BRICS test](https://www.niftytrader.in/markets/indias-e-rupee-28000cr-global-brics-test)
- [East Asia Forum: India turns digital infrastructure into soft power](https://eastasiaforum.org/2026/08/06/india-turns-digital-infrastructure-into-soft-power)
- [World Economic Forum: Building security into India's digital public infrastructure](https://www.weforum.org/stories/cybersecurity/security-by-design-india-digital-public-infrastructure)
