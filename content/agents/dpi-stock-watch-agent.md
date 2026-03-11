---
title: "Agent: DPI Watch Stock Market Summary"
date: 2026-03-11T09:00:00+05:30
draft: false
tags: ["Agents", "AI", "DPI", "Digital Public Infrastructure", "Stocks"]
categories: ["Agents"]
description: "Pre-market summary of Indian DPI (Digital Public Infrastructure) related stocks, government tech, and digital identity plays"
---

# 🤖 Agent: DPI Watch Stock Market Summary

## Overview

| Property | Value |
|----------|-------|
| **Name** | DPI Watch Stock Market Summary |
| **Blog** | DPI Watch |
| **Schedule** | Market days (Mon-Fri) @ 9:00 AM IST |
| **Coverage** | DPI stocks, GovTech, Digital Identity, UPI Infrastructure |
| **Model** | vercel:minimax/minimax-m2.5 |
| **Agent ID** | `dpi-stock-watch-001` |
| **Last Updated** | March 11, 2026 |

---

## Mission

Provide a focused summary of Indian stocks related to **Digital Public Infrastructure (DPI)** — the backbone of India's digital economy:
1. **Indices** — Market direction (Nifty IT, Nifty 50)
2. **DPI Core** — UPI, Aadhaar, Digilocker enablers
3. **GovTech** — Government IT, e-governance players
4. **Digital Identity** — Authentication, KYC, biometrics

---

## Oracle Sources

### Tier 1 (Primary - Official)
| Source | Endpoint | Data |
|--------|----------|------|
| NSE All Indices | `nseindia.com/api/allIndices` | Nifty IT, Nifty 50 |
| NSE Equity | `nseindia.com/api/equity-stockIndices` | Stock quotes |
| BSE India | `bseindia.com` | SME stocks |

### Tier 2 (Secondary)
| Source | Purpose |
|--------|---------|
| Yahoo Finance | Global data, no auth |
| Moneycontrol | Indian markets |
| Screener.in | Fundamental data |

---

## DPI Stock Universe

### 📊 INDICES
- Nifty IT (NSEIT) — Tech/DPI proxy
- Nifty 50 (NSEI) — Broad market
- BSE SME — Small DPI players

### 🏛️ TIER 1: DPI Core Enablers
| Symbol | Company | DPI Role | Why Watch |
|--------|---------|----------|-----------|
| **PAYTM** | One97 Communications | UPI leader, payments infra | 400M+ users, UPI volume |
| **INFIBEAM** | Infibeam Avenues | Enterprise payments, ONDC | Govt e-marketplace tech |
| **NPST** | Network People Services | UPI infrastructure | Banking/DPI solutions |
| **FINOPB** | Fino Payments Bank | Payments bank, DBT | Financial inclusion |

### 🏢 TIER 2: GovTech & E-Governance
| Symbol | Company | GovTech Role | Why Watch |
|--------|---------|--------------|-----------|
| **TCS** | Tata Consultancy | Govt IT projects, GST, MCA | Largest govtech vendor |
| **INFY** | Infosys | GSTN, income tax, passport | Digital govt backbone |
| **WIPRO** | Wipro | Election tech, census, e-courts | Govt digitization |
| **TECHM** | Tech Mahindra | Smart cities, defense IT | Urban DPI infra |
| **HCLTECH** | HCL Technologies | Govt cloud, data centers | Sovereign cloud |
| **COFORGE** | Coforge | Passport seva, NIC | e-gov platforms |
| **BSOFT** | Birlasoft | GST, customs, RBI systems | Financial infra |
| **MINDTREE** | Mindtree | Rural digitization, CSC | Last-mile DPI |

### 🔐 TIER 3: Digital Identity & Authentication
| Symbol | Company | Identity Role | Why Watch |
|--------|---------|---------------|-----------|
| **PBFINTECH** | PB Fintech | KYC, digital onboarding | Insurance/KYC leader |
| **5PAISA** | 5paisa Capital | Digital KYC, onboarding | Brokerage tech |
| **CAMS** | Computer Age | RTA, KYC infrastructure | Mutual fund KYC |
| **KARURVYSYA** | Karur Vysya Bank | Aadhaar-enabled payments | APB, DBT rails |
| **FEDERALBNK** | Federal Bank | Video KYC pioneer | Digital onboarding |

### ☁️ TIER 4: Cloud & Data Infrastructure
| Symbol | Company | Infrastructure Role | Why Watch |
|--------|---------|---------------------|-----------|
| **TANLA** | Tanla Platforms | CPaaS, government SMS | OTP infra, trai norms |
| **ROUTE** | Route Mobile | Govt notification infra | Critical comms |
| **DATAPATTNS** | Data Patterns | Defense/ISRO tech | Sovereign hardware |
| **ZAGGLE** | Zaggle Prepaid | Corporate DPI, DBT | Prepaid instruments |

### 🚫 EXCLUDED (Peripheral to DPI)
- Pure banks without govtech focus
- Generic IT without public infra angle
- E-commerce not enabling DPI

---

## Cross-Reference with CashlessWatch

**Sync with CashlessWatch agents:**
- Daily Fintech Brief: Check for RBI/NPCI/DPI policy news
- Stock Watch: Compare fintech vs DPI stock movements

**Shared Scrips:**
| Scrip | CashlessWatch | DPIWatch | Role |
|-------|--------------|----------|------|
| PAYTM | ✅ Wallets | ✅ UPI infra | Payments backbone |
| INFIBEAM | ✅ Gateways | ✅ ONDC/Gov | Dual play |
| NPST | ✅ Infrastructure | ✅ UPI rails | Banking DPI |
| PBFINTECH | ✅ Insurance | ✅ KYC/Identity | Digital onboarding |
| FINOPB | ✅ Payments Bank | ✅ DBT/Financial inclusion | Last-mile |

---

## Agent Instruction

### Step 1: Fetch Market Data
```bash
cd /home/.z/workspaces/con_PXCpywVCLwND9RsD/dpi-watch
python3 scripts/fetch-dpi-data.py
```

### Step 2: Check DPI News
Read CashlessWatch Daily Brief for:
- NPCI/UPI announcements
- Aadhaar updates
- Digilocker news
- Government IT tenders
- RBI DPI circulars

### Step 3: Generate Summary
Create Hugo post at `content/posts/YYYY-MM-DD-dpi-watch.md`

### Step 4: Send Telegram Alert
```bash
python3 scripts/send-dpi-alert.py
```

### Step 5: Commit & Push
```bash
git add content/posts/YYYY-MM-DD-dpi-watch.md
git commit -m "Add DPI Watch for $(date +%B %d, %Y)"
git push origin main
```

---

## Output Format

### Hugo Post Template
```yaml
---
title: "DPI Watch — March 11, 2026"
date: 2026-03-11T09:00:00+05:30
draft: false
tags: ["DPI", "Digital Public Infrastructure", "GovTech", "Stocks"]
categories: ["DPI Watch"]
description: "Pre-market summary of DPI stocks, government tech, and digital identity plays"
---

# DPI Watch — March 11, 2026

## 📊 INDICES
| Index | Level | Change | % Change |
|-------|-------|--------|----------|
| Nifty IT | ... | ... | ... |
| Nifty 50 | ... | ... | ... |

## 🏛️ DPI CORE — UPI, Aadhaar, Digilocker Enablers
| Company | Symbol | Price | Change | % Change | DPI Context |
|---------|--------|-------|--------|----------|-------------|
| ... | ... | ... | ... | ... | ... |

## 🏢 GOVTECH — Government IT Players
| Company | Symbol | Price | Change | % Change | Gov Context |
|---------|--------|-------|--------|----------|-------------|
| ... | ... | ... | ... | ... | ... |

## 🔐 DIGITAL IDENTITY — KYC, Auth, Biometrics
| Company | Symbol | Price | Change | % Change | ID Context |
|---------|--------|-------|--------|----------|------------|
| ... | ... | ... | ... | ... | ... |

## 📰 DPI News Impact
- [NPCI/UPI news]
- [Aadhaar updates]
- [Government IT tenders]
- [RBI DPI circulars]

## 🔗 CashlessWatch Cross-Reference
- Shared scrips movement
- Sector correlation
- Policy impact comparison

---
*Sources: NSE, BSE, Moneycontrol, CashlessWatch*
*Not investment advice*
```

### Telegram Alert (Compact)
```
🏛️ DPI WATCH — March 11, 2026
━━━━━━━━━━━━━━━━━━━━

📊 INDICES
Nifty IT:   [Level] [Change]
Nifty 50:   [Level] [Change]

🏛️ DPI CORE
PAYTM:   [Price] [Change] — UPI leader
INFIBEAM: [Price] [Change] — ONDC play
NPST:    [Price] [Change] — UPI infra
FINOPB:  [Price] [Change] — Payments bank

📰 DPI News
• [Bullet points from CashlessWatch]

🔗 Cross-watch with CashlessWatch
📎 Full report: [GitHub link]
```

---

## Version History

| Date | Change |
|------|--------|
| 2026-03-11 | Initial agent creation with 18 DPI stocks |

---

*This agent is part of the DPI Watch project. All agent instructions are open source.*
