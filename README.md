# DPI Watch — Digital Public Infrastructure Stock Monitoring

📊 **Daily pre-market summary of India's Digital Public Infrastructure (DPI) stocks.**

---

## 📋 Overview

| Property | Value |
|----------|-------|
| **Name** | DPI Watch |
| **Focus** | India's Digital Public Infrastructure stocks |
| **Schedule** | **8:15 AM IST, market days (Mon-Fri)** — before 8:45 AM pre-market |
| **Format** | 4-section summary: Indices → DPI Core → GovTech → Identity |
| **Delivery** | Telegram alert + Hugo blog post |
| **Repository** | https://github.com/CCAgentOrg/dpi-watch |

---

## 🏛️ DPI Stock Universe (18 Stocks)

### DPI Core — UPI, Aadhaar, Digilocker Enablers
| Symbol | Company | Role |
|--------|---------|------|
| **PAYTM** | One97 Communications | UPI leader, 400M+ users |
| **INFIBEAM** | Infibeam Avenues | ONDC, government payments |
| **NPST** | Network People Services | UPI infrastructure |
| **FINOPB** | Fino Payments Bank | DBT, last-mile inclusion |

### GovTech — Government IT Players
| Symbol | Company | Role |
|--------|---------|------|
| **TCS** | Tata Consultancy | GST, MCA21, passport |
| **INFY** | Infosys | GSTN, income tax, Aadhaar |
| **WIPRO** | Wipro | Election, census, e-courts |
| **TECHM** | Tech Mahindra | Smart cities, defense |
| **HCLTECH** | HCL Technologies | NIC, cloud, cybersecurity |
| **COFORGE** | Coforge | Passport seva, NIC |
| **BSOFT** | Birlasoft | GST, customs, RBI systems |
| **MINDTREE** | Mindtree | Rural digitization, CSC |

### Digital Identity — KYC, Auth
| Symbol | Company | Role |
|--------|---------|------|
| **PBFINTECH** | PB Fintech | KYC marketplace |
| **5PAISA** | 5paisa Capital | Digital onboarding |
| **CAMS** | Computer Age | RTA, KYC infrastructure |

### Infrastructure — Cloud & Comms
| Symbol | Company | Role |
|--------|---------|------|
| **TANLA** | Tanla Platforms | CPaaS, gov SMS/OTP |
| **ROUTE** | Route Mobile | Notification infra |

---

## 🔗 Cross-Reference with CashlessWatch

| Scrip | CashlessWatch | DPIWatch | Context |
|-------|--------------|----------|---------|
| **PAYTM** | Wallets | UPI infra | Payments backbone |
| **INFIBEAM** | Gateways | ONDC/Gov | Dual play |
| **NPST** | Banking | UPI rails | Banking DPI |
| **PBFINTECH** | Insurance | KYC | Digital onboarding |
| **FINOPB** | Payments Bank | DBT | Last-mile inclusion |

---

## 📁 Repository Structure

```
dpi-watch/
├── content/
│   ├── agents/
│   │   └── dpi-stock-watch-agent.md    # Agent documentation
│   └── posts/
│       └── YYYY-MM-DD-dpi-watch.md     # Daily summaries
├── scripts/
│   ├── fetch-dpi-data.py               # Data fetching
│   ├── generate-hugo-post.py           # Post generation
│   └── send-dpi-alert.py               # Telegram alerts
├── agents.json                          # Agent registry
└── README.md                            # This file
```

---

## ⏰ Daily Timeline

| Time | Event | Agent |
|------|-------|-------|
| **8:15 AM** | **DPI Watch Stock Summary** | **DPI Watch** ⭐ |
| 8:45 AM | Pre-market opens | NSE/BSE |
| 9:15 AM | Market opens | NSE/BSE |

**Runs alongside CashlessWatch Stock at 8:15 AM** — complementary coverage:
- **CashlessWatch**: Payments & fintech
- **DPIWatch**: Infrastructure & GovTech

---

## 📊 Data Sources

| Tier | Source | Data |
|------|--------|------|
| 1 | NSE India | Nifty IT, Nifty 50, stock quotes |
| 2 | Yahoo Finance | All stocks, global benchmark |
| 3 | Moneycontrol | Verification, HTML scraping |

---

## 🤖 Agent

- **Schedule**: 8:15 AM IST, market days
- **Model**: minimax-m2.5
- **Delivery**: Telegram + Hugo
- **Agent Doc**: `content/agents/dpi-stock-watch-agent.md`

---

## ⚠️ Disclaimer

**Not investment advice. For informational purposes only.**

All data is timestamped at 08:15 AM IST, before the 08:45 AM pre-market open.

---

*DPI Watch — Tracking India's digital infrastructure plays.*
*Part of the CashlessConsumer project.*
