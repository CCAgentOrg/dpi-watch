---
title: "Agent: DPI Watch Stock Market Summary"
date: 2026-03-11T09:00:00+05:30
draft: false
tags: ["Agents", "AI", "DPI", "Stocks", "GovTech", "India"]
categories: ["Agents"]
description: "Pre-market summary of India's Digital Public Infrastructure (DPI) stocks — UPI, Aadhaar, Digilocker, and GovTech enablers"
---

# 🤖 Agent: DPI Watch Stock Market Summary

## Overview

| Property | Value |
|----------|-------|
| **Name** | DPI Watch Stock Market Summary |
| **Blog** | DPI Watch — Digital Public Infrastructure |
| **Schedule** | **Market days (Mon-Fri) @ 8:15 AM IST** |
| **Coverage** | DPI Core, GovTech, Digital Identity, Infrastructure |
| **Model** | minimax-m2.5 |
| **Agent ID** | `TBD` |
| **Last Updated** | March 11, 2026 |

---

## Mission

Provide a quick 4-section summary of India's **Digital Public Infrastructure (DPI)** stocks:
1. **Indices** — Market direction (IT sector focus)
2. **DPI Core** — UPI, Aadhaar, Digilocker enablers
3. **GovTech** — Government IT implementation partners
4. **Digital Identity** — KYC, authentication, biometrics

**Timing**: Runs at **8:15 AM IST** — delivers before 8:45 AM pre-market open, alongside CashlessWatch Stock Market Summary.

---

## Oracle Sources

### Tier 1 (Primary - NSE India Official)
| Source | Endpoint | Data | Fallback |
|--------|----------|------|----------|
| NSE All Indices | `nseindia.com/api/allIndices` | Nifty IT, Nifty 50 | Yahoo Finance |
| NSE Equity | `nseindia.com/api/equity-stockIndices` | DPI stock quotes | Yahoo Finance |

### Tier 2 (Secondary)
| Source | Endpoint | Data | Reliability |
|--------|----------|------|-------------|
| Yahoo Finance | `query1.finance.yahoo.com` | All stocks | High |
| Moneycontrol | `moneycontrol.com` | Indian markets | HTML scraping |

### Tier 3 (Fallback)
| Source | Purpose |
|--------|---------|
| BSE India | If NSE fails |

---

## Stock Universe

### Indices
- Nifty IT (NSEIT) — Tech/DPI proxy
- Nifty 50 (NSEI) — Broad market
- BSE SME — Small DPI players

### Section 1: DPI Core — UPI, Aadhaar, Digilocker Enablers
| Symbol | Company | DPI Role | Why Included |
|--------|---------|----------|----------------|
| **PAYTM** | One97 Communications | UPI leader | 400M+ users, largest UPI volume |
| **INFIBEAM** | Infibeam Avenues | Enterprise payments | ONDC integration, government gateways |
| **NPST** | Network People Services | UPI infrastructure | Banking solutions, UPI rails |
| **FINOPB** | Fino Payments Bank | Payments bank | DBT disbursement, last-mile inclusion |

### Section 2: GovTech — Government IT Players
| Symbol | Company | GovTech Role | Key Projects |
|--------|---------|--------------|--------------|
| **TCS** | Tata Consultancy | Govt IT backbone | GST, MCA21, passport, tax systems |
| **INFY** | Infosys | Digital government | GSTN, income tax portal, Aadhaar integration |
| **WIPRO** | Wipro | Public sector tech | Election commission, census, e-courts |
| **TECHM** | Tech Mahindra | Smart infrastructure | Smart cities, defense IT, post offices |
| **HCLTECH** | HCL Technologies | Government cloud | Data centers, NIC, cybersecurity |
| **COFORGE** | Coforge | Digital citizen services | Passport seva, NIC projects, e-governance |
| **BSOFT** | Birlasoft | Tax & customs IT | GST, customs automation, RBI systems |
| **MINDTREE** | Mindtree | Rural digitization | CSCs, gram panchayat, rural banking |

### Section 3: Digital Identity — KYC, Auth, Biometrics
| Symbol | Company | Identity Role | DPI Connection |
|--------|---------|---------------|----------------|
| **PBFINTECH** | PB Fintech (PolicyBazaar) | KYC marketplace | Digital onboarding, CKYC, video KYC |
| **5PAISA** | 5paisa Capital | Digital KYC | Paperless account opening |
| **CAMS** | Computer Age Management | RTA/KYC infra | KYC data, investor identity |

### Section 4: Infrastructure — Cloud & Comms
| Symbol | Company | Infra Role | Gov Connection |
|--------|---------|------------|----------------|
| **TANLA** | Tanla Platforms | CPaaS | Govt SMS/OTP, COVID alerts, election |
| **ROUTE** | Route Mobile | Notification infra | Government messaging, Aadhaar OTP |

---

## Cross-Reference with CashlessWatch

Shared scrips that appear in both watches:

| Scrip | CashlessWatch Role | DPIWatch Role | Overlap Reason |
|-------|-------------------|---------------|----------------|
| **PAYTM** | Wallets, payments | UPI infrastructure | Payments backbone |
| **INFIBEAM** | Payment gateway | ONDC/Gov payments | Dual fintech/DPI play |
| **NPST** | Banking solutions | UPI rails | Banking DPI infrastructure |
| **PBFINTECH** | Insurance marketplace | KYC/Identity | Digital onboarding |
| **FINOPB** | Payments bank | DBT/Inclusion | Financial inclusion last-mile |

**Note**: When these stocks move, check both CashlessWatch (payments focus) and DPIWatch (infrastructure focus) contexts for complete picture.

---

## Agent Instruction (Source of Truth)

### Step 1: Run Helper Script
```bash
cd /home/.z/workspaces/con_PXCpywVCLwND9RsD/dpi-watch
./scripts/fetch-dpi-data.py --format all
```

### Step 2: Verify Output
Check that data was fetched for all 4 sections (18 stocks total)

### Step 3: Generate Hugo Post
```bash
./scripts/generate-hugo-post.py --input data/dpi_data_$(date +%Y%m%d).json
```

### Step 4: Send Telegram Alert
```bash
./scripts/send-dpi-alert.py --input data/dpi_data_$(date +%Y%m%d).json
```

### Step 5: Git Commit
```bash
git add content/posts/$(date +%Y-%m-%d)-dpi-watch.md
git commit -m "Add DPI Watch for $(date +%B %d, %Y)"
git push origin main
```

---

## Output Format

### Hugo Post
```yaml
---
title: "DPI Watch Stock Market Summary — March 11, 2026"
date: 2026-03-11T08:15:00+05:30
draft: false
tags: ["DPI", "Stocks", "GovTech", "UPI", "Aadhaar", "India"]
categories: ["DPI Watch"]
description: "Pre-market summary of India's Digital Public Infrastructure stocks: UPI, GovTech, and digital identity plays"
---

# DPI Watch — March 11, 2026

## 📊 INDICES
| Index | Level | Change | % Change |
|-------|-------|--------|----------|
| [Data] | [Data] | [Data] | [Data] |

## 🏛️ DPI CORE — UPI, Aadhaar, Digilocker
| Company | Symbol | Price | Change | % Change | Context |
|---------|--------|-------|--------|----------|---------|
| [Data] | [Data] | [Data] | [Data] | [Data] | [DPI news] |

## 🏢 GOVTECH — Government IT
| Company | Symbol | Price | Change | % Change | Context |
|---------|--------|-------|--------|----------|---------|
| [Data] | [Data] | [Data] | [Data] | [Data] | [Gov contracts] |

## 🔐 DIGITAL IDENTITY — KYC, Auth
| Company | Symbol | Price | Change | % Change | Context |
|---------|--------|-------|--------|----------|---------|
| [Data] | [Data] | [Data] | [Data] | [Data] | [Identity news] |

## ☁️ INFRASTRUCTURE — Cloud & Comms
| Company | Symbol | Price | Change | % Change | Context |
|---------|--------|-------|--------|----------|---------|
| [Data] | [Data] | [Data] | [Data] | [Data] | [Infra news] |

## 📰 DPI Sector News
- [Bullet points on NPCI, UIDAI, MeitY announcements]
- [Government contract wins/losses]
- [UPI/Digilocker updates]

## ⚠️ DISCLAIMER
**Not investment advice. For informational purposes only.**
Data timestamp: 08:15 AM IST — before pre-market (08:45 AM)
```

### Telegram Alert (Compact)
```
🏛️ DPI WATCH — March 11, 2026 | 08:15 AM
━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📊 INDICES
• Nifty IT: [Level] [Change]
• Nifty 50: [Level] [Change]

🏛️ DPI CORE
• PAYTM: [Price] [Change] — UPI context
• INFIBEAM: [Price] [Change] — ONDC context
• NPST: [Price] [Change]
• FINOPB: [Price] [Change]

🏢 GOVTECH (Top 3)
• TCS: [Price] [Change]
• INFY: [Price] [Change]
• WIPRO: [Price] [Change]

📰 DPI News
• [Top 3 bullet points]

⚠️ Not investment advice
📎 Full report: [GitHub URL]
```

---

## Helper Scripts

All scripts in `scripts/` folder:

| Script | Purpose | Output |
|--------|---------|--------|
| `fetch-dpi-data.py` | Fetch from oracle sources | `data/dpi_data_YYYYMMDD.json` |
| `generate-hugo-post.py` | Create Hugo markdown | `content/posts/YYYY-MM-DD-dpi-watch.md` |
| `send-dpi-alert.py` | Telegram alert | Telegram message |

---

## Quality Checks

- [ ] All indices fetched (Nifty IT, Nifty 50)
- [ ] All 4 DPI Core stocks have data (PAYTM, INFIBEAM, NPST, FINOPB)
- [ ] At least 5 GovTech stocks have data
- [ ] Prices cross-verified with NSE/Moneycontrol
- [ ] % change calculations correct
- [ ] Telegram alert sent by 08:20 AM IST (before 08:45 AM pre-market)
- [ ] Hugo post committed to repository

---

## Data Fallback Strategy

If primary source fails:
1. **NSE India** → Use Yahoo Finance
2. **Yahoo Finance** → Use Moneycontrol HTML scraping
3. **Both fail** → Mark as "Data delayed" in output

---

## Version History

| Date | Change | Commit |
|------|--------|--------|
| 2026-03-11 | Initial agent creation with 18 DPI stocks | [TBD] |
| 2026-03-11 | Schedule aligned to 8:15 AM IST (pre-market ready) | [TBD] |

---

*This agent is part of the CashlessConsumer DPI Watch project. All agent instructions are open source.*
