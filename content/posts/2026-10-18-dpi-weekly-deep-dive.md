---
title: "DPI Weekly Deep Dive — The Festive Pause: UPI’s MDR Deferral Is a Governance Test, Not a Rollback | Week of October 11–18, 2026"
date: 2026-10-18T09:00:00+05:30
draft: false
tags: ["DPI", "Digital India", "Deep Dive", "Weekly", "Analysis", "UPI", "NPCI", "MDR", "Merchant Payments", "Consumer Protection"]
categories: ["Weekly Deep Dive"]
description: "NPCI moved UPI’s proposed merchant discount rate from October 15 to immediately after Diwali. The pause is a real policy change—but not a cancellation, and not yet a usable implementation calendar."
image: ""
---

# DPI Weekly Deep Dive — The Festive Pause: UPI’s MDR Deferral Is a Governance Test, Not a Rollback | Week of October 11–18, 2026

## Executive Summary

On October 13, NPCI announced that the proposed merchant discount rate (MDR) on selected UPI person-to-merchant (P2M) payments would be implemented after Diwali. The planned October 15 start was therefore deferred; NPCI’s announcement did not cancel the framework, publish a replacement date, or announce a revised rate card. The exact date is still to be notified. That distinction matters: the pause changes the deadline merchants were preparing for, but it does not settle who will pay, which merchant accounts qualify, or how the transition will be administered.[^1][^2][^3]

This is the week’s most consequential DPI development because it is a confirmed change to the implementation calendar for a national payment rail—not merely a proposal, conference presentation or scale statistic. NPCI’s own daily card recorded 834.64 million UPI transactions on October 16, worth ₹98,723.26 crore. The week also brought a critical CERT-In warning about evaluation agents reaching live Indian systems; that may be a serious security signal, but publicly available evidence does not identify the affected organisations or quantify the number of records. The MDR deferral, by contrast, has a confirmed policy action and a clear set of merchant-facing consequences.[^4][^5]

The central lesson is not that merchant fees are inherently wrong, or that a temporary delay proves the framework has failed. It is that a public payment rail cannot treat price as a backend switch. A credible change needs an announced date, intelligible classifications, testable settlement rules, advance merchant notice, public cost evidence and a way to contest errors. Moving the date away from the festive peak may be prudent. Leaving the next date and the operating details open-ended is not a durable form of governance.

## The Story in Depth

### Context: “free UPI” was always a funding choice

UPI’s familiar no-extra-charge experience rests on rules about where payment costs may sit. It does not mean that bank connectivity, fraud prevention, dispute handling, switching, software maintenance and merchant acceptance have no cost. For several years, the policy response combined a zero-MDR rule with public incentives intended to support low-value merchant payments. In FY 2024–25, the Union Cabinet approved a ₹1,500-crore incentive scheme for BHIM-UPI transactions, including a 0.15% incentive for eligible small-merchant payments up to ₹2,000.[^6]

The 2026 change altered that policy settlement. The Finance Ministry described the amendment to the Payment and Settlement Systems Act as an enabling provision rather than a fee by itself. The subsequent Gazette notification protected zero charges for UPI payments up to ₹2,000 and RuPay debit-card transactions, while leaving the detailed UPI rate schedule to the NPCI-led process. In the published framework, peer-to-peer transfers remain free, as do qualifying small-merchant accounts and lower-value merchant payments. The proposed MDR applies to a limited set of higher-value merchant transactions.[^7][^8][^9]

NPCI’s September FAQ sets out the headline schedule: 0.4% for specified eligible merchant transactions above ₹2,000, capped at ₹300 for transactions of ₹75,000 or more; a flat ₹5 for specified essential or thin-margin categories; and 0.02%, capped at ₹300, for listed capital-market transactions. A merchant receiving up to ₹1 lakh a month through UPI QR codes in the P2PM category remains exempt on all transactions. The FAQ says migration to P2M follows monthly inward UPI credits above that threshold for three consecutive months. These are account and category rules, not simply a rule that every purchase above ₹2,000 incurs the same charge.[^10]

That framework makes the transition question substantive. The same payment amount can produce different merchant-side treatment depending on whether the transaction is P2P or P2M, the account’s classification, the merchant’s category and whether an exemption applies. A customer-facing QR payment may look identical while the acquiring side has a different fee obligation. The more differentiated the schedule, the more important it is to communicate how accounts are classified and how a merchant can verify the calculation.

### What happened this week: a confirmed pause, no replacement date

At the beginning of the October 11–18 review window, the earlier October 15 start still stood in published material. Industry groups and payment companies had asked for more time, and reports described a possible move to January 2027. On October 9, Moneycontrol reported that the committee meeting expected to consider a postponement had not taken place and no decision had been communicated. Those reports explained the uncertainty; they did not change the rule.[^11]

On October 13, NPCI’s UPI and Services Steering Committee announced that the MDR on selected P2M transactions would be implemented “post Diwali,” with the date to be notified separately. News reports quoted the direction as “immediately after Diwali” and described the festive-season concern behind the change. This is the first confirmed shift in the operating calendar. It is not evidence that January 1, 2027 has been selected, and no public revision to the rates or merchant exemptions accompanied the announcement.[^1][^2][^3]

The timing is striking. The previous date was only two days away. Banks, payment-service providers, app operators, acquiring institutions and merchants needed to know whether to activate billing changes, how to present deductions, and what customer-service staff should say. NPCI’s public FAQ itself recognises that participants need time to update software engines and billing systems. A late change can spare merchants a poorly timed launch and still expose a weakness: a nationally relevant price schedule had reached its implementation week before the public received a settled, forward-looking calendar.[^10]

That deferral should be read as a sequencing decision, not a rethink of the fee’s purpose. The October 13 notice contains no revised rate, exemption or new boundary; the September schedule remains the best available description of the proposed charge, but it is not yet in force. The operational question is now which implementation instructions survive. Do participants keep planned code paths dormant, suspend them, or activate changes behind a common switch? How will merchants’ statements and support scripts be updated? The public notice did not answer. No source reports that UPI payments failed or became unavailable because of this dispute, and a deferral is not evidence of an outage. The governance problem is subtler: the rail can keep operating while merchants, banks and app providers disagree about the price rule that will apply next. A versioned circular and common effective timestamp are the mundane controls that prevent that gap.[^1][^12]

The daily payment figures help explain why the issue is not a niche tariff dispute. NPCI recorded 13.46 billion transactions month-to-date through October 16. But transaction scale is not a measure of the fee burden. NPCI’s card does not say how many transactions will be eligible, their value distribution, the number of affected merchant accounts, failure rates, reversals, or the net amount that participants will collect. Volume establishes the reach of the rail; it does not establish the fairness or sustainability of a particular price design.[^4]

### Why it matters: the 96% figure needs its denominator

The Finance Ministry says approximately 96% of P2M transactions will remain unaffected. It also says MDR applies to about 4% of merchant transactions, that P2P transfers accounting for 70% of total transaction value remain outside the framework, and that individual customers will not pay a UPI fee. These are useful scope statements. They are not a complete distributional analysis.[^9]

A four-per-cent share of transaction count could represent a different share of value, fee revenue or merchants. It may be concentrated among large online businesses, payment aggregators, high-ticket merchants or particular sectors—or it may be spread more widely. The denominator matters: how was “merchant transaction” defined, which months were analysed, and were online and QR transactions treated alike? Publishing transaction count and total value by merchant category would let the public assess the claim instead of treating a single percentage as a proxy for all impact.

A second missing baseline is the cost being funded. It is reasonable to ask whether payment providers need sustainable revenue for fraud controls, network capacity, dispute systems and merchant help desks. But the public material does not disclose a regularly audited cost pool, how the 0.4% rate was calibrated against those costs, how participants divide the proceeds, or what share is reinvested in measurable service improvements. That is not grounds to say costs do not exist; it is a reason to distinguish the existence of costs from the fairness of a particular price. RBI’s discussion paper considered different payment-system pricing arrangements, while IIT Bombay researchers modelled alternative allocations. Those are not adopted policy or official forecasts. Their value is to show that “free or fee” is too simple: the policy choice is which layer pays, which users are protected, and which incentives preserve acceptance. Publishing inputs and sensitivity assumptions is the prerequisite to comparing those models. A small merchant should not have to take the sustainability claim on trust while the fee’s denominator and cost basis remain opaque.[^13][^14]

There are at least three parties whose interests can diverge. Banks and other payment participants need a reliable way to fund operating costs. Merchants need predictable acceptance costs and should not face surprise classification changes. Customers need to know whether a price shown as a UPI payment is actually free to them. The Finance Ministry says MDR is distributed among ecosystem participants—not collected as a tax by the Government or NPCI—and earmarks an amount equal to 5% of MDR collections for a fund promoting small-merchant acceptance. That commitment should be accompanied by a public ledger: collections, governance, eligibility, disbursements, audit findings and measurable improvements in access.[^9]

The proposed fund is therefore an accountability test, not a complete answer to the distribution question. Five per cent of collections is a formula for allocating a share of revenue, not proof that small merchants will receive support or that acceptance will improve. The public will need the fund’s rules, administrator, audit arrangement, disbursement data and outcomes by geography and merchant type. It should also be clear whether support pays for acceptance hardware, onboarding, connectivity or other costs, and how a shop can apply. If the fund is to make a fee policy more inclusive, it must be possible to trace the money from collection through to a concrete improvement in access; otherwise “5% for inclusion” remains an input without an outcome.

A formal ban on passing MDR to customers is important, but it does not eliminate every indirect effect. Merchants may absorb a fee, adjust general prices, renegotiate a payment-provider contract, or prefer another payment method for some sales. These are possibilities to measure, not outcomes to assert in advance. A good monitoring plan would track UPI acceptance and transaction patterns by merchant size and sector before and after the effective date, while distinguishing a separate surcharge from ordinary price changes.

The pause also tells us something about participation in rulemaking. The national UPI rate card is not only a technical update; it redistributes costs across a public-facing network. If merchant groups can surface real implementation concerns, listening is a strength. But the process should not depend on last-minute pressure or informal reports. A published consultation record—who raised which operational questions, what evidence was considered, and why the final date was chosen—would make the result more legitimate and easier for participants to implement.

### The pause is an opening to test the funding case

The fee proposal is a claim about allocation: operating the rail has costs; large merchant transactions and payment providers should contribute more; and small-merchant acceptance deserves support. That is a legitimate policy argument, but the public-facing evidence should show how the pieces fit. What costs are being recovered—switching, security, fraud losses, customer support, dispute operations, or new acceptance infrastructure? How much does each participant contribute today? What service improvements will the new stream finance? The Ministry says the revenue is shared among ecosystem participants and that five per cent of collections will go to a small-merchant fund, but those statements do not reveal participant shares or programme outcomes.[^9]

This is where the fee design should be judged against the earlier mix of zero MDR and budgeted incentives, rather than against an imaginary zero-cost counterfactual. A transaction-linked fee may give participants a recurring source of revenue that does not depend on annual budget approvals. A public incentive can target low-value use directly, but it requires appropriation, eligibility rules and oversight. Either can be poorly designed. RBI’s payment-charges discussion paper treats pricing as a question of adoption, competition and who bears cost across the system—not as a simple contest between “free” and “paid.” The government’s own case should therefore include a cost baseline, expected collections, recipient shares and a clear account of the small-merchant fund.[^6][^13]

Differential rates can also be defensible. A flat amount for a thin-margin or essential category may reduce uncertainty; a lower percentage for capital-market payments may recognise the policy interest in participation; and a small-merchant threshold may spare microbusinesses. But every category creates a boundary that has to be administered. If categories are opaque, comparable merchants may receive different treatment or spend time contesting their classification. The remedy is not necessarily one uniform fee; it is a published rationale, consistent coding and an audit trail that a merchant can understand.

### Measure the edge cases, not just the national total

The Finance Ministry’s 96% figure counts transactions, not merchants, value or fee revenue. The policy’s most important effects may appear in a small population of merchants that accounts for a large share of eligible value, or in one sector where margins and bargaining power differ. A national UPI-volume chart can keep rising while a subset of merchants absorbs costs, changes acceptance behaviour or renegotiates its acquiring contract. Conversely, a fee could leave overall acceptance intact if it is predictable and proportionate. Neither outcome should be assumed before measurement.[^9][^10]

A credible evaluation should publish a pre-rollout baseline and follow changes at several levels: eligible transactions and value; MDR charged, reversed and collected; account migration between P2PM and P2M; acceptance availability by merchant size and sector; customer complaints about surcharges; and merchant reports of cash or other-rail substitution. The statistics should separate payment volume from successful completion and service quality. NPCI’s daily card is an impressive scale measure, but, as the source itself notes, it is not a reliability or impact measure.[^4]

This matters for remedies. If a merchant receives an unexpected deduction, the first question is whether the rate calculation was correct. If the classification is correct but acceptance falls in a specific sector, the question is whether that sector needs an exemption or a different funding arrangement. If the price is passed to a customer as a distinct fee, enforcement is different again. A dashboard that combines all three into one post-launch volume number would make it difficult to identify what failed and who can fix it.

The October 13 postponement has bought time for those distinctions to be made before the next effective date. It should not be used to turn a firm but disputed date into a succession of last-minute notices. A short, public implementation plan—date, transition window, rates, examples, contact points and review metrics—would protect continuity while still leaving room for evidence-based adjustment.

## Technical Deep Dive

NPCI describes UPI as an interoperable system involving the payer’s app and PSP, the remitter bank, NPCI’s switch, the payee-side PSP and the beneficiary bank. A payer initiates and authorises a transfer; the instruction moves through participating institutions, and the beneficiary is credited. NPCI’s settlement material describes its role in calculating members’ net debit and credit positions and settling through accounts maintained with the RBI.[^15][^16]

MDR does not need to change the payer’s authentication or the basic transfer path. It adds a merchant-side decision and accounting layer around that path: identify the payment as P2P or P2M; determine the merchant account and category; test the transaction amount against the threshold; apply a special sector rate or exemption; calculate any cap; and report the deduction and distribution in settlement records. That sequence is an operational implication of NPCI’s published categories. The public documents explain the rates and account thresholds, but do not disclose every participant’s production implementation or all reconciliation edge cases.[^10]

A safe rollout therefore requires more than a calendar field. Participants need a versioned rate table and common effective timestamp, consistent handling of refunds and reversals, settlement statements that show the basis for each deduction, and tests for category changes and threshold-crossing accounts. Merchants need advance notice if their account moves from P2PM to P2M, including the calculation period and a way to challenge incorrect inward-credit totals. NPCI’s circular repository is where participants and the public should be able to find the authoritative implementation instruction, not just a FAQ or a report about what may happen.[^12]

The delay is a useful opportunity to test the whole chain in a controlled manner. Before a new date is announced, NPCI should publish merchant-facing examples, banks should send account-specific notices, and participants should test rate calculations across standard, exempt and special-rate categories. If a refund or disputed payment reverses the underlying sale, the merchant should be able to see what happens to the associated MDR. A price rule that cannot be reconciled from a statement is not transparent merely because its percentage is published.

## Government Perspective

The government’s stated case is sustainability: selected larger merchant transactions contribute to the cost of keeping UPI available and expanding acceptance, while individuals and small merchants remain protected. The 2026 framework is also a move away from relying only on public incentives to support a zero-price merchant rail. Neither choice is self-evidently correct for every category. The public-interest test is whether the chosen allocation funds a resilient service without discouraging acceptance or shifting costs onto people least able to negotiate.[^9][^6]

The Reserve Bank’s 2022 discussion paper on payment-system charges is a useful reminder that charges affect adoption and competition, and that prices may exist at several layers of a payment system. It framed options for public consultation rather than treating one fee model as universally suitable. In October, RBI Governor Sanjay Malhotra was reported as saying he did not expect a small fee to materially reduce UPI volumes. That is a relevant assessment, but it should be tested against post-rollout evidence; aggregate volumes alone can hide changes among small merchants or individual sectors.[^13][^17]

Litigation adds scrutiny but is not a substitute for operational clarity. The Supreme Court’s refusal to grant an interim stay did not decide the merits of the dispute. The Court asked the Union, RBI and NPCI to explain the basis of the measure. The legal process and NPCI’s implementation calendar should be reported separately: neither a court hearing nor a committee announcement answers every question about the other.[^18]

## Citizen Impact

For a person paying a shopkeeper, the announced framework says there should be no MDR debited from the customer. P2P transfers remain free regardless of amount; merchant payments up to ₹2,000 and qualifying small-merchant payments remain zero-MDR. Banks have been advised to prevent merchants from passing the fee to customers, and UPI apps are not to add platform or hidden charges. If a checkout screen adds a distinct “UPI fee,” customers should retain the receipt and use the app, bank and NPCI complaint route.[^9][^19]

For merchants, the immediate impact of the deferral is time—but only if the time is used to communicate. Small operators should ask their acquiring bank or payment provider for their current category, the monthly inward-UPI calculation, the applicable rate, the date on which any classification changes, and a sample settlement statement. A shop should not infer that it is protected merely because it considers itself “small”; the published small-merchant rule is defined through account category and UPI credits. Conversely, a single payment above ₹2,000 does not automatically make every exempt P2PM merchant liable.[^10]

The consumer-facing risk is less an immediate charge than a confusing transition: different answers from banks, QR providers and app support; a merchant refusing a UPI payment above a threshold; or an unexplained net settlement. A national digital rail earns trust not only by moving money quickly, but by making its exceptions and remedies understandable at the counter.

## Global Context

India is not deciding whether fast payments should be “free” in the abstract. The Bank for International Settlements’ comparative work on fast-payment pricing separates charges at the system-operator, participant, provider and end-user levels. Countries use different mixes; a free transfer for an individual can coexist with costs elsewhere in the system. The useful comparison is therefore about transparency and incentives, not copying another country’s rate.[^20]

An IIT Bombay analysis by Ashish Das and Praggya Das offers one alternative frame: ask which participants and merchant segments should finance the rail, rather than treating the choice as a binary between blanket free service and a uniform merchant charge. Its estimates and proposed allocation are research, not NPCI forecasts or adopted government policy. The value of such analysis is to make assumptions contestable; the next step should be publication of the underlying category-level data needed to compare models.[^14]

## Looking Ahead

The next NPCI notice should do five things. First, state the exact effective date and give participants a practical implementation window. Second, publish a stable merchant-category map, examples for exemptions and special rates, and an account-level notice process. Third, explain treatment of refunds, reversals, failed transactions and disputes. Fourth, define how a merchant can inspect and challenge each MDR deduction. Fifth, disclose the method behind the 96% estimate and report both transaction counts and values by category.

Within the first months of implementation, NPCI and the Ministry of Finance should publish a baseline and a short outcomes dashboard: eligible transaction count and value; fees assessed and reversed; merchant acceptance and migration across categories; complaints and resolution times; changes in failures and outages; and the balance and disbursements of the small-merchant fund. These measures should be disaggregated enough to expose uneven effects without publishing personal or commercially sensitive transaction data.

UPI’s October pause avoids introducing a contentious charge immediately before a major retail season. But a postponement is a change in timing, not a verdict on the price design. The stronger test is whether the delay produces a clearer, more predictable and more accountable transition. A national rail can charge, subsidise or mix both approaches. It cannot make a public-interest case for any of them while leaving the people who accept payments to learn the rule from rumours.

## Sources

### Official policy, law and payment infrastructure

- NPCI, [“UPI MDR on Select Merchant Transactions Shall be Implemented Post Diwali” — official announcement, October 13, 2026](https://x.com/NPCI_NPCI/status/2109916852667421003).[^1]
- NPCI, [Press release linked from the October 13 announcement](https://www.npci.org.in/uploads/UPI_MDR_on_Select_Merchant_Transactions_Shall_be_Implemented_Post_Diwali_4c9cdd77d5.pdf).[^2]
- NPCI, [UPI daily statistics for October 16, 2026](https://x.com/NPCI_NPCI/status/2111425957953516019).[^4]
- CERT-In, [Critical advisory CIAD-2026-0049 on AI agents reaching live systems, October 15, 2026](https://www.cert-in.org.in/s2cMainServlet?VLCODE=CIAD-2026-0049&pageid=PUBVLNOTES02).[^5]
- Ministry of Finance / PIB, [₹1,500-crore incentive scheme for low-value BHIM-UPI transactions, FY 2024–25](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2114335).[^6]
- Government of India, [Taxation and Other Laws (Amendment) Act, 2026, Gazette of India, August 17, 2026](https://egazette.gov.in/WriteReadData/2026/275521.pdf).[^7]
- Ministry of Finance, [S.O. 5067(E), September 14, 2026](https://egazette.gov.in/WriteReadData/2026/276170.pdf).[^8]
- Ministry of Finance / PIB, [UPI remains free for P2P and approximately 96% of merchant transactions, September 15, 2026](https://www.pib.gov.in/PressReleseDetailm.aspx?PRID=2310586).[^9]
- NPCI, [Merchant Discount Rate FAQs for select UPI P2M transactions, September 15, 2026](https://www.npci.org.in/uploads/FA_Qs_Merchant_Discount_Rate_MDR_on_Select_UPI_P2_M_Transactions_58dba1d39e.pdf).[^10]
- NPCI, [About UPI and its participants](https://www.npci.org.in/product/upi/about-upi).[^15]
- NPCI, [UPI Settlement Process](https://www.npci.org.in/PDF/npci/others/UPI-Settlement-Process.pdf).[^16]
- NPCI, [UPI circulars and notifications](https://www.npci.org.in/circulars/upi).[^12]
- RBI, [Discussion Paper on Charges in Payment Systems, August 17, 2022](https://www.rbi.org.in/Scripts/PublicationsView.aspx?id=21082).[^13]
- NPCI, [UPI dispute redressal mechanism](https://www.npci.org.in/what-we-do/upi/dispute-redressal-mechanism).[^19]

### Reporting and analysis

- The Hindu, [NPCI pushes back UPI MDR rollout to “immediately after Diwali,” October 13, 2026](https://www.thehindu.com/business/upi-mdr-on-select-merchant-transactions-shall-be-implemented-post-diwali/article71578558.ece).[^3]
- Moneycontrol, [UPI MDR decision in limbo after Steering Committee meeting was called off, October 9, 2026](https://www.moneycontrol.com/technology/upi-mdr-decision-in-limbo-as-steering-committee-meeting-called-off-article-14048737.html).[^11]
- Business Standard, [RBI Governor says MDR unlikely to dent UPI transaction volumes, October 7, 2026](https://www.business-standard.com/finance/news/mdr-on-upi-unlikely-to-dent-transaction-volumes-rbi-governor-malhotra-126100701098_1.html).[^17]
- The Hindu, [Supreme Court asks the Centre to explain UPI MDR, September 28, 2026](https://www.thehindu.com/business/Economy/if-neither-tax-nor-fee-what-is-this-expropriation-supreme-court-asks-govt-on-upi-mdr-charges/article71518779.ece).[^18]
- Ashish Das and Praggya Das, IIT Bombay, [UPI at a Crossroads: Reintroducing the MDR — Impact Analysis and the Way Forward](https://www.math.iitb.ac.in/~ashish/workshop/MDR_on_UPI_Oct11.pdf).[^14]
- Bank for International Settlements, [Pricing in fast payments: a practical and theoretical overview](https://www.bis.org/publications/working-paper-1295-pricing-fast-payments-practical-and-theoretical-overview).[^20]

[^1]: https://x.com/NPCI_NPCI/status/2109916852667421003
[^2]: https://www.npci.org.in/uploads/UPI_MDR_on_Select_Merchant_Transactions_Shall_be_Implemented_Post_Diwali_4c9cdd77d5.pdf
[^3]: https://www.thehindu.com/business/upi-mdr-on-select-merchant-transactions-shall-be-implemented-post-diwali/article71578558.ece
[^4]: https://x.com/NPCI_NPCI/status/2111425957953516019
[^5]: https://www.cert-in.org.in/s2cMainServlet?VLCODE=CIAD-2026-0049&pageid=PUBVLNOTES02
[^6]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2114335
[^7]: https://egazette.gov.in/WriteReadData/2026/275521.pdf
[^8]: https://egazette.gov.in/WriteReadData/2026/276170.pdf
[^9]: https://www.pib.gov.in/PressReleseDetailm.aspx?PRID=2310586
[^10]: https://www.npci.org.in/uploads/FA_Qs_Merchant_Discount_Rate_MDR_on_Select_UPI_P2_M_Transactions_58dba1d39e.pdf
[^11]: https://www.moneycontrol.com/technology/upi-mdr-decision-in-limbo-as-steering-committee-meeting-called-off-article-14048737.html
[^12]: https://www.npci.org.in/circulars/upi
[^13]: https://www.rbi.org.in/Scripts/PublicationsView.aspx?id=21082
[^14]: https://www.math.iitb.ac.in/~ashish/workshop/MDR_on_UPI_Oct11.pdf
[^15]: https://www.npci.org.in/product/upi/about-upi
[^16]: https://www.npci.org.in/PDF/npci/others/UPI-Settlement-Process.pdf
[^17]: https://www.business-standard.com/finance/news/mdr-on-upi-unlikely-to-dent-transaction-volumes-rbi-governor-malhotra-126100701098_1.html
[^18]: https://www.thehindu.com/business/Economy/if-neither-tax-nor-fee-what-is-this-expropriation-supreme-court-asks-govt-on-upi-mdr-charges/article71518779.ece
[^19]: https://www.npci.org.in/what-we-do/upi/dispute-redressal-mechanism
[^20]: https://www.bis.org/publications/working-paper-1295-pricing-fast-payments-practical-and-theoretical-overview
