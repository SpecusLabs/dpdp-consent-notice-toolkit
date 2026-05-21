# D2C / E-Commerce — DPDP Implementation Guide

**A consolidated implementation checklist and guide for online stores complying with the Digital Personal Data Protection Act, 2023.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.

---

## Who This Guide Is For

You run an online store — Shopify, WooCommerce, a custom-built storefront, or a mobile commerce app. You sell to customers across India. You collect names, addresses, emails, phone numbers, and payment information at checkout.

This guide walks you through everything you need to do to be DPDP-compliant, in order of priority.

---

## The Core Problem: Your Existing Setup Is Probably GDPR-Compliant, Not DPDP-Compliant

Most Indian D2C stores built their consent and privacy infrastructure to satisfy one of three things:

1. **Shopify's built-in GDPR tools** — designed for European law
2. **A lawyer's boilerplate** — written for IT Act 2000, not DPDP 2023
3. **Nothing at all** — relying on "terms of use" acceptance to cover everything

None of these are DPDP-compliant. The key differences that affect you:

| Issue | Your Current Setup (Likely) | What DPDP Requires |
|-------|---------------------------|-------------------|
| Pre-ticked "subscribe" checkbox | Common | Not allowed |
| Consent bundled with T&Cs | Common | Not allowed |
| Single consent for all data uses | Common | Separate consent per purpose |
| No named Grievance Officer | Very common | Required |
| No withdrawal mechanism | Very common | Required — must be as easy as consent |
| Cookie consent (GDPR style) | Sometimes present | Rules not finalised under DPDP yet |
| No notice before consent | Very common | Required under Section 5 |

---

## Phase 1 — Foundation (Do This First)

### 1.1 Appoint a Grievance Officer

The DPDP Act requires you to name a real, reachable person as Grievance Officer. This is not optional.

- [ ] Identify the person (founder, COO, compliance person, or a designated staff member)
- [ ] Give them a dedicated email address — e.g., `privacy@[yourstore].com`
- [ ] Ensure they know how to handle a data rights request (use `04-consent-withdrawal/withdrawal-process-guide.md`)
- [ ] Publish their name and email on your website (in your privacy policy and consent notice)

### 1.2 Map Your Data

Before you write a notice or privacy policy, know exactly what data you collect.

Complete this data map for your store:

| Data | Where Collected | Stored In | Shared With |
|------|----------------|-----------|-------------|
| Name | Checkout | Shopify/WooCommerce | Courier partner |
| Email | Checkout + Newsletter | Shopify + Mailchimp | Mailchimp |
| Phone | Checkout | Shopify | Courier, SMS platform |
| Delivery address | Checkout | Shopify | Courier |
| Payment data | Checkout | Payment gateway (not you) | Payment gateway only |
| Purchase history | Automatic | Shopify | Analytics, possibly email platform |
| Browsing data | Automatic | Analytics platform | Analytics platform |
| WhatsApp number | Opt-in | WhatsApp platform | WhatsApp provider |

Fill this in for your actual tech stack before writing any documents.

### 1.3 Identify All Your Vendors

List every third party your store sends customer data to:

- [ ] Courier / delivery partner (Delhivery, Shiprocket, DTDC, Blue Dart, etc.)
- [ ] Payment gateway (Razorpay, PayU, Cashfree, CCAvenue, etc.)
- [ ] Email marketing (Mailchimp, Klaviyo, Brevo, etc.)
- [ ] SMS platform (MSG91, Kaleyra, Gupshup, etc.)
- [ ] WhatsApp Business API (Gupshup, Wati, Interakt, etc.)
- [ ] E-commerce platform (Shopify, WooCommerce)
- [ ] Analytics (Google Analytics, Meta Pixel, etc.)
- [ ] Returns platform (if applicable)
- [ ] Customer support (Freshdesk, Intercom, Zendesk, etc.)

This list will appear in your consent notice and privacy policy. It's also your vendor notification list when customers request deletion.

---

## Phase 2 — Consent Infrastructure

### 2.1 Replace Your Checkout Consent

Your current checkout consent is almost certainly non-compliant. Here's what to build:

**What the consent box must look like:**
- An unchecked checkbox — never pre-ticked
- Clear label: "I have read and agree to [STORE NAME]'s data collection notice, and consent to my data being used to process and deliver my order"
- The label must link to the full consent notice
- The consent notice must be visible before checkout completes

**Separate from the above, add optional consents (all unchecked by default):**
- [ ] "I consent to receiving promotional emails from [STORE NAME]"
- [ ] "I consent to receiving promotional SMS / WhatsApp messages from [STORE NAME]"

**Never bundle these.** Each purpose needs its own checkbox.

**Template to use:** `02-consent-notice-templates/consent-notice-d2c-ecommerce.md`

**HTML version (embed directly):** `02-consent-notice-templates/consent-notice-d2c-ecommerce.html`

### 2.2 Shopify-Specific Implementation

If you are on Shopify:

- [ ] Do not rely on Shopify's built-in GDPR cookie consent banner for DPDP compliance
- [ ] Add a custom consent section above the "Place Order" button in your checkout customisation (Shopify Plus allows full checkout customisation; on standard plans, use an app or the "Additional information" field)
- [ ] For marketing consent, add separate unchecked checkboxes — do not use Shopify's "customer accepts marketing" flag as a single bundled consent
- [ ] Use Shopify's Customer Privacy API or a third-party consent management app that can be configured for DPDP (most are GDPR-only by default — check with the vendor)

### 2.3 WooCommerce-Specific Implementation

If you are on WooCommerce:

- [ ] Use the WP Consent API plugin as a base
- [ ] Add separate checkboxes for order consent and marketing consent on the checkout page
- [ ] The "I agree to the terms and conditions" checkbox does not constitute valid DPDP consent for data collection — you need a separate, specific data consent checkbox
- [ ] Store consent timestamps in your database alongside each order

### 2.4 Account Creation Consent

If your store allows account creation:

- [ ] Add a consent notice and checkbox at the account creation screen (same structure as checkout)
- [ ] Do not allow account creation to proceed without ticking the required consent

### 2.5 Newsletter and WhatsApp Opt-In

If you collect emails or WhatsApp numbers separately (via a pop-up, landing page, or link-in-bio):

- [ ] Each collection point needs its own consent notice and unchecked checkbox
- [ ] The notice must state specifically what you will send and how to unsubscribe
- [ ] WhatsApp opt-in must reference WhatsApp explicitly — bundling it with email consent is not valid

---

## Phase 3 — Privacy Policy

Publish a DPDP-compliant privacy policy on your website.

- [ ] Use `03-privacy-policy-templates/privacy-policy-d2c-ecommerce.md` as your base
- [ ] Fill in every [SQUARE BRACKET] field
- [ ] Ensure the vendor list matches your actual tech stack (from Phase 1.3)
- [ ] Publish at a permanent URL (e.g., `yourstore.com/privacy-policy`)
- [ ] Link to it from your consent notice, your website footer, and your checkout

---

## Phase 4 — Withdrawal and Deletion Process

You must give customers a way to withdraw consent and request deletion that is as easy as giving consent.

- [ ] Set up a dedicated email address for withdrawal requests — e.g., `privacy@yourstore.com`
- [ ] Publish this email in your privacy policy and consent notice
- [ ] Optionally embed the withdrawal request form: `04-consent-withdrawal/withdrawal-request-form.html`
- [ ] Brief your Grievance Officer on the withdrawal process: `04-consent-withdrawal/withdrawal-process-guide.md`
- [ ] Set up the withdrawal log: `04-consent-withdrawal/withdrawal-log-tracker.csv`
- [ ] Prepare response email templates: `04-consent-withdrawal/withdrawal-response-templates.md`
- [ ] Prepare vendor notification templates: `04-consent-withdrawal/withdrawal-vendor-notification.md`

**Test your process:** Before going live, run a dummy withdrawal request end-to-end. Can you delete a customer's data from Shopify, Mailchimp, your courier partner's system, and your SMS platform within 7 working days? If not, fix the gaps now.

---

## Phase 5 — Retroactive Notice to Existing Customers

If you have an existing customer database, you should send a retroactive data notice to them.

- [ ] Draft an email explaining that you have updated your data practices to comply with the DPDP Act
- [ ] Include a link to your new privacy policy
- [ ] Remind customers of their right to withdraw consent and how to do it
- [ ] Give them the option to unsubscribe from marketing at the bottom of the email (standard unsubscribe link)

This retroactive notice is best practice and demonstrates good faith to the Data Protection Board.

---

## Compliance Checklist — Full Summary

### Foundation
- [ ] Grievance Officer appointed and published
- [ ] Data map completed
- [ ] Vendor list compiled

### Consent
- [ ] Checkout consent notice in place (unchecked checkbox, links to notice)
- [ ] Separate optional consents for email marketing and WhatsApp
- [ ] Account creation consent in place
- [ ] Newsletter / WhatsApp opt-in forms updated

### Privacy Policy
- [ ] DPDP-compliant privacy policy published at permanent URL
- [ ] Privacy policy linked from consent notice, footer, and checkout

### Withdrawal
- [ ] Withdrawal email address set up and published
- [ ] Withdrawal request form available
- [ ] Withdrawal process documented internally
- [ ] Withdrawal log tracker set up
- [ ] Response templates ready
- [ ] Vendor notification templates ready

### Verification
- [ ] Reviewed by a qualified legal professional
- [ ] Withdrawal process tested end-to-end
- [ ] Date of DPDP implementation recorded internally

---

## Files to Use — Quick Reference

| Task | File |
|------|------|
| Consent notice (checkout) | `02-consent-notice-templates/consent-notice-d2c-ecommerce.md` |
| Consent notice HTML (embed) | `02-consent-notice-templates/consent-notice-d2c-ecommerce.html` |
| Privacy policy | `03-privacy-policy-templates/privacy-policy-d2c-ecommerce.md` |
| Withdrawal request form | `04-consent-withdrawal/withdrawal-request-form.html` |
| Withdrawal process | `04-consent-withdrawal/withdrawal-process-guide.md` |
| Withdrawal log | `04-consent-withdrawal/withdrawal-log-tracker.csv` |
| Response templates | `04-consent-withdrawal/withdrawal-response-templates.md` |
| Vendor notification | `04-consent-withdrawal/withdrawal-vendor-notification.md` |

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
*This is not legal advice. Review with a qualified professional before use.*
