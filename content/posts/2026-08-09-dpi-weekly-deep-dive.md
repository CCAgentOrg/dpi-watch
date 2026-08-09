---
title: "DPI Weekly Deep Dive — The End of Zero-MDR? Parliament Opens the Door to UPI Merchant Fees | Week of August 3–9, 2026"
date: 2026-08-09T09:00:00+05:30
draft: false
tags: ["DPI", "Digital India", "Deep Dive", "Weekly", "Analysis", "UPI", "MDR", "Payments"]
categories: ["Weekly Deep Dive"]
description: "2000-word analysis of the Lok Sabha's passage of the Taxation and Other Laws (Amendment) Bill, 2026, which amends the Payment and Settlement Systems Act to enable merchant charges on UPI — and what it means for India's most successful Digital Public Infrastructure."
image: ""
---

# DPI Weekly Deep Dive — The End of Zero-MDR? Parliament Opens the Door to UPI Merchant Fees | Week of August 3–9, 2026

## Executive Summary

On August 6, 2026, the Lok Sabha passed the Taxation and Other Laws (Amendment) Bill, 2026, which includes a consequential amendment to Section 10A of the Payment and Settlement Systems Act, 2007 — the legal provision that has enforced a blanket ban on Merchant Discount Rates (MDR) for UPI and RuPay debit card transactions since January 2020. The amendment does not impose charges immediately; instead, it replaces the blanket prohibition with a framework that empowers the Central Government to notify, by executive order, which electronic payment modes and transaction categories will remain exempt from MDR, and which may attract fees. [^1]

This is arguably the most significant policy shift affecting India's Digital Public Infrastructure since the zero-MDR regime was introduced six years ago. The amendment arrives at a moment when UPI is processing unprecedented volumes — 23.66 billion transactions worth ₹29.88 lakh crore in July 2026 alone — and when the ecosystem's financial sustainability has become a matter of parliamentary and regulatory concern. [^2]

The immediate consumer impact is zero: no MDR has been imposed, no rates have been set, and Finance Minister Nirmala Sitharaman has explicitly clarified that any future MDR would apply to merchants, not end-users. [^3] But the structural change is real. India's most successful DPI layer — the payment rail that handles 85% of digital payments and nearly 50% of global real-time digital payments — is transitioning from a pure adoption-growth model to one that must reckon with its own operational economics. [^4]

## The Story in Depth

### Context: How Zero-MDR Built UPI

When the Reserve Bank of India launched UPI as a pilot on April 11, 2016 with 21 member banks, the system faced an existential question: how do you compete with cash in a country where the marginal cost of a cash transaction is effectively zero? The answer was a bold policy gamble — make UPI free. [^5]

Section 10A of the Payment and Settlement Systems Act, 2007, as reinforced by a CBDT notification in December 2019 under Section 269SU of the Income-tax Act, prohibited banks and system providers from levying any charge on payers or beneficiaries for transactions through UPI and RuPay debit cards. This zero-MDR policy was not merely a subsidy; it was the foundational design choice that allowed UPI to scale from 920 million annual transactions in FY2017 to an estimated 241.6 billion in FY2026 — a compound annual growth rate that no other retail payment system globally has matched. [^6]

The policy worked. Between 2021 and 2025, digital transactions in India rose nearly 11 times, with UPI commanding an 80% share. The number of banks on the platform grew from 216 to 661. Among merchants, digital acceptance reached near-universality, with 94% of small merchants having adopted UPI. Today, 55.49 crore individuals and 6.5 crore merchants use UPI through 731 banks. [^7] India's zero-cost digital payment rail became the envy of the world — studied by central banks from Brazil to Indonesia, and exported to 10 countries including France, Singapore, the UAE, Nepal, and most recently, the Maldives and Cambodia. [^8]

### What Happened This Week

On August 4, Finance Minister Nirmala Sitharaman introduced the Taxation and Other Laws (Amendment) Bill, 2026 in the Lok Sabha. Alongside income-tax provisions designed to attract foreign portfolio investment — replacing a June 2026 ordinance — the Bill carried a quiet but consequential amendment to Section 10A of the Payment and Settlement Systems Act. [^9]

The amendment, passed by voice vote on August 6, removes the existing legal prohibition that prevented banks and payment service providers from charging MDR on notified electronic payment modes. Critically, it does not prescribe any specific MDR rate, transaction threshold, or implementation timeline. Instead, it creates the legal architecture under which the Central Government can, via notification, specify which payment modes and transaction categories remain charge-free and which may attract merchant fees. [^10]

The Bill also decouples the Payment and Settlement Systems Act from the Income-tax Act's Section 269SU, which had previously been the mechanism for specifying exempt payment modes. This structural separation means the government gains flexibility to tailor exemptions without parliamentary process for each adjustment — a significant delegation of fiscal power to executive rule-making. [^11]

Sitharaman was forceful in her clarification on August 6, responding to Congress leader Jairam Ramesh's allegation that the amendment would burden consumers: "Merchant Discount Rate applies only on the merchants and not on the end users/customers. It will support the banks and fintech to invest more on infrastructure, innovation and security." She further clarified that the UPI and Services Steering Committee, chaired by NPCI, has not yet taken any decision on MDR, and that such decisions would only be considered after the Bill completes its parliamentary journey. [^12]

### Why It Matters

The amendment signals a transition in how India thinks about its digital public infrastructure. For six years, UPI's growth-at-all-costs model was subsidised implicitly: banks bore switch fees and infrastructure costs, payment apps invested in merchant acquisition and user experience with no direct transaction revenue, and the government compensated banks with incentive payments for small-value transactions (₹2,000 and below at small merchant outlets) at rates that have been progressively reduced from 0.40% to the current 0.15%. [^13]

But the arithmetic has become unsustainable at scale. The Department of Financial Services told the Parliamentary Standing Committee on Finance in March 2026 that the incentive scheme covers only 11% of actual industry costs and 14% of potential MDR revenue. The committee itself noted that "the absence of MDR makes the UPI ecosystem financially unsustainable," and flagged a ₹2,000 crore annual infrastructure gap for BHIM-UPI alone. [^14]

The costs are real and growing. Each UPI transaction — even a ₹80 chai payment — passes through four to six parties: the payer's bank, the payee's bank, the payment service provider's PSP bank, the PSP app, NPCI's central switch, and potentially a payment aggregator. Industry estimates put the all-in processing cost at approximately 0.25% per transaction. At July 2026 volumes, that translates to an annual system-wide cost of roughly ₹7,500 crore just for transaction processing, before accounting for cybersecurity, fraud prevention, infrastructure upgrades, and the NPCI's ambitious target of one billion daily transactions. [^15]

ICICI Bank has already begun charging payment aggregators for UPI transactions — a canary in the coal mine indicating that banks will recover costs regardless of the MDR framework. PhonePe paused its IPO in March 2026 citing market volatility, but the passage of this Bill materially improves the payment revenue narrative for fintech valuations. [^16]

## Technical Deep Dive

### The Architecture of MDR in UPI's Stack

UPI's transaction flow is a multi-layered architecture where each hop adds cost:

1. **Payer Initiation**: The user scans a QR code or enters a VPA. The payment app (PSP — e.g., PhonePe, Google Pay) captures and encrypts the payment instruction.

2. **Switch Routing**: The encrypted instruction, along with the UPI PIN, is sent to NPCI's central switch, which maintains the integrity of data packets and routes them to the core banking solutions of both the payer's and payee's banks. NPCI charges banks a per-transaction switch fee for this service.

3. **Authentication & Settlement**: The payer's bank decrypts the PIN, verifies balance, and debits the account. The payee's bank credits the merchant. Settlement occurs in near-real-time through NPCI's settlement systems.

4. **Merchant Settlement**: Payment aggregators (PAs) receive funds owed to merchants and hold them for T+1 or T+2 settlement, earning float income.

Under zero-MDR, the only direct revenue from UPI transactions flows to PAs through float and to PSPs through data monetisation (cross-selling loans, insurance). Banks and NPCI bear the infrastructure costs as a customer-acquisition expense — justified when UPI adoption was nascent, but increasingly difficult to sustain at 23.66 billion monthly transactions. [^17]

### Proposed Tiered Framework

The emerging consensus, as reflected in the Parliamentary Standing Committee's recommendations and the Payments Council of India's submissions, is a tiered MDR structure:

- **Individual users**: Permanently exempt. No charge on P2P transfers.
- **Small merchants** (below specified annual turnover threshold, likely ₹20–40 lakh): Continue with zero MDR, potentially retaining the incentive payment.
- **Large merchants**: MDR applicable, with a reported threshold of ₹2,000 per transaction being discussed, at a rate of 0.30% — consistent with what NPCI had originally proposed in 2019 before Section 10A prohibited it. [^18]

The UPI and Services Steering Committee, chaired by NPCI, is expected to recommend specific rates and thresholds within one to two months of the Bill's passage through both houses. The Rajya Sabha must still pass the Bill before it becomes law. [^19]

### Privacy and Security Parallel Track

Alongside the MDR debate, NPCI issued a circular in late July directing all banks and UPI apps to stop displaying customers' full mobile numbers during transactions, with a compliance deadline of September 4, 2026. Under the new norms, only the last four digits of a registered mobile number may be visible to the counterparty. [^20]

A LocalCircles survey released on August 7 found that 53% of consumers want this masking mandate applied to all UPI transactions, while 77% support it in some form. Nearly half (46%) want user-level control over what information is visible during transactions, and 48% want strong penalties for apps that expose personal data unnecessarily. This indicates growing consumer awareness of privacy as a dimension of DPI quality — not just cost and speed. [^21]

## Government Perspective

The government's framing has been measured. The amendment is presented not as a "UPI tax" but as a sustainability correction — enabling large commercial users of the public infrastructure to contribute to its maintenance, while protecting individual users and small businesses. [^22]

The political calculus is clear: with 55 crore+ UPI users, any perception of charges on ordinary consumers would be electorally toxic. Hence Sitharaman's emphasis on "merchants, not customers." The ₹2,000 transaction threshold, if implemented, would further insulate retail users — the average UPI transaction is well below this figure for P2P transfers. [^23]

The broader fiscal context matters too. The government's incentive payments to banks for UPI zero-MDR — reduced from 0.40% to 0.25% and now 0.15% over successive years — represent a direct budgetary expenditure. A tiered MDR would shift this cost from the exchequer to large merchants, a transfer that aligns with the government's broader narrative of fiscal responsibility. [^24]

Parliamentary procedure also played a role. The Bill was passed by voice vote amid din in the Lok Sabha, with Congress's Jairam Ramesh alleging that the Bill "opens the doors for MDR." The absence of detailed floor discussion means the Rajya Sabha debate will be critical for scrutiny of the executive power the amendment delegates to the government. [^25]

## Citizen Impact

For the vast majority of Indian citizens, the immediate impact is nil. UPI remains free for person-to-person transfers, and any future MDR would apply to the merchant side of person-to-merchant transactions. A ₹50 chai payment at a corner stall will not attract MDR if the stall is a small merchant; even at large merchants, the ₹2,000 threshold means most daily retail transactions would remain exempt. [^26]

The indirect impact is more nuanced. If large merchants pass through MDR costs to consumers via pricing — a phenomenon already observed with credit card surcharges at some online retailers — the cost may be invisible but real. The EPW editorial published on August 8 argued compellingly that banks, the RBI, and the government are already massive net beneficiaries of UPI through reduced cash handling costs, improved tax compliance, and data transparency, and that these gains should be set against UPI infrastructure costs before imposing merchant fees. [^27]

For small merchants, the continuation of zero-MDR (with or without incentive payments) is a continuation of the status quo. For fintech companies, the potential for MDR revenue transforms their business models — PSPs like PhonePe, Google Pay, and Paytm could earn a direct share of transaction revenue rather than relying solely on cross-selling and float. For banks, MDR revenue from UPI transactions with large merchants would partially offset the infrastructure costs they have borne since 2020. [^28]

## Global Context

India's zero-MDR approach has been globally unique among real-time payment systems. Brazil's Pix, which launched in 2020 and has grown to over 150 million users, charges merchants a small MDR (around 0.38–0.99% depending on the institution), and the system is both sustainable and wildly popular — a counterpoint to the argument that any charges would kill adoption. [^29]

Other comparable systems have tiered models. Singapore's PayNow is free for individuals but businesses pay a small per-transaction fee. The European Union's SEPA Instant Credit Transfer scheme has clearing and settlement fees that are borne by banks and passed through to corporate customers. [^30]

India's challenge is different in scale. No other system processes 23.66 billion transactions in a single month. The unit economics that work at Brazil's scale may need adjustment at India's — and conversely, the sheer volume may make even a modest 0.30% MDR on large-merchant transactions generate enough revenue to sustain the ecosystem. At current volumes, a 0.30% MDR on even 15% of transactions (large-merchant P2M above ₹2,000) would generate approximately ₹4,000–5,000 crore annually — significantly closing the sustainability gap. [^31]

India's UPI international expansion also enters the picture. UPI is now live for merchant payments in 10 countries: Bhutan, Singapore, the UAE, France, Mauritius, Sri Lanka, Nepal, Qatar, Cambodia, and the Maldives. NPCI International is building bilateral payment corridors that create network effects — but international transactions inherently involve settlement costs that zero-MDR does not cover. A domestic MDR framework would also provide the pricing template for international corridors. [^32]

## Looking Ahead

Several developments bear watching in the coming weeks:

1. **Rajya Sabha passage**: The Bill must clear the upper house. While the NDA has the numbers, opposition scrutiny of the executive power delegation could lead to amendments.

2. **NPCI Steering Committee recommendations**: Expected within 1–2 months post-passage. The specific MDR rate (0.30% is the floated figure), the turnover threshold for merchant classification (₹20–40 lakh), and the transaction value threshold (₹2,000) will be the critical parameters.

3. **NPCI September 4 privacy deadline**: The mobile number masking mandate goes live, testing the ecosystem's ability to implement privacy-by-design across hundreds of banks and apps simultaneously.

4. **UPI international corridors**: The Maldives corridor just went live; Cambodia's Phase 1 is operational with 4.5+ million merchants. Malaysia negotiations are reportedly advancing.

5. **Long-term UPI architecture**: NPCI's target of one billion daily transactions requires infrastructure investment that the current zero-MDR model cannot sustain. The MDR debate is, at its core, a debate about whether the world's largest real-time payment system can fund its own future growth. [^33]

The question before India is not whether UPI should remain free for ordinary citizens — there is bipartisan consensus on that. The real question is whether the world's most successful digital public infrastructure can transition from a subsidised growth model to a self-financing one without losing the inclusivity that made it iconic. How the government, NPCI, and the ecosystem answer that question will determine not just the future of UPI, but the template for DPI sustainability worldwide.

## Sources

- [1] Lok Sabha passes Bill to authorise Govt to permit banks to levy charges on UPI transactions — The Hindu, August 7, 2026](https://www.thehindu.com/news/national/parliament-monsoon-session-lok-sabha-clears-bills-taxation-upi-transactions-charges/article71313208.ece)
- [2] India processed a record 23.66 billion UPI transactions in July 2026 — NPCI data via Firstpost, August 7, 2026](https://www.facebook.com/firstpostin/posts/1575753891252259)
- [3] FM Nirmala Sitharaman clarifies on UPI MDR — Moneycontrol, August 6, 2026](https://www.facebook.com/moneycontrol/posts/fm-nirmala-sitharaman-clarifies-on-upi-mdr-says-no-charge-for-end-usersrespondin/1513984710773123)
- [4] Internet subscribers cross 109 crore; 2.21 lakh GPs made service-ready under BharatNet — India Gazette, August 6, 2026](https://www.indiagazette.com/news/279223930/internet-subscribers-cross-109-crore-221-lakh-gram-panchayats-made-service-ready-under-bharatnet-govt)
- [5] Time to say goodbye to subsidy for UPI? A case for tiered MDR regime — Business Standard](https://www.business-standard.com/opinion/columns/time-to-say-goodbye-to-subsidy-for-upi-a-case-for-tiered-mdr-regime-126050300369_1.html)
- [6] India Opens Door to UPI Merchant Fees as Parliament Amends Six-Year Zero-MDR Law — TechTimes, August 4, 2026](https://www.techtimes.com/articles/322958/20260804/india-opens-door-upi-merchant-fees-parliament-amends-six-year-zero-mdr-law.htm)
- [7] 3rd India International FinTech Festival 2026 — ASSOCHAM via ANI, August 6, 2026](https://www.indiasnews.net/news/279225079/india-emerges-as-global-fintech-innovation-hub-ai-and-dpi-to-drive-next-growth-phase-industry-leaders)
- [8] Countries Accepting UPI Payment 2026 — Vajiram & Ravi, updated August 2026](https://vajiramandravi.com/current-affairs/countries-accepting-upi-payment)
- [9] Taxation and Other Laws Amendment Bill tabled in Lok Sabha — Mint, August 4, 2026](https://www.livemint.com/money/personal-finance/taxation-and-other-laws-amendment-bill-lok-sabha-mdr-upi-charges-tax-measures-exemption-foreign-invest-manufacture-boost-11785837662918.html)
- [10] Will UPI Payments Above ₹2,000 Become Chargeable? — Indian Pay Calculator, August 2026](https://www.indianpaycalculator.in/govt-news/upi-mdr-fee-above-2000-who-pays-august-2026)
- [11] Lok Sabha passes bill allowing Centre to permit banks to levy charges on UPI transactions — New Indian Express, August 6, 2026](https://www.newindianexpress.com/india/2026/Aug/06/lok-sabha-clears-bill-allowing-centre-to-permit-banks-to-levy-charges-on-upi-transactions)
- [12] UPI charges: Lok Sabha passes bill for government to make changes — Times of India, August 7, 2026](https://timesofindia.indiatimes.com/india/upi-charges-lok-sabha-passes-bill-for-government-to-make-changes/articleshow/133017916.cms)
- [13] Scanner on UPI as nobody really wants to pay — FinBox](https://www.finbox.in/newsletter/thepattern/scanner-on-upi-as-nobody-really-wants-to-pay)
- [14] UPI MDR debate: Why free payments need a cost model — Policy Circle](https://www.policycircle.org/industry/upi-mdr-debate-free-payments)
- [15] UPI faces a zero-sum game — Akshay Joshi, Substack](https://substack.com/home/post/p-143094180)
- [16] India Opens Door to UPI Merchant Fees — TechTimes (PhonePe IPO reference)](https://www.techtimes.com/articles/322958/20260804/india-opens-door-upi-merchant-fees-parliament-amends-six-year-zero-mdr-law.htm)
- [17] No Transaction Fees on UPI Payments, Please! — EPW Editorial, August 8, 2026](https://www.epw.in/journal/2026/32/editorials/no-transaction-fees-upi-payments-please.html)
- [18] UPI Charges: No Fee for Users, MDR May Apply Only to Select Large Merchant Transactions — Indian Masterminds, August 8, 2026](https://indianmasterminds.com/news/upi-charges-no-fee-users-mdr-select-large-merchant-transactions-222791)
- [19] Lok Sabha Passes Bill Allowing Govt to Permit Banks, Others to Charge for UPI Transactions — The Wire, August 6, 2026](https://m.thewire.in/article/banking/lok-sabha-passes-bill-allowing-govt-to-permit-banks-others-to-charge-for-upi-transactions)
- [20] 53% consumers seek mandate to hide users' mobile no's from UPI apps — LocalCircles, August 7, 2026](https://www.localcircles.com/a/press/page/upi-consumer-survey)
- [21] Ibid.
- [22] Govt Clarifies No Charges on UPI Transactions — TaxGuru (Lok Sabha reply, August 2025)](https://taxguru.in/finance/govt-clarifies-charges-upi-transactions.html)
- [23] UPI MDR debate: Consumers, small merchants to stay exempt — Fortune India, August 8, 2026](https://www.fortuneindia.com/india/upi-mdr-debate-consumers-small-merchants-to-stay-exempt-says-payments-council/152847)
- [24] Banks told to refund UPI charges collected by them since January 1 — MediaNama, August 2020 (historical context)](https://www.medianama.com/2020/08/223-banks-refund-upi-charges-cbdt)
- [25] Lok Sabha passes bill to authorise govt to permit banks to levy charges on UPI transactions — Akashvani (News on Air), August 7, 2026](https://newsonair.gov.in/lok-sabha-passes-bill-to-authorise-govt-to-permit-banks-to-levy-charges-on-upi-transactions)
- [26] Will You Pay For UPI Now? Here's What The New Bill Actually Changes — Sahi.com, August 7, 2026](https://www.sahi.com/blogs/upi-mdr-new-bill-explained)
- [27] EPW Editorial — cited above](https://www.epw.in/journal/2026/32/editorials/no-transaction-fees-upi-payments-please.html)
- [28] UPI Zero MDR Model Faces Growing Sustainability Questions — BFSI Media](https://bfsimedia.com/upi-zero-mdr-model-faces-growing-sustainability-questions)
- [29] How India's UPI and Brazil's Pix are fast pushing the financial inclusion pedal — Moneycontrol (referenced in Substack analysis)](https://substack.com/home/post/p-143094180)
- [30] RBI interlinking UPI with Europe's TIPS payments system — MediaNama, November 2025](https://www.medianama.com/2025/11/223-rbi-interlinking-upi-europes-tips-payments-system/feed)
- [31] UPI's Cross-Border Payments Infrastructure — LinkedIn analysis, August 2026](https://www.linkedin.com/posts/nidhikaushik2015_upi-crossborderpayments-digitalpayments-activity-7490413753960902656-sbyx)
- [32] India-funded DPI projects underway in Sri Lanka, Myanmar, Kenya and Guyana — Moneycontrol](https://www.moneycontrol.com/news/business/india-funded-dpi-projects-underway-in-sri-lanka-myanmar-kenya-and-guyana-mous-signed-with-24-nations-13996734.html)
- [33] India may see productivity gains from AI, says Nilekani — Times of India, August 6, 2026](https://timesofindia.indiatimes.com/business/india-business/india-may-see-productivity-gains-from-ai-says-nilekani/articleshow/133019097.cms)
