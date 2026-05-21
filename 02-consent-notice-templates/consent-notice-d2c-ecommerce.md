# Consent Notice — D2C / E-Commerce

**For online stores using Shopify, WooCommerce, custom storefronts, or mobile apps.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.
> All fields in [SQUARE BRACKETS] must be filled in before use.

---

## Context: Why Your Current Consent Banner Probably Doesn't Work

If you are running a Shopify or WooCommerce store, your consent pop-up was almost certainly built for GDPR (European law). GDPR and DPDP are different:

| Issue | GDPR | DPDP |
|-------|------|------|
| Pre-ticked boxes | Not allowed | Not allowed |
| Consent bundled with terms | Sometimes acceptable | Not acceptable |
| Cookie consent | Required | Rules not yet finalised |
| Right to erasure | Yes | Yes |
| Consent for marketing | Separate required | Separate required |
| Language | EU languages | English + 8th Schedule languages |

Your existing banner likely does not:
- Give a clear notice before consent (Section 5)
- Separate consent by purpose (Section 6)
- Name a Grievance Officer as required by the DPDP Act
- Explain withdrawal in plain language

Use this template to build a DPDP-specific consent notice for your store.

---

## Where to Place This Notice

- **At checkout** — before the "Place Order" button, for order data
- **At account creation** — before the "Create Account" button
- **At newsletter signup** — before the "Subscribe" button (separate consent)
- **In your WhatsApp opt-in flow** — as a separate consent (do not bundle with checkout)

---

## Consent Notice — D2C / E-Commerce

---

**DATA COLLECTION NOTICE**
*Issued by [COMPANY NAME] | [WEBSITE URL] | Last updated [DATE]*

---

### What We Collect

When you place an order or create an account on our store, we collect:

| Data | Why We Collect It |
|------|------------------|
| Name | To address your order and communications |
| Email address | To send order confirmations, shipping updates, and receipts |
| Phone number | To contact you about delivery and order status |
| Delivery address | To ship your order to the correct location |
| Payment information | Processed securely by [PAYMENT GATEWAY — e.g., Razorpay / PayU / Stripe India] — we do not store your card or UPI details |
| Purchase history | To process returns, handle disputes, and improve our product recommendations |
| Device and browsing data | To show you relevant products and improve our website — see below |

**If you opt in to marketing communications (separate consent required):**
| Data | Why We Collect It |
|------|------------------|
| Email address | To send you promotional offers, new product announcements, and sale notifications |
| Phone number | To send you order-related SMS updates |
| WhatsApp number | To send you offers via WhatsApp — only if you opt in separately |

---

### Who We Share Your Data With

| Third Party | What We Share | Why |
|------------|--------------|-----|
| [COURIER PARTNER — e.g., Delhivery / Shiprocket / DTDC] | Name, phone, delivery address | To ship and deliver your order |
| [PAYMENT GATEWAY — e.g., Razorpay] | Name, email, order amount | To process your payment |
| [RETURN/EXCHANGE PLATFORM — if applicable] | Name, order details, phone | To process return and exchange requests |
| [ANALYTICS TOOL — e.g., Google Analytics] | Anonymised browsing data | To understand how people use our store |
| [EMAIL MARKETING TOOL — e.g., Mailchimp / Klaviyo — if applicable] | Name, email | To send marketing emails — only if you opt in |

We do not sell your personal data to any third party.

---

### How Long We Keep Your Data

| Data | Retention Period |
|------|----------------|
| Order and transaction data | 7 years (as required under GST and income tax law) |
| Account data | Until you delete your account or request erasure |
| Email marketing data | Until you unsubscribe or request erasure |
| Browsing and analytics data | [RETENTION PERIOD — e.g., 13 months] |

---

### Cookies and Tracking

Our website uses cookies and similar tracking technologies. These are used for:
- Keeping your cart intact while you browse
- Remembering your login (if you have an account)
- Understanding which products and pages are most popular
- [Showing you personalised recommendations — if applicable]

**Note:** Rules on cookies under the DPDP Act have not yet been finalised. We will update this notice when they are. In the meantime, we use cookies only for the purposes described above.

---

### Your Rights

Under the Digital Personal Data Protection Act, 2023, you have the right to:

- **Access** the data we hold about you — email us and we will provide a copy
- **Correct** any inaccurate data — update your account or contact us
- **Erase** your data — we will delete your account and personal data, subject to any legal retention requirements (e.g., we must keep GST transaction records for 7 years)
- **Withdraw** your consent at any time
- **File a grievance** with our Grievance Officer
- **Complain** to the Data Protection Board of India

---

### How to Withdraw Your Consent

To withdraw your consent or request erasure of your data:
- Email: [WITHDRAWAL/GRIEVANCE EMAIL]
- [Submit a request at: WITHDRAWAL FORM URL]

We will respond within [TIMEFRAME — e.g., 7 working days].

If you withdraw consent from data necessary to deliver your order (for example, your delivery address), we may not be able to fulfil that order.

---

### Grievance Officer

**Name:** [GRIEVANCE OFFICER NAME]
**Email:** [GRIEVANCE OFFICER EMAIL]
**Response time:** [TIMEFRAME — e.g., 7 working days]

---

### Your Consent

**For your order:**
☐ I have read this notice and consent to [COMPANY NAME] collecting and using my personal data to process and deliver my order as described above.

**For marketing communications (optional — do not pre-tick):**
☐ I consent to [COMPANY NAME] sending me promotional offers, new product updates, and sale announcements by email.

☐ I consent to [COMPANY NAME] sending me promotional messages via WhatsApp.

*You can withdraw any of these consents at any time by emailing [WITHDRAWAL EMAIL].*

---

*For our full Privacy Policy, visit: [PRIVACY POLICY URL]*

*This notice is issued under Section 5 of the Digital Personal Data Protection Act, 2023.*

---

## Implementation Notes for Shopify / WooCommerce

**Shopify:**
- Do not rely on the default Shopify GDPR cookie banner — it is not DPDP-compliant
- Add this notice above the "Place Order" button in your checkout template
- Use separate checkboxes (not pre-ticked) for each consent type
- If you use Shopify Email or Klaviyo for marketing, ensure marketing consent is a separate unchecked checkbox

**WooCommerce:**
- Use a plugin like WP Consent API or build a custom consent checkbox
- The WooCommerce "terms and conditions" checkbox does not constitute valid DPDP consent for data collection
- Build separate checkboxes for order consent and marketing consent

**Both platforms:**
- Log the timestamp and consent version when a user ticks a checkbox
- Store this consent log in your CRM or database
- When a user requests erasure, check your consent log, your order management system, your email platform, and all vendors listed in your notice

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
*This is not legal advice. Review with a qualified professional before use.*
