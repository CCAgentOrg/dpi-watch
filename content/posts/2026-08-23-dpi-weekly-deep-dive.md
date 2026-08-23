---
title: "DPI Weekly Deep Dive — The UPI Pricing Reckoning: From Zero MDR to the ₹20,000 Crore Question | Week of August 17–23, 2026"
date: 2026-08-23T09:00:00+05:30
draft: false
tags: ["DPI", "Digital India", "Deep Dive", "Weekly", "Analysis", "UPI", "Payments", "NPCI", "MDR", "Pricing", "Policy", "RBI"]
categories: ["Weekly Deep Dive"]
description: "After a decade of zero-MDR, Parliament has cleared the path to charge for UPI. This week's deep dive examines the economics, the legislation, the politics, and what it means for 300 million Indians."
image: ""
---

# DPI Weekly Deep Dive — The UPI Pricing Reckoning: From Zero MDR to the ₹20,000 Crore Question | Week of August 17–23, 2026

## Executive Summary

This week, India's most consequential digital public infrastructure debate crystallised into legislative fact. On August 10, Parliament passed the Taxation and Other Laws (Amendment) Bill, 2026, amending Section 10A of the Payment and Settlement Systems Act, 2007. The amendment grants the government power to designate which electronic payment modes will be exempt from charges — and, by implication, which will not be. [^1]

This is not a new UPI tax on consumers. Finance Minister Nirmala Sitharaman has been explicit: person-to-person (P2P) transfers will remain free, and consumers will face no direct charges. [^2] But the amendment opens the door to a Merchant Discount Rate (MDR) on select high-value person-to-merchant (P2M) UPI transactions — a fee merchants pay to the banks and payment processors that handle their digital payments. The proposed rate of 0.3% on transactions above ₹2,000 would mark the first time in six years that UPI carries a price tag. [^3]

The debate this week has been intense and revealing. The BBC ran a major feature calling it "the bill" — the moment India's digital payments miracle meets fiscal reality. [^4] Bloomberg published an opinion piece arguing that UPI needs reform driven by domestic economics, not US pressure. [^5] The Indian Express carried a compelling argument by former Telecom Secretary R.S. Sharma that the savings UPI generates for the exchequer — in reduced currency printing, lower cash-handling costs, and increased tax compliance — should fund the system, not MDR on merchants. [^6] And Forbes India documented the growing rift between large merchants who can absorb a 0.3% charge and small merchants for whom even a nominal fee erodes already thin margins. [^7]

The core tension is simple: India built the world's largest real-time payment system on the premise that free drives adoption. Now that adoption has been achieved — 23.66 billion transactions in July 2026, worth ₹29.88 lakh crore [^8] — the question is whether free is sustainable. The answer, as this analysis will show, depends entirely on who you ask and what costs you count.

## The Story in Depth

### Context: How UPI Got to Zero

When UPI launched on April 11, 2016, it operated under the same MDR framework as other digital payment systems. Banks and payment service providers charged merchants a fee — typically 0.25% to 1% — for processing digital payments. This was standard practice globally: card networks charge 1-3%, and most instant payment systems either levy interchange fees or recover costs through banking relationships.

In January 2020, the government mandated zero MDR on UPI and RuPay debit card transactions, motivated by the goal of accelerating digital payment adoption among small merchants and everyday consumers. [^9] The policy was unambiguous in its intent: remove the price barrier, let behavioural economics do the rest. It worked. UPI transaction volumes grew from 1.2 billion in FY2017-18 to 242 billion in FY2025-26 — a 200x increase in under a decade. [^10] Transaction value surged from ₹0.07 lakh crore to over ₹314 lakh crore in the same period. [^11]

To compensate banks for the revenue foregone, the government introduced the UPI and RuPay incentive scheme. This paid banks 0.15% on low-value merchant transactions (up to ₹2,000). The scheme peaked at ₹3,631 crore in FY2023-24, but has since been in structural decline. For FY2026-27, the Union Budget allocated ₹2,000 crore — nearly five times the previous year's budget estimate of ₹437 crore, but still far below the system's actual running costs. [^12]

### What Happened This Week

The legislative change itself is small but significant. The Taxation and Other Laws (Amendment) Bill, 2026, passed by Parliament on August 10, amends Section 10A of the Payment and Settlement Systems Act, 2007. Previously, Section 10A prohibited charges on prescribed payment systems. The amendment inverts this logic: instead of prohibiting charges, the government now has the power to *designate* which payment methods will be protected from charges. Everything else becomes chargeable. [^1]

This is a subtle but important shift. Under the old framework, the default was free, and the government had to affirmatively act to allow charges. Under the new framework, the government must affirmatively act to maintain free status for any given payment method. It gives the executive flexibility to introduce a tiered MDR structure without returning to Parliament for each adjustment.

The mechanism for determining the actual MDR rates falls to the UPI and Services Steering Committee, led by NPCI. [^13] The Department of Financial Services (DFS) has indicated it is considering two options: (1) restoring MDR for transactions or merchants above a specified threshold, or (2) introducing multi-level incentives and phasing out government support over several years. [^14] The Payments Council of India has proposed a 0.3% MDR on large merchants, which the Standing Committee on Finance has endorsed as a starting point. [^15]

### Why It Matters

The ₹20,000 crore question — literally. Industry and expert estimates put the annual cost of running UPI at ₹20,000 crore, shared between banks, NPCI, and payment service providers. [^7] Against this, the government's ₹2,000 crore incentive covers roughly 10%. The Parliamentary Standing Committee on Finance, in its 32nd Report tabled in March 2026, flagged this gap starkly: the incentive scheme covers only about 11% of the sector's real expenses and 14% of potential MDR collections. [^15]

But the framing of "cost" matters enormously. Economist Ajit Ranade has argued that UPI's costs should be charged to the RBI, noting that ₹20,000 crore would be barely 7% of the central bank's annual dividend to the Union government. [^7] R.S. Sharma, former Secretary of the Department of Telecommunications and former CEO of NPCI, made an even more fundamental argument in the Indian Express this week: the government should fund UPI from the savings it generates. Cash handling, currency printing, and the efficiency gains from digital payments represent a fiscal dividend that far exceeds the system's operating costs. [^6]

This argument has merit. The RBI's own data on currency management costs, combined with the tax-base widening that digital payment trails enable, suggests UPI's net fiscal impact is already positive. The question is not whether UPI pays for itself — it almost certainly does — but whether those savings are visible and allocable enough to justify continued exchequer funding.

## Technical Deep Dive

### The Volume-Value Paradox

The most important technical detail in this debate is the structure of UPI transactions themselves. IIM Bangalore's analysis of NPCI data reveals a stark dual-use pattern: 86% of P2M transactions are under ₹500, while only 4% of transactions exceed ₹2,000 — yet those 4% account for 66% of total P2M value. [^16]

This has a direct bearing on the MDR debate. If MDR is applied only to transactions above ₹2,000, it would affect roughly 4% of transactions but capture the bulk of value. The estimated revenue potential at a 0.3% MDR on high-value P2M would be substantial — the Standing Committee estimated potential MDR collections at roughly ₹14,000 crore, against which the ₹2,000 crore incentive covers just 14%. [^15]

But there is a catch. The average UPI ticket size has been declining — from over ₹1,600 in early 2023 to approximately ₹1,314 by end of 2025. [^17] Worldline's India Digital Payments Report for CY2025 recorded a further 8.6% year-on-year decline in average transaction size. This means UPI is increasingly used for micro-payments: chai, vegetables, auto-rickshaws, parking. [^18] These are precisely the transactions that any MDR framework would exempt. The revenue potential of a high-value MDR is real but depends on the threshold staying relevant as average ticket sizes shrink.

### AI and Infrastructure Costs

The cost argument is also evolving. NPCI announced FiMI (Finance Model for India) in February 2026 — a domain-specific language model that powers UPI's Help Assistant, handling payment queries and dispute resolution in four languages. [^19] The RBI Innovation Hub's MuleHunter.AI, adopted by 23 banks with 95% detection accuracy at Canara Bank, blocks roughly 20,000 mule accounts per month. [^19] By June 2026, the Indian Cyber Crime Coordination Centre (I4C) had shared information on 3.208 million first-layer mule accounts with banks, preventing suspicious transactions worth ₹25,698 crore. [^20]

These AI systems are not cheap to build or run. But they exist because UPI's scale makes manual oversight impossible. At 763 million transactions per day (July 2026 average), even a 0.01% fraud rate would mean 76,300 fraudulent transactions daily. The infrastructure costs are real, growing, and directly tied to the system's scale.

### The Offline Frontier

NPCI is developing UPI Lite 'tap and pay' using NFC for transactions up to ₹2,000 without internet connectivity, targeted for launch by end of 2026. [^21] This addresses a real problem: a LocalCircles survey this week found that 8 in 10 users face disruption in digital payments due to mobile internet issues. [^22] Offline payments add another infrastructure layer — secure element provisioning, settlement reconciliation without real-time connectivity, and dispute resolution for delayed settlements — all of which add to costs.

## Government Perspective

The government's position has been carefully calibrated. The official line, reinforced by a BJP social media post this week, is that "consumers will not have to pay charges on UPI transactions" and that MDR, if introduced, will apply only to a limited set of merchant transactions above a specified threshold at a nominal rate far lower than card MDR. [^2]

Behind this public reassurance lies a genuine policy dilemma. The Standing Committee on Finance, chaired by BJP leader Bhartruhari Mahtab, has been unequivocal: the current zero-MDR model is fiscally unsustainable and constrains long-term infrastructure investment. [^15] The Committee warned that delays in implementing a tiered MDR framework would leave payment service providers dependent on inadequate government support.

The DFS, in its response to the Committee, signalled it is assessing both options — a threshold-based MDR and a phased incentive reduction. [^14] Neither is politically easy. A UPI charge, even if technically levied on merchants, is easily framed as a betrayal of the "free UPI" promise. The BJP's own social media team felt compelled to issue clarifications this week, suggesting the political sensitivity is real. [^2]

The incentive budget trajectory tells the real story. From ₹1,389 crore in FY2021-22 to ₹3,631 crore in FY2023-24 (peak), then crashing to ₹437 crore (budgeted) in FY2025-26 before being bumped to ₹2,000 crore for FY2026-27. [^12] This is not a smooth fiscal glide path — it is a zigzag that reflects political calculation as much as economic reasoning. The government wants to signal commitment to digital payments while managing its own fiscal constraints.

## Citizen Impact

For the vast majority of UPI users, nothing changes. The proposed MDR framework explicitly exempts P2P transfers and small-value P2M transactions (below ₹2,000). Given that 86% of P2M transactions are under ₹500, the overwhelming majority of everyday UPI usage remains untouched. [^16]

But the impact on merchants is asymmetric. Large merchants — organised retail, e-commerce platforms, chain restaurants — can absorb a 0.3% MDR without breaking stride. Their margins are healthy, their digital payment volumes are high, and they already pay MDR on card transactions (1-2% for credit cards, 0.4-0.9% for debit cards). A 0.3% UPI MDR would still be the cheapest option. [^7]

Small merchants are a different story. A vegetable vendor doing ₹50-100 transactions isn't affected because those fall below the threshold. But a neighbourhood electronics shop, a furniture store, or a medical supply shop that regularly processes payments above ₹2,000 will feel the pinch. These merchants operate on thin margins — often 5-10% — and a 0.3% charge on their payment flow is not trivial. [^7]

The deeper concern is behavioural. One of UPI's most powerful adoption drivers has been its absolute simplicity and zero friction. The moment a merchant sees a line item called "UPI charges" on their bank statement, even if small, it creates a psychological incentive to prefer cash — precisely the behaviour the zero-MDR policy was designed to eliminate. The BBC's feature this week quoted small merchants who said they would consider raising prices or steering customers toward cash if UPI became chargeable. [^4]

There is also the pass-through question. While MDR is technically charged to merchants, not consumers, anyone who has watched Indian kirana stores add a ₹2-5 "card charge" to small transactions knows that costs flow downhill. A formal UPI MDR on large transactions could trigger informal pass-through charges across the board, eroding consumer trust in the system's "free" promise.

## Global Context

India is not alone in grappling with instant payment system pricing. The comparison is instructive.

**Brazil's PIX**, launched in 2020 by the Central Bank of Brazil, offers a useful parallel. PIX adopted a tiered model: person-to-person transfers are free for individuals, but merchants pay a small fee to receiving institutions. The model has been sustainable, and PIX has grown to over 140 million users processing billions of transactions monthly. [^23]

**The European Union's SEPA Instant Credit Transfer** mandates that all payment service providers offer instant payments by January 2025, but allows banks to charge for the service. Most EU banks do levy fees for instant transfers, typically €0.10-0.50 per transaction. [^24]

**Sweden's Swish** is free for P2P transfers but charges merchants, with the fee structure set by the receiving bank. The system remains profitable and widely used. [^25]

The common pattern is clear: free for individuals, chargeable for merchants, with the state playing a smaller direct funding role than India has. India's zero-MDR experiment was uniquely aggressive in its scope and duration. The global consensus suggests some form of merchant pricing is normal and compatible with high adoption.

Bloomberg's Andy Mukherjee argued this week that India's UPI reform should be driven by domestic economics, not external pressure from US firms lobbying for market access. [^5] This is a fair point. The UPI pricing debate predates any international pressure and is rooted in genuine fiscal and infrastructure sustainability concerns.

The BRICS Digital Public Infrastructure Repository proposed by India at this week's BRICS ICT meetings in Pune adds another dimension. [^26] India is positioning UPI as a model for other developing nations — but those nations will want to understand the full cost structure, not just the adoption numbers. A transparent, sustainable pricing model would strengthen, not weaken, India's DPI export narrative.

## Looking Ahead

Several developments are worth watching in the coming weeks:

1. **DFS Notification on Protected Payment Modes**: The Department of Financial Services must issue a notification specifying which payment modes continue to receive statutory protection from charges. This is the critical next step — without it, the legislative amendment is just an enabling provision. [^13]

2. **NPCI Steering Committee's MDR Framework**: The UPI and Services Steering Committee will determine the actual MDR structure — the threshold, the rate, any merchant categorisation, and the revenue-sharing arrangement between banks, NPCI, and PSPs. [^13]

3. **Incentive Scheme Trajectory**: The FY2026-27 allocation of ₹2,000 crore will be watched closely. If actual spending falls short — as it did in FY2025-26 when only ₹437 crore was budgeted — it will signal that the government is already winding down direct support, making MDR implementation more urgent. [^12]

4. **RBI's Fraud-Prevention Measures**: The RBI's proposed one-hour cooling-off window for UPI transfers above ₹10,000, and the scaling of MuleHunter.AI to more banks, will add to the infrastructure cost base — strengthening the case for sustainable funding. [^20]

5. **Merchant and Consumer Behaviour**: The most important variable is whether a 0.3% MDR on high-value transactions causes any measurable shift back to cash. If it doesn't — and the evidence from Brazil and the EU suggests it won't, if the threshold is well-calibrated — the pricing debate will fade. If it does, the government will face an uncomfortable choice between fiscal sustainability and adoption continuity.

The fundamental insight of this week is that India's UPI pricing debate is not really about pricing. It is about how a democracy funds public digital infrastructure. The answer will shape not just UPI's future, but the template for every DPI layer that follows — ONDC, Account Aggregator, DigiLocker, and the platforms yet to be built.

## Sources

- [1] Parliament passes Taxation and Other Laws (Amendment) Bill, 2026 — [PIB](https://www.pib.gov.in/)
- [2] BJP clarification on UPI charges — [BJP4India / Facebook](https://www.facebook.com/BJP4India/posts/1535717955269152)
- [3] UPI Merchant Discount Rate: MDR of 0.3% on Large Transactions — [Chetan Bharat / Current Affairs](https://currentaffairs.chetanbharat.com/upi-merchant-discount-rate-upsc)
- [4] India built a digital payments miracle. Now comes the bill — [BBC News](https://www.bbc.com/news/articles/c8xnwqe00v1o)
- [5] India's UPI Needs Reform, Not US Pressure — [Bloomberg Opinion](https://www.bloomberg.com/opinion/articles/2026-08-20/india-s-upi-needs-reform-not-us-pressure)
- [6] Keep UPI free, and fund it from the savings it generates — R.S. Sharma, [Indian Express](https://indianexpress.com/article/opinion/columns/upi-payments-free-fund-savings-generates-10844124)
- [7] Why UPI MDR's Return Could Widen the Gap Between Large and Small Merchants — [Forbes India](https://www.forbesindia.com/article/news/deep-dive/mdr-reintroduction-ignites-small-vs-big-player-debate/2997348/1)
- [8] UPI processes 23.66 billion transactions in July 2026 — [NPCI data via Economic Times](https://m.economictimes.com/gff-2026-as-upi-scales-fraud-detection-faces-a-new-ai-challenge/articleshow/133403719.cms)
- [9] Zero MDR on UPI and RuPay (January 2020 notification) — [RBI / DFS historical records](https://www.digitalindia.gov.in/initiative/unified-payment-interface-upi)
- [10] UPI transaction volume growth: 20 million (FY17) to ~242 billion (FY26) — [NPCI via LinkedIn / Arjun Vaidya](https://www.linkedin.com/posts/arjunvaidya_ive-come-back-from-a-2-week-holiday-and-activity-7488820245823037440-7QYf)
- [11] UPI transaction value exceeds ₹314 lakh crore in FY 2025-26 — [Millennium Post](https://www.millenniumpost.in/business/upi-transaction-value-exceeds-rs-314-lakh-crore-in-fy-2025-26-658127)
- [12] Parliamentary panel calls for MDR on UPI; incentive scheme allocation details — [Inc42](https://inc42.com/buzz/parliamentary-panel-calls-for-mdr-on-upi-to-ensure-sustainability)
- [13] FinTales Edition 48: UPI Monetisation — [Ikigai Law](https://www.ikigailaw.com/article/693/fintales-edition-48---upi-monetisation-and-revolving-credit-rules)
- [14] Government weighs MDR on select UPI payments — [National Herald India](https://www.nationalheraldindia.com/business/government-weighs-mdr-on-select-upi-payments-to-support-ecosystem)
- [15] Parliamentary Standing Committee on Finance, 32nd Report (March 2026) — [Times of India](https://timesofindia.indiatimes.com/business/india-business/mdr-on-upi-soon-parliamentary-panel-recommends-expeditious-introduction-on-high-value-transactions/articleshow/133204726.cms)
- [16] India's UPI usage: volume vs value dilemma — [IIM Bangalore](https://www.iimb.ac.in/sites/default/files/2025-09/India-UPI-usage-volume-dilemma.pdf)
- [17] Active UPI QR Codes Cross 731 Million; average transaction size falls — [ClearingPost / Worldline](https://clearingpost.com/insights/worldline-cy2025-upi-qr-merchant-growth)
- [18] UPI's 10-year journey: from innovation to infrastructure — [NPCI / PIB](https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=)
- [19] How UPI Processes 228 Billion Transactions a Year (FiMI, MuleHunter.AI) — [Medium / DKMH](https://medium.com/@dkmh2822/how-upi-processes-228-billion-transactions-a-year-the-big-data-story-behind-indias-payment-fa6eb6aba360)
- [20] I4C mule account data; fraud prevention — [The Financial World](https://www.thefinancialworld.com/wp-content/uploads/2026/08/22-August-FW-Delhi-Edition.pdf)
- [21] Offline UPI Payments 'Tap and Pay' Coming Soon — [Namma Kudla English](https://www.nammakudlaenglish.com/offline-upi-payments-tap-and-pay-coming-soon)
- [22] 8 in 10 users face disruption in digital payments — [LocalCircles](https://www.localcircles.com/a/press/page/transaction-disruption-telecom-survey)
- [23] Brazil's PIX payment system model — referenced via [BIS Instant Payment Systems report](https://www.bis.org/)
- [24] SEPA Instant Credit Transfer Scheme — [European Payments Council](https://www.europeanpaymentscouncil.eu/)
- [25] Swish merchant pricing — [Swedish Bankers' Association](https://www.swish.nu/)
- [26] 7th BRICS ICT Working Group: India presents DPI Repository concept note — [PIB](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2300968&reg=48&lang=1)
