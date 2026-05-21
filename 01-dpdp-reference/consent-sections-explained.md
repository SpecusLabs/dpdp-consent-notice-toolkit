# DPDP Act — Consent Sections Explained

**A plain English overview of Sections 5, 6, and 7 of the Digital Personal Data Protection Act, 2023.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.

---

## Why These Three Sections Matter

If your business collects any personal data from any person in India — a customer's phone number, a worker's Aadhaar, a user's email address — you are covered by the DPDP Act.

Sections 5, 6, and 7 are the three sections that govern how you collect that data. Together they answer:

- **Section 5:** What do you have to *tell* people before you collect their data?
- **Section 6:** What counts as valid *consent* — and what doesn't?
- **Section 7:** Are there situations where you don't need consent at all?

Understanding all three before you build your consent framework will save you significant rework.

---

## Section 5 — Notice

**The short version:** Before you collect someone's data, you must give them a notice that tells them exactly what you're collecting and why.

**What your notice must include:**
1. The personal data you intend to collect
2. The purpose for which you are collecting it
3. How they can exercise their rights (access, correction, erasure, grievance)
4. How they can withdraw their consent
5. How they can make a complaint to the Data Protection Board of India

**Key points:**
- The notice must be in clear and plain language
- It must be available in English and in any language specified under the 8th Schedule of the Constitution (if the user requests it)
- If you collected data before the DPDP Act came into force, you must still issue a notice as soon as reasonably practicable

**Common mistake:** Burying your notice inside a long terms and conditions document. The notice must be clear and accessible — not hidden.

See `section-5-notice-requirements.md` for a full breakdown.

---

## Section 6 — Consent

**The short version:** Consent must be free, specific, informed, unconditional, and unambiguous. Pre-ticked boxes do not count.

**What valid consent looks like:**
- The user actively does something (ticks a box, clicks a button, signs a form) to indicate agreement
- They do it after reading the notice in Section 5
- They are not forced or pressured into it
- The consent is specific to the purpose — you cannot get one consent for ten different uses
- There are no conditions attached — you cannot make a service contingent on consent to unrelated data collection

**The right to withdraw:**
- Users can withdraw consent at any time
- Withdrawal must be as easy as giving consent
- When someone withdraws, you must stop using their data — and notify any third parties (vendors) you've shared it with

**What does NOT count as consent:**
- Pre-ticked checkboxes
- "By using this website, you agree to..."
- Consent buried in terms and conditions
- Consent obtained under pressure or as a condition of service (unless the data is genuinely necessary for that service)

See `section-6-consent-requirements.md` for a full breakdown.

---

## Section 7 — Legitimate Use (No Consent Required)

**The short version:** There are specific situations where you can process personal data without consent. These are narrow exceptions, not loopholes.

**When you don't need consent:**
1. **State functions** — Government entities processing data for subsidies, services, licences, permits, or benefits
2. **Legal obligation** — You are required by Indian law to process this data (e.g., collecting PAN for tax compliance)
3. **Medical emergency** — To protect life in an emergency situation
4. **Public health** — During epidemics or health emergencies
5. **Employment** — Processing employee data for employment-related purposes (within reasonable limits)
6. **Judicial proceedings** — Processing required for court or tribunal orders
7. **Public interest functions** — Specific functions notified by the Central Government

**What this means for most businesses:**
- Collecting PAN or Aadhaar for statutory compliance (TDS, PF, ESIC) → Section 7 applies, consent not required
- Collecting a customer's name and address to deliver an order → Section 6 applies, consent required
- Processing employee salary data for payroll → Section 7 applies
- Sending marketing SMS to a customer → Section 6 applies, consent required

**Important:** Section 7 is not a blanket excuse. If you rely on it, you should document why you believe it applies to each specific data use. Do not use Section 7 to avoid building a proper consent framework.

See `section-7-legitimate-use.md` for a full breakdown.

---

## How the Three Sections Work Together

```
User arrives at your platform / fills your form
           │
           ▼
Is this a Section 7 legitimate use?
(Legal obligation, employment, state function, etc.)
           │
     Yes ──┼── No consent required. Document your basis.
           │
          No
           │
           ▼
Give the user a Section 5 Notice
(What data, what purpose, their rights, how to withdraw)
           │
           ▼
Obtain Section 6 Consent
(Active, specific, informed, unconditional)
           │
           ▼
Collect and use data only for the stated purpose
           │
           ▼
User withdraws consent?
           │
           ▼
Stop using data. Notify vendors. Log the withdrawal.
```

---

## Quick Reference — Your Obligations as a Data Fiduciary

| Obligation | Section | What It Means |
|-----------|---------|---------------|
| Issue a notice before collecting data | 5 | Tell users what you collect and why |
| Get valid consent | 6 | Active, specific, unconditional agreement |
| Allow withdrawal of consent | 6(4) | Must be as easy as giving consent |
| Stop processing on withdrawal | 6(5) | Cease use and notify vendors |
| Document your legal basis if not using consent | 7 | Record why Section 7 applies |
| Appoint a Grievance Officer | 13 | A real person users can contact |

---

## What Happens If You Don't Comply

The DPDP Act provides for financial penalties. While the Rules are still being finalised, the Act specifies penalties up to ₹250 crore for failure to implement reasonable data security measures, and up to ₹200 crore for failure to notify breaches. The Data Protection Board of India will have adjudication powers.

More importantly: non-compliance is a business risk. A customer or worker who cannot exercise their data rights can file a complaint with the Board.

---

## Further Reading

- Full text of the DPDP Act, 2023: [meity.gov.in](https://www.meity.gov.in)
- `section-5-notice-requirements.md` — detailed Section 5 breakdown
- `section-6-consent-requirements.md` — detailed Section 6 breakdown
- `section-7-legitimate-use.md` — detailed Section 7 breakdown

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
