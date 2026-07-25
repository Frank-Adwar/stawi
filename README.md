# 🌱 Sitawi — Tax & Policy Navigator for Kenyans

**Sitawi** (Swahili for *"to thrive"*) is a mobile-first web application that helps everyday Kenyans — freelancers, gig workers, small business owners — understand and manage their tax obligations in plain, jargon-free language.

Built as a single-page HTML app with no server dependency, Sitawi works offline-ready in any modern browser.

---

## ✨ Features

### 📋 Personalized Onboarding
- Step-by-step profiling (income sources, income band, foreign currency, KRA PIN status, business registration)
- A rules engine derives which obligations apply to **you** specifically — no generic tax guides

### 🏠 Smart Home Dashboard
- **Estimated tax** for the year based on your profile
- **Next deadline** awareness with countdown
- **"Needs attention"** action items or a clean **"All caught up"** state
- **Finance Bill 2026 alerts** with severity levels (critical / warning / info) and English ↔ Swahili toggle

### 🔍 Explore
Visual category cards for:
- **Income Tax** — returns, what you owe, deadlines
- **Business** — Turnover Tax, eTIMS, deductions
- **Health** — SHIF (replaces NHIF), NSSF
- **Housing Levy** — rates, remittance, refund rules
- **Savings** — reliefs, deductible expenses, capital allowances

Each card opens a rich detail page with data tables, key figures, warnings, and citations to official KRA sources.

### 💬 Ask Sitawi (AI Chat)
- Conversational interface grounded in **official KRA guidance only**
- Every answer includes a source citation and verification date
- **Never bluffs** — escalates to a licensed tax agent when confidence is low
- Context-aware: if you've logged transactions, it answers with **your real numbers**
- Supports questions about expenses, deductions, income, eTIMS compliance, projections, and more

### 💰 Money (Financial Pipeline)
- **M-Pesa message parser** — paste an SMS and it auto-extracts amount, merchant, direction, date, and category
- **Manual entry** — add transactions with category, direction, amount, and date
- **Bank CSV import** — drag & drop your bank statement CSV
- **Auto-categorization** by merchant name (Shell → Fuel, Safaricom → Airtime, etc.)
- **Deductible tagging** — flags which expenses qualify as tax deductions and which need eTIMS invoices
- **Live dashboard** — income, expenses, deductible total, and estimated tax saved
- **Category breakdown** with visual bars
- **Export** to CSV or multi-sheet Excel (transactions, categories, tax summary)

### 👤 Profile
- View your onboarding answers and derived obligations
- Trust score badge
- Security & Data Protection detail page (7 principles including Kenya DPA 2019 compliance path)

### 🎨 Design
- Mobile-native UI with realistic iPhone frame (390 × 844)
- **Light & dark mode** — respects `prefers-color-scheme` or manual toggle
- Custom design tokens, smooth transitions, micro-animations
- Fully responsive — collapses to full-screen on small viewports
- Accessibility: `prefers-reduced-motion` support, focus-visible outlines, semantic HTML

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| **Structure** | Single HTML file, semantic HTML5 |
| **Styling** | Vanilla CSS with CSS custom properties (design tokens) |
| **Logic** | Vanilla JavaScript (no frameworks, no build step) |
| **Fonts** | [Inter](https://fonts.google.com/specimen/Inter), [Poppins](https://fonts.google.com/specimen/Poppins) via Google Fonts |
| **Storage** | `localStorage` for transaction persistence |
| **Icons** | Inline SVGs with reusable `<symbol>` definitions |

---

## 🚀 Getting Started

### Quick Start
Simply open the file in any modern browser:
```
open sitawi-app.html
```
No server, no npm install, no build step required.

### Other Files in this Repo

| File | Description |
|------|-------------|
| `sitawi-app.html` | Main application (full-featured) |
| `sitawi-mobile.html` | Mobile-optimized variant |
| `sitawi-mockup.html` | Design mockup / prototype |
| `sitawi-onboarding.html` | Standalone onboarding flow |
| `sitawi-lemonade.html` | Lemonade-style explore page |
| `huduma-alert.html` | Huduma alert system prototype |

---

## 📱 How It Works

```
┌──────────────┐     ┌─────────────┐     ┌──────────────┐
│  Onboarding  │ ──▶ │ Rules Engine │ ──▶ │  Personalized│
│  (5 questions)│     │ (in-browser) │     │  Dashboard   │
└──────────────┘     └─────────────┘     └──────────────┘
                                               │
                    ┌──────────────────────────┤
                    ▼                          ▼
             ┌────────────┐           ┌──────────────┐
             │ Ask Sitawi │           │   Money Tab  │
             │  (Chat AI) │ ◀──────▶ │  (M-Pesa,    │
             │            │  context  │  CSV, Manual)│
             └────────────┘           └──────────────┘
```

1. **Onboard** — Answer 5 questions about how you earn
2. **See your dashboard** — Obligations, deadlines, and alerts personalized to you
3. **Explore** — Tap any policy card to read plain-language breakdowns with official sources
4. **Log transactions** — Paste M-Pesa messages, upload bank CSVs, or enter manually
5. **Ask anything** — Chat with Sitawi for answers grounded in KRA guidance, using your real data

---

## 🔒 Security & Privacy

- **No backend required** — all data stays in your browser's `localStorage`
- **No personal data sent to AI** — the chat engine uses anonymized categories only
- **Kenya Data Protection Act 2019** compliance path documented
- **Encryption-ready architecture** — TLS for transit, column-level encryption at rest (when server is deployed)
- Full 7-point security framework detailed in-app under Profile → Security

---

## 🇰🇪 Kenyan Tax Context

Sitawi covers the following obligations as of **July 2026**:

- **Income Tax** — PAYE brackets, personal relief (KES 28,800/yr)
- **Turnover Tax** — 3% of gross for businesses under KES 25M
- **SHIF** — 2.75% (replaced NHIF)
- **NSSF Tier II** — up to KES 2,160/month
- **Housing Levy** — 1.5% of gross
- **eTIMS** — mandatory electronic invoicing for all deductions from Jan 2026
- **Finance Bill 2026** — alerts on proposed changes with severity ratings

---

## 📄 License

This project is proprietary. All rights reserved.

---

## 🤝 Contributing

This project is currently in active development. For inquiries, reach out via the [GitHub repository](https://github.com/Frank-Adwar/stawi).

---

<p align="center">
  <b>Sitawi</b> — Know what you owe. Keep what you've earned. 🌱
</p>
