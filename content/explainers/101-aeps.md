---
title: "AePS 101: Aadhaar-Enabled Banking at the Last Mile"
description: "A fact-checked guide to the Aadhaar Enabled Payment System—how its bank-agent network works, what NPCI's published data shows, and the implications for inclusion, privacy, authentication failure, and grievance redress."
date: 2026-10-22
draft: false
tags: ["aeps", "aadhaar", "npci", "banking", "financial-inclusion", "digital-public-infrastructure", "privacy", "india"]
categories: ["DPI Basics"]
author: "CashlessConsumer"
readingTime: "14 min"
---

# AePS 101: Aadhaar-Enabled Banking at the Last Mile

## What is AePS?

The **Aadhaar Enabled Payment System (AePS)** is a bank-led service for basic banking through an authorised Business Correspondent (BC), also called a Bank Mitra, at an AePS touchpoint such as a micro-ATM. A customer can use an Aadhaar-enabled bank account to make a transaction at a participating bank's touchpoint, with Aadhaar authentication. NPCI operates the interoperable switching and settlement layer; the customer's bank remains responsible for the account and its transaction response. AePS is a payment rail and assisted service—not a stand-alone consumer app. [^1][^2][^3][^4]

The core services include cash withdrawal and deposit, balance enquiry, mini statement and Aadhaar-to-Aadhaar fund transfer. NPCI documentation also describes non-financial functions such as Best Finger Detection and e-KYC. The service is designed to bring basic banking closer to people who may be far from a bank branch or ATM; that is its stated inclusion rationale, not proof that every person can access it reliably or affordably. [^1][^3][^4]

**AePS is not the Aadhaar Payments Bridge System (APBS).** AePS lets a customer initiate banking at a touchpoint. APBS is a separate payment system used to route certain government benefit credits to Aadhaar-linked accounts. **BHIM Aadhaar Pay** is a merchant-payment service; NPCI's retail statistics group it with other AePS financial transactions in one table, so its figures should not all be read as cash withdrawals. [^4][^5]

RBI records AePS as operational since **January 2011**. Its 2021 payment-systems booklet describes the original split of roles: UIDAI performs biometric authentication, while NPCI handles switching, clearing and settlement. The current service still depends on these distinct identity, bank-account and payment-network functions. [^4]

## How it works

1. **The customer chooses a touchpoint and service.** AePS is delivered in assisted mode by a BC/Bank Mitra at an eligible micro-ATM or other authorised touchpoint. Touchpoints may be fixed or mobile. [^2][^4]
2. **The customer identifies the bank account to use.** The AePS product booklet lists an Aadhaar number or Virtual ID (VID), the bank name/issuer identification number, the transaction type and—where relevant—the amount. The account must be enabled for Aadhaar-based access. NPCI lists VID as an option, but support can depend on the particular bank and touchpoint. [^2]
3. **The customer authenticates.** A transaction uses the biometric captured at the touchpoint; RBI's 2025 directions also refer to Aadhaar authentication using biometrics or OTP. The exact method offered depends on the participating bank and service. The customer should be told what is being requested before approving it. [^2][^6][^7]
4. **The request is routed and answered.** UIDAI authentication checks the submitted identity information. NPCI's switch routes the transaction to the bank that holds the account; that bank returns an approval or decline and processes the account debit or credit. In an inter-bank transaction, the customer may use another bank's touchpoint, but the account-holding bank still serves the account. [^1][^4]
5. **The customer checks the result.** For a financial transaction, keep the receipt or transaction reference and check the account balance or statement. An authentication response is not itself proof that money was credited or debited correctly; the account-holding bank's ledger is the place to verify the money movement. [^1][^4]

## Key Statistics

NPCI's retail-payments table reports the following **inter-bank AePS financial transactions over micro-ATMs**. FY2024–25 is the latest complete annual series used here; NPCI's live product-statistics dashboard provides more recent monthly indicators, but it measures a broader mix of activity. [^5][^8]

| Measure | FY2023–24 | FY2024–25 | What it measures |
|---|---:|---:|---|
| All listed AePS inter-bank financial transactions | 1,197.05 million; ₹3,210.03 billion | 1,258.20 million; ₹3,417.63 billion | Cash withdrawal/deposit and the table's other grouped AePS categories |
| Cash withdrawals | 1,175.71 million; ₹3,140.36 billion | 1,235.51 million; ₹3,343.98 billion | Withdrawal count and value |
| Cash deposits | 1.51 million; ₹5.80 billion | 0.64 million; ₹2.18 billion | Deposit count and value |
| Other: fund transfers and BHIM Aadhaar Pay | 19.85 million; ₹63.86 billion | 22.05 million; ₹71.48 billion | The table combines these categories |

The total inter-bank transaction volume rose by about **5.1%** between FY2023–24 and FY2024–25; the value rose by about **6.5%**. These percentages are calculations from NPCI's published annual totals. They are not unique-user counts, and they do not show whether a transaction was initiated by a distinct person. NPCI's public tables do not provide, alongside these totals, a national count of authentication failures, disputed transactions, fraud losses or people unable to use a touchpoint. The absence of those measures is a transparency gap, not evidence that the underlying rates are zero. [^5][^8]

**Why other NPCI totals look different:** For September 2026, the product dashboard reports **508.58 million total approved transactions**: 193.21 million approved off-us transactions worth ₹23,211 crore, 313.55 million on-us authentication transactions, and 1.82 million BHIM Aadhaar Pay transactions. Those categories sum to the dashboard's total, but on-us authentication events are not equivalent to money movements. The 1,258.20 million FY2024–25 figure above is specifically the retail table's annual inter-bank financial-transactions count. The two totals are not directly comparable. [^5][^8]

**Scope caveat:** the annual figures above cover the retail table's inter-bank financial transactions over micro-ATMs. They should not be described as all AePS activity, all Aadhaar authentications, or all welfare transfers. NPCI warns that monthly and daily figures are rounded, so small discrepancies can occur when totals are reconstructed from sub-periods. [^5][^8]

## Layers Classification (L1-L7)

This is DPI Watch's analytical mapping, not an official government or NPCI taxonomy.

| Layer | Classification | AePS's role |
|---|---|---|
| **L1 — Vision & policy** | Financial inclusion policy | Extends basic banking through interoperable, assisted touchpoints; this is the system's stated purpose. [^1][^4] |
| **L2 — Regulation** | Rules and accountability | RBI payment-system oversight and its AePS Touchpoint Operator directions; Aadhaar Act and UIDAI authentication rules apply to Aadhaar authentication. [^6][^7] |
| **L3 — Digital rails** | Core infrastructure | NPCI's switch and settlement arrangements connect the acquiring touchpoint to the account-holding bank, while UIDAI provides authentication. [^1][^4] |
| **L4 — APIs & protocols** | Interfaces and standards | AePS transaction and authentication specifications connect touchpoint devices, banks, NPCI and UIDAI. RBI requires controls so technological integrations such as APIs are used only for AePS operations. [^2][^6] |
| **L5 — Applications & access points** | User-facing systems | Banks and their onboarded operators provide fixed or mobile touchpoints, including micro-ATMs; this is an assisted service, not a single national consumer app. [^1][^2][^6] |
| **L6 — Use cases** | Banking services | Cash withdrawal/deposit, balance enquiry, mini statement and Aadhaar-to-Aadhaar transfer; merchant payment via BHIM Aadhaar Pay is related but distinct. [^1][^4][^5] |
| **L7 — Analytics & oversight** | Monitoring and reporting | Banks monitor operator transactions and risk; NPCI publishes aggregate transaction statistics. The public series cited here does not provide failure, fraud-loss or exclusion rates. [^8][^5][^6] |

## Regulatory Framework

**Payment-system and operator oversight.** AePS is operated by NPCI under RBI's payment-system regulatory framework. RBI's **AePS – Due Diligence of AePS Touchpoint Operators Directions, 2025**, effective from **1 January 2026**, require acquiring banks to conduct due diligence and KYC of operators before onboarding and periodically thereafter. Banks must re-check an operator's KYC before reactivating an operator who has been inactive for three continuous months, monitor operator activity on an ongoing basis, and set risk-based operational parameters. RBI cited reports of fraud involving identity theft or compromise of customer credentials as context for these controls, but the directions do not publish a fraud count or loss estimate. The rules establish safeguards, not proof of how many cases they prevent or resolve. [^6]

**Aadhaar authentication and alternatives.** Section 8 of the Aadhaar Act requires a requesting entity, subject to statutory exceptions, to obtain consent before collecting identity information for authentication, tell the person what information is shared and how it will be used, and inform them of alternatives. If authentication fails for reasons such as age, illness, disability or technical failure, the requesting entity must provide an alternative means of identification; section 8(6) says a service must not be denied because the person refuses or is unable to authenticate. The Act also restricts the sharing and use of core biometric information. [^7]

**Privacy and data-protection law.** The Supreme Court recognised privacy as a fundamental right in *Justice K.S. Puttaswamy (Retd.) v. Union of India*. The Digital Personal Data Protection Act, 2023 and Rules, 2025 have a staggered commencement: as of **22 October 2026**, some institutional provisions are in force, but the main personal-data processing duties and data-principal rights in sections 3–17 are scheduled to commence eighteen months after the November 2025 Gazette notification, in **May 2027**. The Rules follow their own schedule: rules 1, 2 and 17–21 commenced on publication; rule 4 is due after one year; and rules 3, 5–16, 22 and 23 are due after eighteen months. “Notified” therefore does not mean every DPDP right is already operative. [^9][^10][^11]

## Citizen Rights Analysis

### What the design can improve

- **Local access without a card or personal smartphone.** An assisted banking point can let a customer withdraw cash or check an account without travelling to a branch or operating an app personally. This is the service's inclusion rationale; the public volume totals do not measure how far travel fell or who remains unserved. [^1][^4]
- **Interoperability.** NPCI describes AePS as usable at a participating bank's touchpoint for an Aadhaar-enabled account held elsewhere. This can reduce dependence on a single bank's local branch network. [^1][^4]
- **A legal right to an alternative when authentication fails.** The Aadhaar Act says an authentication failure must not, by itself, lead to denial of the service and requires an alternative identification method in the circumstances specified by law. A customer can point to this rule when a service operator treats a failed biometric as the end of the process. [^7]

### What deserves scrutiny

- **A biometric match is not the same as a person's free and informed consent to every transaction.** The customer should see the service type and amount before authentication. A fingerprint match establishes an authentication result; it does not prove that an operator explained the transaction or that the customer understood it. This is a rights-and-design concern, not a claim that every AePS operator misbehaves. [^2][^7]
- **The assisted model creates a local power imbalance.** The operator is present while the customer identifies an account, chooses an action and authenticates. That can help people who need assistance, but it also makes clear receipts, visible amounts, private transaction space and a way to complain especially important. [^1][^2]
- **Authentication can fail for the people who most need cash access.** Fingerprint condition, device quality, connectivity or service availability can interrupt a transaction. NPCI describes a Best Finger Detection process, and the Aadhaar Act requires alternatives in specified failure circumstances, but the NPCI statistics cited above do not quantify AePS-specific failure or retry rates. [^2][^5][^7]
- **Public reporting is incomplete for citizen oversight.** Aggregate transaction counts and values show system use, not whether people received the right amount, encountered failed authentication, paid extra charges, or recovered money after a dispute. Publicly comparable metrics for these outcomes would make inclusion and safety claims testable. [^8][^5]

## Privacy Implications

AePS connects an identity credential to a bank account and a specific action such as withdrawal, deposit or balance enquiry. Transaction logs can therefore be sensitive even when the service does not expose the full account number. At the physical touchpoint, the operator and anyone nearby may see the customer's action, amount or receipt; account statements and balance information deserve particular care. This is a risk inherent in an assisted financial service, not evidence that NPCI or UIDAI makes every transaction log publicly visible. [^1][^2][^4]

Biometrics are not like a password that a customer can simply replace after exposure. The Aadhaar Act restricts the sharing and use of core biometric information, and the authentication response must not include core biometric information. However, citizens still need clear answers about the biometric capture device, the transaction records kept by each participant, access controls, retention periods and incident reporting. The cited public AePS materials do not quantify those system-wide privacy outcomes. [^7]

UIDAI provides Aadhaar authentication-history and biometric lock/unlock services. Locking biometrics can block biometric authentication—including a biometric AePS transaction—until the holder unlocks them; it is a control to weigh against the convenience of using biometric services, not a substitute for checking bank transactions or reporting fraud. [^12]

## Safeguards

- Check the amount and transaction type before authenticating; do not approve a transaction that the operator has not explained. Ask for a receipt or transaction reference and verify the debit or credit in the account-holding bank's statement. [^1][^2]
- Where supported, ask whether the touchpoint accepts a **Virtual ID (VID)** instead of the Aadhaar number. NPCI's product documentation lists VID, but support may vary by bank or terminal. [^2]
- Review Aadhaar authentication history and consider UIDAI's biometric lock/unlock service if you do not expect to use biometric authentication. Be aware that locking may prevent a biometric AePS transaction until the biometrics are unlocked. [^12]
- If an SMS or statement shows a transaction you did not authorise, report it to the account-holding bank immediately and keep the complaint acknowledgement. RBI's customer-liability directions make prompt reporting important; the bank must assess liability under the applicable rules and its approved policy. [^13]
- Banks and touchpoint operators should make fees and transaction amounts visible, provide an accessible alternative when Aadhaar authentication fails as required by law, issue a receipt, protect customers' transaction privacy, and make the complaint path clear. [^6][^7]

## Complaints & Grievance Redressal

1. **For a wrong or unauthorised debit, contact the bank that holds the account first.** Report the transaction promptly, give the date, amount and reference number, and ask for a complaint number and written status. Prompt reporting matters under RBI's unauthorised electronic-banking transaction framework. [^13]
2. **For an operator or touchpoint problem, also complain to the acquiring bank**—the bank that onboarded the operator. RBI assigns that bank due-diligence and ongoing monitoring responsibilities. If you do not know which bank acquired the touchpoint, ask your account-holding bank to identify the channel and route the complaint. [^6]
3. **Escalate to the RBI Ombudsman if the bank does not resolve the complaint.** Under the Reserve Bank – Integrated Ombudsman Scheme, 2026, first approach the regulated entity. You may then complain if you receive no reply within 30 days—or the longer time specified by RBI, NPCI or card-network guidelines—or if you are dissatisfied with the reply. File within 90 days after that applicable period expires or the bank's last communication, whichever is later. Complaints can be filed through the RBI CMS portal. [^14]
4. **For Aadhaar authentication-history or biometric-lock issues, contact UIDAI.** UIDAI's Aadhaar service portal and helpline **1947** cover Aadhaar services; the bank remains the first route for disputing a missing or unauthorised account transaction. [^12][^13]

## Prime References

[^1]: NPCI, [AePS product overview](https://www.npci.org.in/what-we-do/aeps/product-overview).
[^2]: NPCI, [AePS Product Booklet](https://www.npci.org.in/PDF/AePS/Product-Booklet.pdf).
[^3]: NPCI, [AePS frequently asked questions](https://www.npci.org.in/what-we-do/aeps/faqs).
[^4]: Reserve Bank of India, [Payment and Settlement Systems in India: Journey in the Second Decade of the Millennium](https://rbidocs.rbi.org.in/rdocs/Publications/PDFs/PSSBOOKLET93D3AEFDEAF14044BC1BB36662C41A8C.PDF).
[^5]: NPCI, [Retail Payments Statistics on NPCI Platforms](https://www.npci.org.in/uploads/RETAIL_PAYMENTS_STATISTICS_1_xlsx_de91fc7ec0.pdf).
[^6]: Reserve Bank of India, [AePS – Due Diligence of AePS Touchpoint Operators, 27 June 2025](https://www.rbi.org.in/scripts/RTGS_Notification.aspx?Id=12877).
[^7]: UIDAI, [The Aadhaar Act, 2016, as amended](https://uidai.gov.in/en/aadhaar-act).
[^8]: NPCI, [AePS Product Statistics dashboard](https://www.npci.org.in/product/aeps/product-statistics).
[^9]: Supreme Court of India, [Justice K.S. Puttaswamy (Retd.) v. Union of India, 24 August 2017](https://api.sci.gov.in/supremecourt/2012/35071/35071_2012_Judgement_24-Aug-2017.pdf).
[^10]: Ministry of Electronics and Information Technology, [G.S.R. 843(E), DPDP Act commencement notification, 13 November 2025](https://www.meity.gov.in/static/uploads/2025/11/c56ceae6c383460ca69577428d36828b.pdf).
[^11]: Ministry of Electronics and Information Technology, [Digital Personal Data Protection Rules, 2025](https://www.meity.gov.in/static/uploads/2025/11/53450e6e5dc0bfa85ebd78686cadad39.pdf).
[^12]: UIDAI, [My Aadhaar: authentication history and biometric lock/unlock services](https://uidai.gov.in/en/my-aadhaar).
[^13]: Reserve Bank of India, [Customer Protection – Limiting Liability of Customers in Unauthorised Electronic Banking Transactions](https://www.rbi.org.in/scripts/notificationuser.aspx?id=11040).
[^14]: Reserve Bank of India, [Reserve Bank – Integrated Ombudsman Scheme, 2026: FAQs](https://www.rbi.org.in/commonman/Upload/English/FAQs/PDFs/RBIOS01072026.pdf).

---

*Fact-check date: 22 October 2026. This explainer distinguishes published transaction totals from unreported failure, fraud and inclusion outcomes, and separates AePS from APBS and BHIM Aadhaar Pay.*
