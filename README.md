# SecureScorecard

> Instantly scan any business domain for security vulnerabilities. Get a professional PDF report with actionable remediation steps.

🔗 **Live at [securescorecard.io](https://securescorecard.io)**

---

## What It Does

SecureScorecard performs automated external security assessments on any domain. In under 10 seconds it checks 15+ security controls and generates a scored report with remediation guidance.

### Security Checks
- **Email Security** — SPF, DMARC, DKIM, MX Records
- **Web Security** — HTTPS, SSL Certificate, HSTS, Clickjacking Protection
- **HTTP Headers** — CSP, X-Content-Type, Referrer Policy, Permissions Policy
- **Reputation** — Blacklist Status, WHOIS Exposure, Subdomain Recon

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Next.js 15, TypeScript, Tailwind CSS |
| Backend | Next.js API Routes, Node.js |
| Database | Supabase (PostgreSQL) |
| Auth | Supabase Auth |
| Payments | Stripe |
| PDF Generation | jsPDF |
| Hosting | Vercel |

---

## Pricing Tiers

| Plan | Price | Features |
|------|-------|----------|
| Basic | Free | 15+ security checks, score & grade |
| Full Report | $49 one-time | Everything + PDF report |
| Pro | $99/mo | Unlimited scans, dashboard, CSV export |
| White Label | $199/mo | Custom branding, resell to clients |

---

## Features

- 15+ automated security checks
- Security score (0-100) with letter grade
- Professional PDF report generation
- WHOIS data via RDAP
- Passive subdomain reconnaissance
- Stripe payments (one-time + subscriptions)
- User dashboard with scan history
- Score trend charts
- CSV export
- Mobile responsive
- Row Level Security on all database tables

---

## Background

Built by [Garrett Fegley](https://linkedin.com/in/garrettfegley) — CompTIA Security+ certified, cybersecurity bootcamp graduate, and penetration tester. SecureScorecard was built to make professional security auditing accessible to small businesses who can't afford enterprise tools.

---

## Local Development

```bash
git clone https://github.com/GFSec-Cyber/securescorecard
cd securescorecard
npm install
```

Create `.env.local`:
```
NEXT_PUBLIC_SUPABASE_URL=your_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_key
SUPABASE_SERVICE_ROLE_KEY=your_service_key
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_key
STRIPE_SECRET_KEY=your_key
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

```bash
npm run dev
```
