---
title: "DPI Weekly Deep Dive — ONDC's Inflection Point | Corporate Investment, Multimodal Transport & Kirana Digitisation"
date: 2026-06-28T09:00:00+05:30
draft: false
tags: ["DPI", "Digital India", "Deep Dive", "Weekly", "Analysis", "ONDC", "Digital Commerce"]
categories: ["Weekly Deep Dive"]
description: "How ONDC's Rs 430 crore funding round, Uber's strategic investment, metro ticketing integration, and the DigiDukaan kirana digitisation drive mark a decisive inflection point for India's open e-commerce network."
image: ""
---

# DPI Weekly Deep Dive — ONDC's Inflection Point | Week of June 22–28, 2026

## Executive Summary

The week of June 22–28, 2026 will be remembered as the moment ONDC — the Open Network for Digital Commerce — crossed from government-backed experiment to commercially validated infrastructure. Three developments converged simultaneously: Uber announced a Rs 60 crore strategic investment in ONDC alongside the launch of metro ticketing on its app via the open network, starting with Delhi Metro; the network closed a Rs 430 crore funding round from a consortium of institutional and corporate investors including SBI, Zoho, Paytm, and Amul; and DigiDukaan, ONDC's flagship B2B kirana digitisation initiative, went live in Rajasthan with Chief Minister Bhajan Lal Sharma inaugurating the rollout in Jaipur.

Taken together, these moves signal that ONDC is no longer just a policy ambition. It has acquired corporate backing at scale, expanded into mobility and transit use cases beyond its original retail-commerce remit, and begun onboarding the country's 1.4 crore kirana stores into digital procurement through DigiDukaan. With 20 crore buyers, over 7.64 lakh sellers, presence in 616 cities, and nearly 90 lakh monthly transactions already on the books, ONDC is approaching the critical mass where network effects could become self-reinforcing. The question is no longer whether ONDC will survive — it is whether India's digital commerce landscape will look fundamentally different in three years because of it.

## The Story in Depth

### Context: What ONDC Is and Why It Matters

ONDC is a Section 8 non-profit company set up by the Department for Promotion of Industry and Internal Trade (DPIIT) under the Ministry of Commerce and Industry. It operates an open protocol called Beckn that decouples buyer apps from seller apps, much as UPI decoupled payment apps from banks. In the traditional e-commerce model, a platform like Amazon or Flipkart controls the entire stack: discovery, cataloguing, ordering, payments, logistics, and settlement. ONDC breaks this into independent layers — buyer apps handle presentation and user acquisition, seller apps expose catalogues, gateways route messages between them, logistics service providers handle delivery, and a settlement layer reconciles money flows across all counterparties. [^1]

The protocol is asynchronous. When a buyer searches for "rice 5kg," the buyer app constructs a Beckn `search` message, posts it to the ONDC gateway, and the gateway broadcasts it to all registered seller apps in the relevant domain. Responses arrive asynchronously as `on_search` messages within a configurable window, typically 8 seconds. The buyer app aggregates, ranks, and presents results. The user never knows they just queried 80–200 independent seller systems simultaneously. [^2]

This architecture matters because it eliminates the platform monopoly on discovery. A kirana store in Jaipur lists once through a seller app and becomes discoverable on Paytm, PhonePe, Magicpin, or any other buyer app — without paying listing fees to any single platform. The ONDC 2.0 vision, as articulated by ONDC's leadership, aims for "sovereign, agentic commerce at population scale." [^3]

### What Happened This Week

**Uber's strategic investment and metro ticketing.** On June 24, Uber launched metro ticketing on its app powered by ONDC, with Delhi Metro as the first live city. This is not merely a product feature — it represents ONDC's expansion beyond its original retail-commerce mandate into multimodal urban transit. Uber's Chief Technology Officer Praveen Neppalli Naga described it as aligning with Uber's vision of becoming a one-stop mobility solution, while ONDC's Acting CEO Vibhor Jain called it a significant step in expanding access to interoperable digital infrastructure. [^4]

Simultaneously, Uber confirmed a Rs 60 crore strategic investment in ONDC, announced earlier in June. Prabhjeet Singh, then-President of Uber India and South Asia, said: "India has been at the forefront of building Digital Public Infrastructure that is inclusive, interoperable, and transformative at scale." Uber's investment builds on its existing operational integrations and aims to expand access to multimodal transportation architectures and decentralised logistics frameworks on the open network. [^5] Notably, the ONDC integration in Mumbai already encompasses Mumbai Metro, MMRC, Maha Mumbai Metro, BEST buses, Uber, Ola, State Transport, and Indian Railways — effectively creating a single-ticketing surface for the city's entire public transit ecosystem. [^6]

**The Rs 430 crore funding round.** ONDC is raising Rs 430 crore from a consortium of strategic corporate and institutional investors to fuel its next growth phase. The first tranche of Rs 220 crore has already been secured, led by SaaS firm Zoho with a Rs 70 crore infusion, alongside Uber and Paytm, which invested Rs 60 crore each. Other participants include the State Bank of India and Amul. This is ONDC's largest capital raise to date and marks the first time major corporate players have taken direct equity positions in the network. [^3]

**DigiDukaan goes live in Rajasthan.** On June 19, Rajasthan Chief Minister Bhajan Lal Sharma inaugurated DigiDukaan in Jaipur — ONDC's flagship B2B initiative designed to digitise procurement for kirana stores. The platform shifts small retailers from fragmented, phone-and-ledger-based ordering from distributors to an open, decentralised digital procurement grid. DigiDukaan connects retailers, distributors, and FMCG brands on the ONDC protocol, enabling digital ordering, real-time inventory visibility, and automated reconciliation. The National Traders' Welfare Board noted the successful launch in its June 26 meeting and appreciated the encouraging response from local traders. [^7]

**Government engagement.** Commerce and Industry Minister Piyush Goyal held a review meeting with ONDC and Nirmit Bharat officials on June 10, discussing leveraging open digital networks to transform retail and distribution ecosystems. The DPIIT-ONDC Bharat Commerce Chintan Shivir, a CPG roundtable held on June 12, brought together FMCG industry leaders to discuss digitising procurement for India's 1.4 crore kirana stores through DigiDukaan. [^8] In Kerala, an inter-departmental workshop on ONDC's proposals across retail, tourism, and transport was held on June 24, chaired by Minister for Industries and Commerce P.K. Kunhalikutty. [^9]

**Global recognition.** Queen Máxima of the Netherlands, in her capacity as the UN Secretary-General's Special Advocate for Financial Health, visited India during the week and praised India's digital public infrastructure — including ONDC alongside UPI and Aadhaar — noting that around 89% of Indians now have bank accounts, largely driven by the digital stack. [^10]

### Why It Matters

**Network effects are accelerating.** Uber's investment and metro integration do two things simultaneously: they bring a marquee global brand into the ONDC ecosystem, and they prove that the Beckn protocol can handle use cases far beyond retail groceries. If a commuter can buy a Delhi Metro ticket on Uber's app through ONDC, the same protocol can handle bus passes, train tickets, parking payments, and last-mile logistics. ONDC is no longer competing only with Amazon and Flipkart — it is becoming the interoperability layer for all digital transactions in India's urban economy.

**The kirana digitisation play is massive.** India's general trade — the unorganised retail sector comprising kirana stores, paan shops, and local provision stores — accounts for over 88% of the country's retail turnover but remains overwhelmingly analogue in its procurement. DigiDukaan's Rajasthan launch is the first state-level rollout of what ONDC envisions as a national programme. The CPG roundtable with DPIIT brought together major FMCG brands to discuss onboarding their distribution networks, indicating serious corporate engagement with the digitisation agenda. [^8]

**The funding round validates the model.** When SBI, Zoho, Paytm, Uber, and Amul — institutions spanning banking, enterprise SaaS, fintech, mobility, and dairy cooperatives — all invest in ONDC, it signals that the open-commerce thesis has crossed the credibility threshold. This is not government money; these are commercial entities making calculated bets on ONDC as infrastructure.

## Technical Deep Dive

ONDC's technical architecture rests on the **Beckn protocol** — an open, JSON-over-HTTP specification that defines message types for the entire commerce lifecycle: `search`, `on_search`, `select`, `on_select`, `init`, `on_init`, `confirm`, `on_confirm`, `status`, `on_status`, `track`, `on_track`, `cancel`, `on_cancel`, `rating`, `on_rating`, `support`, and `on_support`. [^1]

The key components are:

1. **Registry** (`prod.registry.ondc.org/v2.0/lookup`) — issues cryptographic identities to all network participants. Each buyer app, seller app, and gateway has a signed identity that the network uses for trustful message routing. [^11]

2. **Gateways** — route messages between participants without storing catalogue data. When a buyer app sends a `search`, the gateway fans it out to all registered seller apps matching the domain and geo-cell, then aggregates their `on_search` responses back to the buyer.

3. **Buyer Apps (BAPs)** — consumer-facing surfaces that implement the full Beckn message set, handle identity signing, and build their own ranking and presentation. Examples include Paytm, PhonePe, Magicpin, and the Tata Neu integration. [^2]

4. **Seller Apps (BPPs)** — catalogue surfaces that expose merchant products, prices, inventory, and fulfilment options via Beckn endpoints. Major BPPs include eSamudaay, Mystore, and large retailers like Reliance Smart and ITC running their own integrations. [^2]

5. **Logistics Service Providers (LSPs)** — selected via Beckn's `Logistics` domain for delivery fulfilment. Loadshare, Shadowfax, Dunzo Daily, and Porter are active on the network.

The metro ticketing integration works through ONDC's **mobility profile** — a domain-specific extension of Beckn that handles transit ticketing, seat selection, and real-time schedule queries. When Uber displays Delhi Metro ticketing, it acts as a buyer app querying the Delhi Metro's seller app endpoint through the ONDC gateway. The same architecture that delivers groceries from a kirana store now delivers QR-coded metro tickets. [^4] [^6]

DigiDukaan adds a **B2B procurement profile** to ONDC, enabling order management between retailers, distributors, and brands rather than the traditional B2C consumer-to-merchant flow. This extends ONDC from a consumer-commerce protocol to a full-spectrum commerce protocol — encompassing B2C retail, B2B procurement, and multimodal transit ticketing on a single open network. [^7]

## Government Perspective

The government's stance on ONDC has shifted from cautious incubation to aggressive acceleration. Minister Piyush Goyal's June 10 review meeting with ONDC and Nirmit Bharat focused on "leveraging open digital networks to transform retail, distribution ecosystems," with explicit mention of empowering farmers and artisans through digital market access. [^8]

The ONDC Advisory Council, chaired by R.S. Sharma with mentors including Nandan Nilekani, has set ambitious five-year targets: 900 million buyers, 1.2 million sellers, and GMV exceeding $48 billion. [^12] The ₹430 crore funding round, partially sourced from public-sector banks like SBI alongside private corporates, suggests that the government views ONDC as strategic infrastructure worthy of both policy support and capital allocation.

DigiDukaan's state-level rollout pattern — Rajasthan first, followed by planned expansion to Mumbai, Bengaluru, and Delhi-NCR — mirrors the government's preferred approach of demonstrating success in one geography before scaling nationally. The National Traders' Welfare Board's endorsement of the Jaipur launch in its official minutes indicates that the Centre is actively coordinating with state governments on ONDC adoption. [^7]

The multimodal transit integration aligns with the broader National Urban Digital Mission and India's push for interoperable transit solutions — a natural extension of UPI's interoperability thesis to physical mobility.

## Citizen Impact

For ordinary Indians, ONDC's expansion this week has three tangible implications.

**Lower prices on food and grocery delivery.** With Uber, Paytm, PhonePe, and other buyer apps all sourcing from the same pool of ONDC-registered sellers, price competition among buyer-facing surfaces is increasing. Restaurants and food sellers on ONDC typically charge 3–5% commission versus 20–30% on dominant food delivery platforms, and those savings are partially passed to consumers. A meal that costs ₹300 on a traditional platform can cost ₹225–255 through an ONDC buyer app. [^2]

**Digital tools for kirana store owners.** DigiDukaan gives kirana store owners — who have traditionally managed procurement through phone calls, WhatsApp messages, and handwritten ledgers — a digital ordering interface connected to their existing distributors and brands. This means better price visibility, automated order tracking, digital invoices, and access to promotional schemes they previously missed. For a kirana store in Jaipur ordering FMCG products, DigiDukaan reduces the cognitive and logistical burden of managing 15–20 supplier relationships. [^7]

**Simplified urban transit.** The metro ticketing integration means a Delhi or Mumbai commuter can buy metro tickets on Uber's app without downloading a separate transit app. Under the Railway Minister Ashwini Vaishnaw's push, ONDC now integrates Mumbai Metro, MMRC, Maha Mumbai Metro, BEST, Uber, Ola, State Transport, and Indian Railways — enabling seamless multimodal trip planning and ticketing from a single interface. This is particularly valuable for the estimated 80 million daily public transit users across India's top 20 cities. [^6]

## Global Context

ONDC is being watched closely as a potential template for other countries seeking to break e-commerce monopolies without resorting to heavy-handed regulation. Kenya has experimented with Beckn-based open commerce in Nairobi; ASEAN nations have expressed interest in interoperable commerce protocols. The comparison with UPI is now explicit: just as UPI demonstrated that an open protocol could displace platform-owned payment rails at population scale, ONDC aims to do the same for e-commerce discovery and fulfilment. [^2]

Queen Máxima's visit during this week — specifically praising India's digital public infrastructure — reinforces the international narrative that India's DPI model (Aadhaar + UPI + ONDC) is the world's most complete stack for digital inclusion at scale. Her observation that 89% of Indians now have bank accounts, driven largely by the digital infrastructure layer, validates the theory that DPI creates access before markets do. [^10]

The UPI comparison is instructive. UPI processed 24,162 crore transactions worth Rs 314 lakh crore in FY 2025-26, with cross-border acceptance across eight countries and daily volumes exceeding 66 crore transactions. [^13] If ONDC captures even a fraction of that adoption curve, the implications for India's 14 crore retail businesses — 1.4 crore of which are kirana stores — are transformative.

## Looking Ahead

Several developments merit close monitoring in the coming weeks:

1. **DigiDukaan state expansion.** The planned rollout to Mumbai, Bengaluru, and Delhi-NCR will test whether the Rajasthan model scales. Success depends on distributor and brand participation — getting Dabur, ITC, HUL, and Nestlé onto the B2B procurement grid is the real bottleneck.

2. **ONDC's FY27 targets.** With 21.8 crore transactions in FY26 and 7.64 lakh sellers, ONDC needs to demonstrate accelerating growth in its next fiscal year to maintain investor and government confidence. The 900 million buyer target is a 4.5x jump from current levels. [^3]

3. **Competitive response.** Amazon and Flipkart have not been passive. Expect aggressive counter-measures: commission reductions, exclusive brand deals, and potential legal challenges to ONDC's governance structure. The National Traders' Welfare Board meeting suggests the government anticipates this and is preparing the institutional framework to support ONDC's defence. [^7]

4. **ONDC 2.0 and agentic commerce.** ONDC's leadership has publicly described a vision for "sovereign, agentic commerce" — AI agents that can autonomously search, negotiate, and transact across the open network on behalf of consumers. This aligns with India's broader "AI for All" strategy and could make ONDC the first population-scale testbed for AI-native commerce. [^3]

5. **International UPI-ONDC integration.** With UPI accepted across eight countries and expanding, the natural next step is ONDC adoption in those markets — allowing an Indian buyer in Dubai to discover and purchase from an ONDC-registered seller in Jaipur, settled via UPI international. This is speculative but technically feasible within the existing protocol architecture.

## Sources

- [^1]: [ONDC Architecture Deep Dive — pdpspectra](https://pdpspectra.com/blog/india-ondc-architecture-deep-dive)
- [^2]: [What Is ONDC? — IBM](https://www.ibm.com/think/topics/ondc)
- [^3]: [ONDC Secures Funding from Zoho, Paytm, BSE and Uber — Adil Zainulbhai, LinkedIn](https://www.linkedin.com/posts/adil-zainulbhai-6394544a_the-most-interesting-thing-about-ondcs-recent-activity-7468897068342738945-M5OP)
- [^4]: [Uber Launches Metro Ticketing via ONDC — APAC News Network](https://apacnewsnetwork.com/2026/06/uber-launches-metro-ticketing-via-ondc-begins-with-delhi-metro)
- [^5]: [Uber Invests in ONDC to Deepen Integration — Motoring Trends](https://motoring-trends.com/technology/uber-invests-in-ondc-to-deepen-integration-with-indias-digital-public-infrastructure)
- [^6]: [ONDC integrates Mumbai Metro, MMRC, BEST, Uber, Ola, State Transport — Dr. Sanjay Mukherjee, Facebook](https://www.facebook.com/drsanjaymukherjee/posts/thank-you-firstpost-america-for-this-international-recognition-mumbai-metros-mod/1024358829409979)
- [^7]: [National Traders' Welfare Board 10th Meeting — PIB](https://www.pib.gov.in/PressReleaseDetail.aspx?PRID=2277207&reg=1&lang=1)
- [^8]: [Piyush Goyal reviews ONDC and Nirmit Bharat — Piyush Goyal, LinkedIn](https://www.linkedin.com/posts/piyushgoyalofficial_held-a-review-meeting-with-the-officials-activity-7470504082114252802-83hh)
- [^9]: [Kerala Industries — ONDC Inter-Departmental Workshop, Facebook](https://www.facebook.com/IndustriesKerala/posts/ondc-is-a-pioneering-initiative-of-the-department-for-promotion-of-industry-and-/1013585044380033)
- [^10]: [Queen Máxima praises India's DPI — Instagram](https://www.instagram.com/p/DZ7KgkITPJY)
- [^11]: [ONDC Official — GitHub](https://github.com/ONDC-Official)
- [^12]: [Piyush Goyal on ONDC five-year targets — Facebook](https://www.facebook.com/PiyushGoyalOfficial/posts/held-a-review-meeting-with-the-officials-from-open-network-for-digital-commerce-/1569053034592110)
- [^13]: [UPI Statistics 2026 — CoinLaw](https://coinlaw.io/upi-statistics)
