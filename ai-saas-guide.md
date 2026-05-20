# AI SaaS — DPDP Implementation Guide

**A consolidated implementation checklist and guide for AI-powered software products complying with the Digital Personal Data Protection Act, 2023.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.

---

## Who This Guide Is For

You build a software product that uses AI — whether that's an AI-native product (LLM-powered chat, document analysis, automation) or a traditional SaaS product with AI features (AI-generated insights, smart suggestions, predictive analytics). Your product processes user data through third-party AI APIs or your own models.

---

## Why AI Products Have Elevated DPDP Obligations

Standard SaaS products collect data and use it to run the service. AI products do something more complex: user inputs are sent to external AI systems, potentially retained by those systems, potentially used to train future models, and the outputs may be based on aggregated patterns from many users' data.

DPDP requires you to disclose all of this — specifically, clearly, and before users consent.

The specific obligations that affect AI products:

| Issue | Standard SaaS | AI SaaS |
|-------|--------------|---------|
| Third-party data sharing | Disclose vendors | Disclose AI providers + what is sent + training use |
| Data retention | State your own retention | State both your retention AND the AI provider's |
| Deletion on request | Delete from your systems | Attempt deletion + be transparent about API limitations |
| Consent for model training | N/A | Separate explicit consent required |
| Output disclaimer | N/A | Required — AI outputs may be inaccurate |
| Data sent to third parties | List vendors | List AI providers with specificity |

---

## Phase 1 — Foundation

### 1.1 Appoint a Grievance Officer

- [ ] Identify the person (typically a founder, CTO, or a designated privacy lead)
- [ ] Give them a dedicated email address — e.g., `privacy@[yourproduct].com`
- [ ] Publish their name and email in your privacy policy and consent notice

### 1.2 Audit Your AI Stack

Before writing any document, know exactly which AI providers you use and what user data each one receives.

Complete this audit:

| AI Provider | API/Service Used | User Data Sent | Training Opt-Out Enabled? | Log Retention (per their policy) |
|-------------|-----------------|---------------|--------------------------|----------------------------------|
| [e.g., OpenAI] | GPT-4o API | User text inputs | [Yes / No] | [e.g., 30 days] |
| [e.g., Anthropic] | Claude API | User text inputs | [Yes / No] | [e.g., Deleted immediately after response] |
| [e.g., Google Vertex] | Gemini API | [Data sent] | [Yes / No] | [Retention period] |
| [Other] | [Service] | [Data] | [Yes / No] | [Period] |

**Finding this information:**
- OpenAI: platform.openai.com/docs/models/data-usage — check your API data controls
- Anthropic: anthropic.com/privacy — enterprise customers can opt out of training use
- Google Cloud: cloud.google.com/terms/data-processing-terms

**Recommendation:** Enable training opt-out with every AI provider where it is available. This reduces your disclosure burden and is better for your users.

### 1.3 Map All Other Vendors

Beyond AI providers, map every vendor who receives user data:

- [ ] Cloud hosting (AWS, GCP, Azure, Railway, Vercel, etc.)
- [ ] Analytics (Mixpanel, Amplitude, PostHog, Google Analytics, etc.)
- [ ] Email provider (Postmark, SendGrid, Resend, etc.)
- [ ] Customer support (Intercom, Freshdesk, Zendesk, Crisp, etc.)
- [ ] Payment provider (Razorpay, Stripe India, etc.)
- [ ] Authentication provider (Auth0, Clerk, Supabase Auth, etc.)
- [ ] Database / storage (if using a managed service)
- [ ] Error monitoring (Sentry, Datadog, etc.)

This list forms your vendor disclosure table in your privacy policy and consent notice.

---

## Phase 2 — Consent Infrastructure

### 2.1 Consent at Signup

Every user must see a notice and give active consent before they create an account.

**What your signup consent must include:**
- That AI is used in the product and what user inputs are sent to which AI providers
- Whether user inputs are used for model training (by you or by the AI provider)
- A link to your full privacy policy
- An unchecked checkbox to confirm consent

**What it must NOT include:**
- Pre-ticked checkboxes
- "By signing up you agree to..." (not valid consent)
- Bundled consent for multiple purposes in one checkbox

**Template to use:** `02-consent-notice-templates/consent-notice-ai-saas.md`

**HTML version (embed):** `02-consent-notice-templates/consent-notice-ai-saas.html`

### 2.2 Contextual Consent for AI Features

If your product has distinct AI features (not just "AI powers the whole product"), consider giving a brief contextual notice the first time a user engages with each feature.

Example: If a user uploads a document for AI analysis for the first time, show: *"This document will be sent to [AI Provider] for analysis. [AI Provider] does not use this to train its models. [Link to full details in privacy policy]."*

This is above and beyond the minimum requirement — but it builds trust.

### 2.3 Separate Consent for Model Training

If you (not just the AI API provider) use user data to train or fine-tune your own models, this requires **separate, explicit consent**. It must be:

- A separate, clearly labelled checkbox — not bundled with the main product consent
- Optional — the user can refuse without losing access to the core product
- Easily withdrawable

If users have previously consented to training use and you later change your training approach, you need to re-collect consent for the new approach.

### 2.4 In-Product Consent Updates

If you add a new AI provider or a new data use after a user has signed up, you must obtain fresh consent for that new use before enabling it for that user.

Build a consent versioning system:
- Store the version of the privacy policy / consent notice each user consented to
- When you release a new version with material changes, prompt existing users to re-consent before accessing the product

---

## Phase 3 — Privacy Policy

- [ ] Use `03-privacy-policy-templates/privacy-policy-ai-saas.md` as your base
- [ ] Complete the AI provider table (Section 5 of the template) with real data from your Phase 1.2 audit
- [ ] Fill in every [SQUARE BRACKET] field
- [ ] Publish at a permanent URL — e.g., `yourproduct.com/privacy`
- [ ] Link to it from your signup consent notice, your product footer, and your settings page

**Review your privacy policy every time you:**
- Add a new AI provider or change your AI stack
- Add a new feature that processes a new type of user data
- The DPDP Rules are finalised (and update accordingly)

---

## Phase 4 — Withdrawal and Deletion Process

AI products have a specific deletion challenge: once user data has been processed by an AI API, it may not be deletable from that system. Your obligation is to:

1. Delete everything from your own systems (database, logs, backups)
2. Notify the AI provider and request deletion if their API supports it
3. Be transparent with the user about what you can and cannot delete from third-party AI systems

- [ ] Build an account deletion flow in your product (Settings → Delete Account)
- [ ] Define what deletion means for your product: which tables, logs, files, and backup systems
- [ ] Set up a deletion timeline and test it (target: all data deleted within 30 days of request)
- [ ] Prepare vendor notification templates for your AI providers: `04-consent-withdrawal/withdrawal-vendor-notification.md` (Template C — AI API Provider)
- [ ] Set up the withdrawal log: `04-consent-withdrawal/withdrawal-log-tracker.csv`
- [ ] Prepare response templates: `04-consent-withdrawal/withdrawal-response-templates.md`

**Language to use in your completion response when AI provider deletion is uncertain:**

> "We have deleted your data from our own systems. We have notified [AI Provider] and requested deletion from their systems. [AI Provider]'s data retention policy is [X days / per their API terms]. We cannot guarantee deletion from their systems beyond what their API permits, and recommend reviewing [AI Provider]'s privacy policy at [URL]."

This is transparent, honest, and demonstrates good faith.

---

## Phase 5 — AI Output Disclaimer

Add a disclaimer wherever AI-generated outputs appear in your product. This is both good product design and a compliance measure.

**Minimum language:**

> *AI-generated content may be inaccurate or incomplete. Do not rely on it for legal, medical, financial, or professional decisions without independent verification.*

Place this:
- In your privacy policy
- In your consent notice
- In the product UI near AI-generated outputs (tooltip, footer, or inline note)
- In your terms of service

---

## Phase 6 — B2B Considerations

If your AI SaaS product is sold to businesses (not individuals directly), your users' end-customers may also have data rights. Clarify this in your documentation:

- You are a **Data Processor** for your business customers (they are the Data Fiduciary for their end-users)
- Your business customers are responsible for obtaining consent from their own users before inputting that data into your product
- Your [Data Processing Agreement (DPA)](https://github.com/specuslabs/dpdp-vendor-compliance-kit) with each business customer should define how deletion requests from their end-users flow through to you
- When a business customer asks you to delete a specific end-user's data, you must be able to do so

---

## Compliance Checklist — Full Summary

### Foundation
- [ ] Grievance Officer appointed and published
- [ ] AI provider audit completed (what is sent, training opt-out status, log retention)
- [ ] All vendor data map completed

### Consent Infrastructure
- [ ] Signup consent notice in place with AI-specific disclosures
- [ ] Consent is active (unchecked checkbox), specific, and informed
- [ ] Separate consent for model training (if applicable)
- [ ] Consent versioning in place (store which version each user consented to)

### Privacy Policy
- [ ] AI-specific privacy policy published with AI provider table
- [ ] Linked from consent notice, product footer, and settings

### Withdrawal and Deletion
- [ ] In-product deletion flow built
- [ ] Deletion tested end-to-end
- [ ] Vendor notification process for AI providers prepared
- [ ] Withdrawal log set up
- [ ] Response templates ready

### AI Output Disclaimer
- [ ] Disclaimer in privacy policy
- [ ] Disclaimer in consent notice
- [ ] Disclaimer in product UI

### B2B (if applicable)
- [ ] DPA template prepared for business customers
- [ ] End-user deletion request flow defined

---

## Files to Use — Quick Reference

| Task | File |
|------|------|
| Consent notice (at signup) | `02-consent-notice-templates/consent-notice-ai-saas.md` |
| Consent notice HTML (embed) | `02-consent-notice-templates/consent-notice-ai-saas.html` |
| Privacy policy | `03-privacy-policy-templates/privacy-policy-ai-saas.md` |
| Withdrawal request form | `04-consent-withdrawal/withdrawal-request-form.html` |
| Withdrawal process guide | `04-consent-withdrawal/withdrawal-process-guide.md` |
| Withdrawal log | `04-consent-withdrawal/withdrawal-log-tracker.csv` |
| Response templates | `04-consent-withdrawal/withdrawal-response-templates.md` |
| AI provider notification | `04-consent-withdrawal/withdrawal-vendor-notification.md` |
| Section 6 — consent requirements | `01-dpdp-reference/section-6-consent-requirements.md` |

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
*This is not legal advice. Review with a qualified professional before use.*
