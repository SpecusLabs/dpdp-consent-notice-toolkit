# Section 5 — Notice Requirements

**A detailed plain English breakdown of what your consent notice must contain under the DPDP Act, 2023.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.

---

## What Section 5 Says

Section 5 of the Digital Personal Data Protection Act, 2023 requires every Data Fiduciary (that's you — any person or business that determines the purpose and means of processing personal data) to give a **notice** to the Data Principal (the person whose data you're collecting) at the time of, or before, seeking consent.

---

## What Your Notice Must Contain

The Act specifies that the notice must contain:

### 1. The Personal Data You Intend to Collect
Be specific. Don't say "we collect some information about you." Say exactly what you collect:
- Name, phone number, email address
- Delivery address
- Payment information (or note that payment is processed by a third party like Razorpay)
- Date of birth, gender
- Aadhaar number, PAN (only if genuinely required)
- Browsing behaviour, purchase history
- Location data

**Practical tip:** List your data fields in a table. It forces clarity and makes your notice easier to read.

### 2. The Purpose of Processing
For each category of data, explain *why* you need it. Vague purposes do not satisfy the Act.

**Not acceptable:** "To improve your experience"
**Acceptable:** "To send you order confirmation and delivery status updates via SMS and email"

**Not acceptable:** "For marketing purposes"
**Acceptable:** "To send you promotional offers about new products via WhatsApp — only if you opt in separately"

### 3. How to Exercise Rights
Your notice must tell users how they can:
- **Access** the data you hold about them
- **Correct** inaccurate data
- **Erase** their data (right to be forgotten)
- **Withdraw** their consent
- **File a grievance** with your Grievance Officer
- **Complain** to the Data Protection Board of India

This does not need to be fully detailed in the notice itself — you can link to your privacy policy for the full process. But the notice must acknowledge these rights exist and tell the user where to go.

### 4. How to Withdraw Consent
This must be explicit. The user must know:
- That they *can* withdraw consent at any time
- *How* to do it (email address, web form, WhatsApp number — be specific)
- What happens when they do (you will stop using their data and delete it)

### 5. Grievance Officer Contact
The Act requires every Data Fiduciary to appoint a Grievance Officer. Your notice must include:
- The Grievance Officer's name (or designation)
- How to reach them (email address is sufficient)

---

## Format Requirements

The Act specifies that the notice must be:

**In clear and plain language** — No legal jargon. Write as if explaining to a first-time customer.

**In English or a language in the 8th Schedule** — If a user requests the notice in a scheduled language (Hindi, Tamil, Bengali, Marathi, etc.), you must provide it. Build this into your process even if you start with English only.

**Separate from other documents** — A notice buried inside a 10-page terms and conditions document does not satisfy the Act. The consent notice should be a distinct, clearly labelled communication.

---

## What If You Collected Data Before the DPDP Act?

If you collected personal data before the Act came into force, you are still required to issue a notice "as soon as reasonably practicable." This means:

- You cannot simply ignore historical data collection
- You should send a retroactive notice to your existing customer/user/worker base
- Give them the opportunity to withdraw consent for any data use they did not previously know about

**Practical action:** Use the notice templates in `02-consent-notice-templates/` as the basis for a retroactive email or SMS notice to your existing database.

---

## Notice vs. Privacy Policy — What's the Difference?

Many businesses confuse a consent notice with a privacy policy. They are different things:

| Consent Notice | Privacy Policy |
|---------------|----------------|
| Given at the point of data collection | Published on your website |
| Short and specific | Long and comprehensive |
| Tied to a specific consent action | General statement of practices |
| Must be given every time you collect new data | Updated periodically |
| Required by Section 5 | Best practice and required by other laws |

You need both. Your consent notice is what the user sees before they click "I agree." Your privacy policy is the full document they can read for details.

---

## Checklist — Does Your Notice Cover Everything?

- [ ] Lists every category of personal data you collect
- [ ] States the specific purpose for each category
- [ ] Tells users they have the right to access, correct, and erase their data
- [ ] Tells users they can withdraw consent at any time
- [ ] Explains *how* to withdraw consent (specific channel)
- [ ] Names your Grievance Officer and gives their contact details
- [ ] Mentions the Data Protection Board of India as a complaints authority
- [ ] Written in plain language — no jargon
- [ ] Separate from your terms and conditions
- [ ] Available in English (and a scheduled language if requested)

---

## What This Looks Like in Practice

**For a D2C e-commerce business**, the notice appears at checkout — before the customer clicks "Place Order." It lists: name, address, phone, email, payment data (processed by Razorpay), purchase history. It states purposes: order fulfilment, delivery tracking, customer support. It links to the full privacy policy.

**For a labour/staffing company**, the notice is on page 1 of the worker application form (or a separate sheet attached to it). It lists: name, address, Aadhaar, PAN, bank details, photo, work history. It states purposes: employment placement, statutory compliance (PF, ESIC, TDS), payroll. It names the Grievance Officer.

**For an AI SaaS product**, the notice appears at signup. It lists: name, email, usage data, any data the user inputs into the product. It states purposes: product functionality, model improvement (if applicable — this must be explicit and separately consented to). It links to the privacy policy.

---

## Templates to Use

- `02-consent-notice-templates/consent-notice-generic.md` — starting point for any business
- `02-consent-notice-templates/consent-notice-d2c-ecommerce.md` — for online stores
- `02-consent-notice-templates/consent-notice-labour-staffing.md` — for labour/staffing companies
- `02-consent-notice-templates/consent-notice-ai-saas.md` — for SaaS and tech products
- `02-consent-notice-templates/consent-notice-offline-paper.md` — for paper form contexts

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
