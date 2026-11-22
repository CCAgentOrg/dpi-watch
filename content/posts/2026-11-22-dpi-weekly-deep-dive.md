---
title: "DPI Weekly Deep Dive — The Face That Fails: Supreme Court, UIDAI and the Right to Authenticate Independently | Week of November 16–22, 2026"
date: 2026-11-22T09:00:00+05:30
draft: false
tags: ["DPI", "Digital India", "Deep Dive", "Weekly", "Analysis", "Aadhaar", "UIDAI", "Accessibility", "Face Authentication", "Disability Rights"]
categories: ["Weekly Deep Dive"]
description: "2000-word analysis of the Supreme Court's contempt warning to Centre and UIDAI over Aadhaar face authentication that locks out blind and low-vision users — and what it reveals about India's identity layer as it scales past five billion transactions."
image: ""
---

# DPI Weekly Deep Dive — The Face That Fails: Supreme Court, UIDAI and the Right to Authenticate Independently | Week of November 16–22, 2026

## Executive Summary

On November 16, 2026, a Supreme Court bench of Justices J.B. Pardiwala and K.V. Chandran orally warned the Union government and UIDAI of contempt proceedings unless they filed a detailed response with a fixed timeline for making Aadhaar face authentication independently usable by blind and low-vision citizens.[^1][^2] The warning came in a Miscellaneous Application by advocate Amar Jain, who is blind, and who annexed to his filing something more damning than any argument: his own October 2026 credit-card e-KYC rejection — eighteen months after the Court's April 30, 2025 judgment in *Pragya Prasun v. Union of India* and *Amar Jain v. Union of India* had laid down twenty binding directions to make digital KYC accessible.[^3][^4]

This is not a niche disability dispute. It is a stress test of the identity layer of India's Digital Public Infrastructure at the exact moment that layer is scaling aggressively. Aadhaar face authentication — launched in October 2021 as a fallback for failed fingerprints — crossed 500 crore (five billion) cumulative transactions by September 2026, is integrated by nearly 200 entities, and became mandatory for subsidised LPG refills from October 1, 2026, reaching 89.9% of active LPG consumers before enforcement even began.[^5][^6][^7] Meanwhile the government's own ABHA health registry crossed 98.99 crore IDs, most created via Aadhaar-linked authentication flows.[^8] Every new mandate converts a modality that fails blind users into a gate on cooking gas, pensions, ration and banking.

The week's takeaway: India's DPI stack has an accessibility debt that is now being called at the highest court in the land. The technology works at population scale — but "population scale" is not the same as "every person," and the gap between the two is precisely where the Aadhaar Act's own safeguards (Sections 4(6) and 8(2)) were designed to operate. The Court's contempt threat converts a statutory promise into a deadline. What UIDAI files in response — and whether it includes audio-guided capture, liveness alternatives to eye-blink prompts, and a committed date — will define whether the identity layer remains an instrument of inclusion or acquires a permanent excluded class.

## The Story in Depth

### Context: The fallback that became the front door

Face authentication was designed as a patch. Fingerprint biometrics — the original Aadhaar modality — degrade with agricultural labour, age, and manual work; UIDAI's own field experience showed a meaningful share of residents could not authenticate reliably with fingers alone. In October 2021, UIDAI deployed an AI/ML-based face authentication system, developed in-house, as an additional modality: capture a live face image, run a liveness check, send the encrypted packet to UIDAI's Central Identities Data Repository (CIDR) for a 1:1 match against the Aadhaar photograph on file.[^9][^10]

The adoption curve since then is one of the steepest in the DPI stack. From 1.77 lakh transactions in FY2021-22, face authentication grew to 23.5 crore in FY2023-24; January 2025 crossed 12 crore in a single month; November 2025 hit 28.29 crore — more than double November 2024's 12.04 crore — and nearly 60% of pensioners' Digital Life Certificates that month were generated using the face modality.[^11][^12][^13] By September 2026, cumulative volume crossed 500 crore with nearly 200 entities on board — central and state departments, banks, NBFCs, telecom operators, brokerages, certifying authorities.[^5] Cumulative Aadhaar e-KYC now stands above 2,752 crore transactions.[^14]

The reason for the hockey stick is deliberate policy: face authentication is easier to mandate than fingerprint hardware. It needs only a smartphone camera, works on Android and iOS, and increasingly rides inside service-provider apps. The Petroleum Ministry's biometric Aadhaar authentication (BAA) mandate for subsidised LPG refills — effective October 1, 2026 — is the clearest example. Consumers authenticate through IndianOil ONE, HelloBPCL or HP PAY apps using the Aadhaar FaceRD app's face capture; 27.43 crore consumers, 89.9% of active domestic LPG consumers, had completed BAA by September 19, 2026, after a two-year outreach campaign involving over 12 crore SMS and WhatsApp messages.[^6][^7][^15] The same flow now gates pension proof-of-life, PDS, CoWIN, SIM issuance, banking e-KYC and, with ABHA at 98.99 crore IDs, the health layer.[^8][^13]

### What happened this week

Into this scaling story walked a contempt threat. On November 16, a bench of Justices Pardiwala and Chandran heard Amar Jain's Miscellaneous Application in the *Pragya Prasun*/*Amar Jain* proceedings. Jain's application followed a concrete, recent injury: a private bank rejected his credit-card application in October 2026 because he could not complete the blink-based liveness check in Aadhaar face authentication-driven e-KYC. His counsel annexed the rejection itself to the filing. The Court, while condoning the delay in filing the application, orally warned the Centre, UIDAI and the concerned authorities with contempt if they failed to file a detailed response covering: the steps taken since April 2025, the technology developed to address the accessibility gap, and a fixed timeline for implementation — with specific detail demanded on audio-guided interfaces and alternative verification modes.[^1][^2][^3]

The Court's oral framing was pointed: disability rights cannot be subordinated to technological convenience, and Aadhaar authentication is essential for welfare benefits, pensions, ration and banking — so a citizen who cannot complete the process independently is effectively excluded from those services.[^2] That is not an abstraction. The original April 2025 judgment (2025 INSC 599) arose from exactly this lived experience: acid attack survivor Pragya Prasun could not complete digital KYC for a SIM card because burn scarring defeated facial recognition and blink detection; Amar Jain, with 100% blindness, could not complete e-KYC at all.[^4][^16] The bench of Justices Pardiwala and R. Mahadevan issued twenty directions: alternative authentication methods, removal of the restrictive definition of "liveness," acceptance of thumb impressions as signature, periodic accessibility audits by certified professionals, involvement of blind users in user-acceptance testing, dedicated grievance redressal with human review of accessibility-based rejections, and paper-based/offline KYC fallbacks.[^3][^4]

The week also sharpened the institutional map of who owes compliance. The Reserve Bank of India did act after the 2025 judgment — an August 14, 2025 circular directed banks, NBFCs and regulated entities to comply — but that circular was withdrawn to consolidate instructions, and the obligation now lives inside the Responsible Business Conduct Directions issued November 28, 2025, which expressly require compliance with the April 30, 2025 judgment.[^17][^18] The problem: the RBI's clarifications on liveness apply to its regulated entities' video KYC processes. They do not reach UIDAI's face authentication pipeline itself, and they do not reach service providers who have hard-wired their customer journeys around a specific app or modality. UIDAI develops and regulates the authentication system; banks, telecom operators and oil marketing companies decide how to embed it. The 2025 judgment assigned duties to both — but as Jain's October 2025-and-after rejections show, the seam between the two is where citizens fall through.[^3]

A parallel application also pending before the Court challenges the Petroleum Ministry's LPG biometric mandate itself — the same October 1, 2026 policy that made face-linked authentication a precondition for subsidised refills.[^3] And on November 21, the week's DPI briefs recorded the broader context in which this fight lands: ABHA at 98.99 crore, UIDAI's free document-update window extended to June 14, 2027 (driving residents into update-and-authenticate flows), and states like Nagaland formally accepting Aadhaar app verifiable credentials as valid ID — every one of them another surface where the authentication moment repeats.[^8][^19]

### Why it matters

Three structural reasons elevate this story above the week's other DPI news (GeM cartelisation disclosure, ONDC's verticals pivot, CPGRAMS closure-quality disputes — all covered in this week's layer deep-dives).

**First, the identity layer is the dependency root of the stack.** Payments, health, welfare, telecom and commerce all authenticate through Aadhaar. A failure mode here is not one broken service; it is a broken prerequisite for dozens of services. The LPG mandate is the sharpest illustration: cooking gas is close to a universal household good, the subsidy is a near-universal entitlement, and the authentication gate now stands in front of it. When 89.9% compliance is reported as success, the correct reading is that 10% of active consumers — crores of households — had not authenticated before enforcement.[^7]

**Second, the excluded class is identifiable and measurable — which makes the failure unforgivable in a way random failures are not.** Blind and low-vision users, acid attack survivors, and people with facial disfigurement are not edge cases that appear in logs; they are constitutionally recognised rights-holders under the Rights of Persons with Disabilities Act, 2016, and they have told the state exactly who they are, in sworn filings, for two years. The Aadhaar Act itself already contains the answer: Section 4(6) requires requesting entities to inform users of alternative viable means of identification and prohibits denying a service solely because a person refuses or is unable to authenticate; the proviso to Section 8(2) mandates viable alternatives where authentication fails due to illness, injury, infirmity or technical reasons; Regulation 5 of the Aadhaar (Authentication and Offline Verification) Regulations, 2021 operationalises alternative identification.[^20][^21] The Court's 2025 judgment did not invent these duties — it constitutionalised them, holding digital accessibility a constitutional imperative flowing from dignity and equality.[^3]

**Third, the enforcement signal matters for every DPI layer watching.** India's DPI governance model relies heavily on circulars, sandbox guidance and voluntary adoption timelines. A contempt threat — the judiciary's most blunt instrument against executive inaction — signals that courts will convert soft compliance into hard deadlines when rights-holders return with receipts. That signal travels: to NPCI on UPI accessibility, to NHA on ABDM interfaces, to every DPI operator building citizen-facing flows without accessibility budgets.

## Technical Deep Dive

Understanding where accessibility breaks requires understanding the face authentication pipeline. In the classic architecture, a service provider (an Authentication User Agency, AUA) invokes the headless **Aadhaar FaceRD app** on the resident's device. FaceRD captures a live image, performs on-device processing and liveness detection, packages the face data encrypted, and hands it to the AUA's application, which forwards it to UIDAI's CIDR for a 1:1 biometric match against the stored photograph. The response returns digitally signed.[^9][^10][^22]

**Liveness is the choke point.** UIDAI's liveness detection uses AI/ML models checking for physical facial movement and depth cues; historically this meant prompting the user to blink, smile, or turn their head — randomized prompts to defeat photo and replay spoofing.[^10][^22] For a blind user, a visual prompt is invisible instruction: the app demands an action they cannot see was requested. The April 2025 judgment ordered that "liveness" be redefined beyond eye-blinking and that alternatives be provided; the RBI's circulars repeated this for V-CIP. But the FaceRD pipeline's prompts, error messaging, and failure handling are UIDAI's code, not the bank's — which is why eighteen months of RBI-side compliance did not fix the actual rejection experience.[^3][^17]

**The September 2026 SDK changes the attack surface — and the obligation.** At Global Fintech Fest 2026 (September 9), UIDAI launched the Aadhaar Face Authentication SDK and Sandbox: the face capture, liveness and anti-spoofing stack now embeds directly into provider apps on Android and iOS, eliminating the FaceRD app-switch. The Sandbox lets organisations test the full journey — provisioning, consent, capture, liveness, authentication, error handling, response validation, plus failure scenarios like network interruptions, invalid signatures and spoofing attempts — without external biometric hardware.[^5][^23] This is architecturally the right moment to fix accessibility: liveness UX is being rebuilt anyway, and the SDK's error-handling surface can carry audio guidance, extended timeouts, and non-visual prompt modes as first-class options. But nothing in the SDK launch materials committed to accessibility testing with blind users — precisely what the Court's UAT direction requires of regulated entities.[^3][^5]

**Scale cuts both ways.** UIDAI now handles roughly 10 crore authentications daily and is building capacity toward 25–30 crore per day; 2.49 crore devices are registered in the ecosystem.[^14][^24] A modality used at this volume sets defaults for the entire market: when face authentication becomes the cheapest KYC path, service providers converge on it, and the failure mode replicates across every adopting entity simultaneously. The SDK amplifies this — one accessibility-fixed capture stack, deployed once, propagates to hundreds of apps. Equally, an unfixed one propagates a blind spot into every integration.

## Government Perspective

The state's position is not hostile to accessibility on paper — it is split across three institutions with different clocks. **UIDAI/MeitY** own the authentication pipeline and have optimised relentlessly for scale: SDK, sandbox, onboarding playbook, entity count, transaction records. Accessibility fixes have not appeared in their public milestones; the Court now demands a technology-and-timeline response.[^1][^5] **RBI** moved earliest and most procedurally, folding the judgment into the RBC Directions — its limits are jurisdictional, not intentional.[^17][^18] **MoPNG** drove the most aggressive authentication mandate (LPG BAA), publicly framing it as leakage control — preventing diversion of subsidised cylinders to commercial use — with an explicit "not meant to deny genuine households" caveat and opt-out channels via web portals, WhatsApp chatbots and IVRS for those unwilling or unable to authenticate.[^6][^7]

That caveat is where the government's argument is weakest. An opt-out route that itself runs through digital channels (apps, chatbots, IVRS) is not a meaningful alternative for a user who cannot independently complete the primary flow and may also struggle with the fallback. Section 4(6) demands *viable* alternatives and an informed choice — not a menu of additional barriers. The pending challenge to the LPG mandate will test exactly this.[^3][^20]

There is also a budget question the response filing must answer. Accessibility is not free, but it is cheap relative to DPI budgets: audio-guided capture flows, non-visual liveness alternatives, human-review grievance desks. The April 2025 judgment's twenty directions were written to be implementable — the contempt stage exists because implementation, not feasibility, failed.

## Citizen Impact

For a blind or low-vision Indian in November 2026, the practical experience is a cascade of blocked essentials. A credit card application dies at the e-KYC step, as Jain's own filing documents.[^3] A subsidised LPG refill requires biometric authentication through an app whose face capture they cannot see; the delivery-agent assisted route exists but depends on the agent's presence and cooperation. A pension digital life certificate — 60% of which now flow through face authentication — can be impossible to generate without help.[^13] A new SIM, a bank account, a scholarship DBT: each begins with an authentication moment designed around a sense they do not have.

The deeper harm is dependency itself. As the Court noted previously and the accessibility filings reiterate, a citizen who must hand their phone to a stranger — or a shopkeeper, or an agent — to complete authentication has surrendered privacy and financial agency: their identity transaction is witnessed, their PIN and OTPs are exposed to whoever holds the device. For women, elderly people living alone, and rural users far from service points, assisted authentication is not a neutral workaround; it is an extractive intermediary inserted between citizen and entitlement.[^2][^4]

There is a countervailing citizen-interest the analysis must hold honestly: liveness checks exist to stop real fraud — photo spoofing, replay attacks, identity theft in e-KYC. Weak liveness harms the very welfare populations this piece centres, whose stolen identities feed ghost-beneficiary leakages. The policy answer is not to abolish liveness but to pluralise it — voice-liveness, motion-independent depth checks, assisted human verification with audit trails — so that security and accessibility stop trading off against each other. That is a technical specification, and it is what the Court has now demanded the government file.[^1]

## Global Context

India is not alone in building face-based identity at scale — but it is furthest along in building it *mandatory*. The EU's eIDAS 2.0 wallet framework carries explicit accessibility requirements in its technical specifications, and the EU Web Accessibility Directive governs public-sector digital services; Brazil's gov.br ID, the most comparable scale deployment, publishes accessibility conformance reports. The World Bank's ID4D programme has documented biometric exclusion systematically: fingerprint failure rates of 5–30% in field deployments across Africa and South Asia drove the industry toward face — and the same research stream now warns that facial systems introduce their own exclusion classes when liveness and capture UX assume sighted users.[^25][^26]

India's Unique Disability ID and rights framework (RPwD Act 2016) is, on paper, among the strongest globally; the *Pragya Prasun* judgment itself will likely be cited internationally as the most developed judicial articulation of digital accessibility as a constitutional right. The irony worth registering: the jurisdiction with the strongest legal doctrine on accessible digital identity is also the one where the doctrine is being tested against the world's largest biometric rollout. How UIDAI's response and implementation land will export a template — DPI is explicitly marketed abroad, through India Stack diplomacy and bilaterals, as a replicable public good. An identity layer with a known, court-documented excluded class is a defect that travels with the export.[^26]

## Looking Ahead

**The response filing is the first milestone.** The Court has asked for steps taken, technology developed, and a fixed timeline; contempt attaches if the response is evasive or the timeline imaginary. Watch for whether UIDAI commits to: audio-guided prompts in FaceRD/SDK, non-blink liveness alternatives in production (not pilot), published accessibility conformance reports, and a grievance desk with human review — the four concrete deliverables implied by the 2025 directions.[^1][^3]

**The LPG challenge will intersect.** If the main matter hardens into enforceable accessibility technology, the Petroleum Ministry's mandate will need to demonstrate its opt-out channels meet the "viable alternative" standard — or reopen the mandate's design.

**Watch the SDK accessibility release notes.** The September 2026 SDK is the pipeline's future; an accessibility-oriented SDK update (audio prompts, configurable liveness modes, screen-reader support) would be the cheapest path to population-wide fix, and its absence past the Court's deadline would be evidence of non-compliance by architecture.[^5][^23]

**And watch the numbers.** UIDAI's monthly releases celebrate face authentication growth; they do not publish authentication failure rates by modality, let alone by disability. An identity layer that measures success only in transaction counts cannot see its own exclusions. The most important reform this case could force is not a feature — it is a metric: exclusion-counting as a first-class DPI statistic. A stack that can report 500 crore successes but not its failure census is flying blind on the one number that defines inclusion.[^5][^11]

## Sources

[^1]: https://idtechwire.com/id-tech-digest-november-17-2026
[^2]: https://www.newindianexpress.com/india/2026/Nov/16/sc-warns-centre-uidai-of-contempt-over-lack-of-accessible-aadhaar-authentication-for-visually-impaired-persons
[^3]: https://www.scobserver.in/journal/making-aadhaar-accessible-for-everyone
[^4]: https://www.scconline.com/blog/post/2025/05/01/directives-issued-to-ease-digital-kyc-for-acid-attack-victims-visually-impaired-sc-legal-news
[^5]: https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=2308398
[^6]: https://ddnews.gov.in/en/biometric-aadhaar-authentication-mandatory-for-subsidised-lpg-refills-from-october-1
[^7]: https://www.thehindu.com/news/national/lpg-ekyc-deadline-how-to-complete-and-what-happens-if-you-dont-finish-it-by-october-1/article71499493.ece
[^8]: https://dpiwatch.cashlessconsumer.in/posts/2026-11-21-dpi-brief/
[^9]: https://www.microsave.net/wp-content/uploads/2024/10/240826_UIDAI_Unlocking_face_authentication_playbook_Digital_version.pdf
[^10]: https://blog.mantratec.com/Aadhaar-Face-Authentication-SDK-and-Sandbox
[^11]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2141878
[^12]: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2197605&reg=3&lang=1
[^13]: https://ddnews.gov.in/en/uidai-records-231-crore-aadhaar-authentication-transactions-in-november
[^14]: https://uidai.gov.in
[^15]: https://newsonair.gov.in/biometric-aadhaar-authentication-mandatory-for-subsidised-lpg-refills-from-october-1
[^16]: https://lawfoyer.in/pragya-prasun-ors-v-union-of-india-ors-2025-insc-599
[^17]: https://www.rbi.org.in/Scripts/NotificationUser.aspx?Id=12892&Mode=0
[^18]: https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=13141
[^19]: https://dpiwatch.cashlessconsumer.in/posts/2026-11-17-dpi-brief/
[^20]: https://indiankanoon.org/doc/80538569/
[^21]: https://api.sci.gov.in/assets/uploads/2025/05/2025_599_2025_9_1501_56588_Judgement_30-Apr-2025-67298.pdf
[^22]: https://aadhaarfacerd.en.aptoide.com/app
[^23]: https://www.biometricupdate.com/202609/uidai-expands-aadhaar-face-authentication-with-native-sdk-developer-sandbox
[^24]: https://www.facebook.com/sanjay.moody/posts/-uidai-makes-aadhaar-face-authentication-easier-for-developers-the-uidai-has-lau/38368965996051422
[^25]: https://www.medianama.com/2026/03/223-lpg-aadhaar-ekyc-mandate-india
[^26]: https://www.ibef.org/news/aadhaar-authentication-crosses-150-billion-transactions-powering-india-s-digital-economy-and-welfare-services
