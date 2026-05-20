# Usage Guide

**How to use this kit based on your situation — start here.**

---

## Step 1 — Identify Your Situation

Answer these three questions:

**Q1: What kind of business do you run?**
- D2C / e-commerce → go to the D2C track below
- Labour supply / staffing / manpower → go to the Labour track below
- AI SaaS / tech product → go to the AI SaaS track below
- Other (retail, services, B2B) → use the Generic track below

**Q2: How do you currently collect data?**
- Online only (website, app, WhatsApp) → use digital consent notice templates
- Offline only (paper forms, in-person) → use `02-consent-notice-templates/consent-notice-offline-paper.md`
- Both → use both

**Q3: Do you share data with vendors or third parties?**
- Yes → you also need `04-consent-withdrawal/withdrawal-vendor-notification.md` and the [DPDP Vendor Compliance Kit](https://github.com/specuslabs/dpdp-vendor-compliance-kit)
- No → skip the vendor notification file

---

## The D2C / E-Commerce Track

You run an online store — Shopify, WooCommerce, a custom site, or an app.

**Problem:** Your existing cookie banner or consent popup was probably built for GDPR (European law). DPDP has different requirements. Notably, DPDP does not allow bundled or pre-ticked consent.

**Files to use, in order:**

1. `01-dpdp-reference/section-6-consent-requirements.md` — understand what valid consent means under DPDP
2. `02-consent-notice-templates/consent-notice-d2c-ecommerce.md` — your consent notice at checkout and account creation
3. `03-privacy-policy-templates/privacy-policy-d2c-ecommerce.md` — your full privacy policy
4. `04-consent-withdrawal/withdrawal-process-guide.md` — how to handle deletion and withdrawal requests
5. `04-consent-withdrawal/withdrawal-request-form.md` — the form you give customers to submit requests
6. `04-consent-withdrawal/withdrawal-response-templates.md` — your email/WhatsApp response templates
7. `05-sector-guides/d2c-ecommerce-guide.md` — consolidated implementation checklist

**Common D2C data points to cover in your notice:**
- Name, phone, email (at checkout)
- Delivery address
- Payment data (note: if processed by Razorpay, PayU, etc., their consent applies — you must say this)
- Purchase history and browsing data (if used for marketing)
- WhatsApp opt-in (separate consent required)

---

## The Labour / Staffing Track

You supply workers to client companies or manage a large field workforce. You collect Aadhaar, PAN, bank details, photos, and sometimes biometrics.

**Problem:** Paper application forms with no consent notice are a significant compliance risk. Workers often do not know what data you hold, who you share it with, or how to ask for deletion. Sensitive data (Aadhaar, biometrics) has stricter requirements.

**Files to use, in order:**

1. `01-dpdp-reference/section-5-notice-requirements.md` — what your notice must contain
2. `01-dpdp-reference/section-6-consent-requirements.md` — how to obtain valid consent
3. `02-consent-notice-templates/consent-notice-labour-staffing.md` — consent notice for worker onboarding
4. `02-consent-notice-templates/consent-notice-offline-paper.md` — how to add consent to your existing paper forms
5. `03-privacy-policy-templates/privacy-policy-labour-staffing.md` — your full privacy policy
6. `04-consent-withdrawal/withdrawal-process-guide.md` — how to handle withdrawal from workers
7. `04-consent-withdrawal/withdrawal-vendor-notification.md` — notify client companies when a worker withdraws consent
8. `05-sector-guides/labour-staffing-guide.md` — consolidated implementation checklist

**Key issue for this sector:** You share worker data with client companies. When a worker withdraws consent, you must notify every client who has their data. See the vendor notification file.

---

## The AI SaaS Track

You run a software product that uses AI, processes user data, or involves third-party AI APIs (OpenAI, Anthropic, Google, etc.).

**Problem:** AI products often process data in ways users don't expect — model training, inference logs, third-party API calls. DPDP requires you to disclose all of this in plain language.

**Files to use, in order:**

1. `01-dpdp-reference/consent-sections-explained.md` — full overview first
2. `02-consent-notice-templates/consent-notice-ai-saas.md` — consent notice at signup and for specific data uses
3. `03-privacy-policy-templates/privacy-policy-ai-saas.md` — your full privacy policy with AI-specific disclosures
4. `04-consent-withdrawal/withdrawal-process-guide.md` — how to handle deletion, especially from AI model logs
5. `04-consent-withdrawal/withdrawal-vendor-notification.md` — notifying your AI API vendors
6. `05-sector-guides/ai-saas-guide.md` — consolidated implementation checklist

---

## The Generic Track

You run a business that doesn't fit neatly into the above categories — a retail store, a services firm, a B2B company, a professional practice.

**Files to use:**

1. `01-dpdp-reference/consent-sections-explained.md` — full overview
2. `02-consent-notice-templates/consent-notice-generic.md` — adapt this for your context
3. `03-privacy-policy-templates/privacy-policy-generic.md` — adapt this for your context
4. `04-consent-withdrawal/withdrawal-process-guide.md` — set up your withdrawal process
5. `04-consent-withdrawal/withdrawal-request-form.md` — give this to users who want to withdraw

---

## Customising Templates

Every template in this kit uses `[SQUARE BRACKET PLACEHOLDERS]` for fields you need to fill in. Common ones:

| Placeholder | What to fill in |
|-------------|----------------|
| `[COMPANY NAME]` | Your registered business name |
| `[WEBSITE URL]` | Your website |
| `[GRIEVANCE OFFICER NAME]` | The person handling data complaints (required by DPDP) |
| `[GRIEVANCE OFFICER EMAIL]` | Their email address |
| `[DATA CATEGORIES]` | The specific types of data you collect |
| `[PURPOSE]` | Why you collect this data |
| `[RETENTION PERIOD]` | How long you keep data |
| `[VENDOR LIST]` | Third parties you share data with |
| `[EFFECTIVE DATE]` | When this policy goes live |

---

## Before You Go Live

- [ ] Have a qualified legal professional review your final notices and policies
- [ ] Ensure your grievance officer is a real, reachable person
- [ ] Test your withdrawal / deletion process end-to-end before publishing
- [ ] Document when you started using DPDP-compliant notices (keep a record)
- [ ] Set a calendar reminder to review when DPDP Rules are finalised by the Government

---

> **Disclaimer:** This kit is not legal advice. Review all materials with a qualified legal professional before use.
