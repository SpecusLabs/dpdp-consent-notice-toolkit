# Consent Withdrawal Process Guide

**A step-by-step operational guide for handling consent withdrawal and data deletion requests under the DPDP Act, 2023.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.

---

## Why This Matters

Section 6(4) of the DPDP Act gives every Data Principal (customer, worker, user) the right to withdraw their consent at any time.

Section 6(5) requires you to:
1. Stop using their personal data
2. Cause your data processors and vendors to stop using it
3. Honor the withdrawal as easily as consent was given

This is not a theoretical obligation. If a customer, worker, or user sends you a data deletion or withdrawal request, you have a defined set of steps to follow — and a defined timeframe to follow them in.

This guide walks you through the entire process.

---

## The Four Types of Requests You Will Receive

Under the DPDP Act, you may receive four types of requests from Data Principals:

| Request Type | What They Want | Your Obligation |
|-------------|---------------|----------------|
| **Access** | A copy of the data you hold about them | Provide a copy within [7 working days] |
| **Correction** | To fix inaccurate or outdated data | Correct and confirm within [7 working days] |
| **Erasure / Withdrawal** | For their data to be deleted and consent withdrawn | Delete all non-statutory data, notify vendors, log the action |
| **Grievance** | A complaint about how you handled their data | Acknowledge, investigate, and respond within [7 working days] |

This guide focuses primarily on **Erasure / Withdrawal** — the most operationally complex request.

---

## Step-by-Step Process — Erasure and Withdrawal

### Step 1 — Receive the Request

Requests may arrive by:
- Email to [WITHDRAWAL EMAIL]
- Submission of the withdrawal request form (see `withdrawal-request-form.md` or `.html`)
- WhatsApp message to your registered number
- In person at your office

**Assign a reference number** to every request the moment it arrives. This reference number ties together all records of this withdrawal.

Format: `WDR-[YEAR]-[SEQUENTIAL NUMBER]` — e.g., `WDR-2024-001`

**Log the request immediately** in the withdrawal log (see `withdrawal-log-tracker.md` or `.csv`).

---

### Step 2 — Acknowledge Within 48 Hours

Send an acknowledgement to the person within 48 hours of receiving the request. Include:
- The reference number
- Confirmation that you have received their request
- The timeframe within which you will respond
- Contact details if they have questions

Use the acknowledgement template in `withdrawal-response-templates.md`.

---

### Step 3 — Verify Identity

Before processing a deletion or withdrawal, verify that the request is from the actual Data Principal.

**For digital requests:** Match the email address or phone number to your records.

**For paper/in-person requests:** Ask for a copy of a government ID (Aadhaar card number, not a full copy).

**Do not make this process unreasonably difficult.** The Act requires withdrawal to be as easy as giving consent. A complex verification process that discourages withdrawal is not compliant.

---

### Step 4 — Identify All Data You Hold

Before you can delete anything, you need to know where the person's data lives. For a typical business, this means checking:

**Internal systems:**
- [ ] CRM or customer database
- [ ] Order management system
- [ ] HR / payroll system (if applicable)
- [ ] Email marketing platform
- [ ] Website analytics (anonymise or delete)
- [ ] Customer support tool (tickets, chat history)
- [ ] WhatsApp Business (if you have chat history)
- [ ] Paper files (if any — flag for physical destruction)
- [ ] [Any other internal system]

**External vendors:**
- [ ] Every vendor listed in your privacy policy / consent notice
- [ ] Every vendor you have shared this person's data with

Create a list of vendors to notify. Use `withdrawal-vendor-notification.md` to send each notification.

---

### Step 5 — Check for Legal Retention Requirements

Before deleting, identify any data you are **legally required to retain**. You cannot delete this data even on request.

| Data | Legal Retention Requirement |
|------|---------------------------|
| GST transaction records | 7 years (GST Act) |
| TDS and income tax records | 8 years (Income Tax Act) |
| PF and ESIC records | Duration required by EPFO/ESIC |
| Wage records | 3 years (Payment of Wages Act) |
| Employment records | 3-8 years depending on applicable labour law |
| Court order compliance data | As directed by the court |

**Anything not covered by a legal retention requirement must be deleted.**

Tell the person clearly what you are deleting and what you are retaining, and why.

---

### Step 6 — Delete All Non-Statutory Data

Execute the deletion across all systems identified in Step 4.

**Delete or anonymise:**
- Name, contact details, and profile data (from CRM, email platform, marketing lists)
- Browsing history and analytics data (anonymise — remove the link to the individual)
- Document uploads (from AI product or storage systems)
- Chat and support history
- Paper records (shred; log date of shredding)

**Retain with restricted access:**
- Transaction records (retain but flag as "deletion requested — retention required by law")
- Tax and statutory records

---

### Step 7 — Notify Vendors

For every vendor who holds the person's data, send a withdrawal notification within [TIMEFRAME — e.g., 72 hours of completing internal deletion].

Use the template in `withdrawal-vendor-notification.md`.

**Vendors must be notified, not just assumed to have deleted.** Keep a record of:
- Which vendors were notified
- When they were notified
- Their confirmation of deletion (if received)

---

### Step 8 — Respond to the Data Principal

Send a final response to the person confirming:
- What data has been deleted (list the categories)
- What data has been retained and why (legal requirement)
- Which vendors were notified
- That their consent has been formally withdrawn
- Their reference number, for their records

Use the completion template in `withdrawal-response-templates.md`.

**Timeframe:** Complete this step within [TIMEFRAME — e.g., 7 working days of receiving the request]. If complexity requires more time, communicate this in your acknowledgement.

---

### Step 9 — Update the Withdrawal Log

Update the withdrawal log with:
- Completion date
- What was deleted
- What was retained (and legal basis)
- Vendors notified (and dates)
- Any issues encountered

This log is your compliance record if the Data Protection Board ever investigates.

---

## Process for Access and Correction Requests

**Access request:**
1. Verify identity (Step 3 above)
2. Compile a summary of all data you hold about the person
3. Provide the summary in a readable format (PDF or table in email)
4. Do this within [7 working days]

**Correction request:**
1. Verify identity
2. Make the requested correction in all relevant systems
3. Notify any vendors who hold a copy of the incorrect data
4. Confirm the correction to the person
5. Do this within [7 working days]

---

## Process for Grievance Requests

1. Log the grievance in the withdrawal/grievance log
2. Send acknowledgement within 48 hours
3. Investigate: what happened? Was there a process failure?
4. Respond with your findings and any remedial action taken
5. If not resolved, inform the person they may escalate to the Data Protection Board of India
6. Complete within [7 working days for initial response / 30 days for resolution]

---

## Timeframe Summary

| Step | Deadline |
|------|---------|
| Acknowledge receipt | 48 hours |
| Complete internal deletion | [7 working days] |
| Notify all vendors | [72 hours after internal deletion] |
| Send final confirmation to person | [7 working days from request] |
| Close and log | Same day as final confirmation |

---

## What Happens to Active Orders / Engagements

If someone requests withdrawal while they have an active order or engagement:

- **For D2C:** If the order is in transit, you cannot delete the delivery address until delivery is complete. Inform the person of this. Delete immediately after delivery.
- **For labour/staffing:** If the worker is currently placed, you must inform the client company of the withdrawal but the worker's data may need to be retained until the placement ends and statutory records settled.
- **For SaaS:** If they have an active subscription, withdrawal may result in account closure. Inform them clearly.

---

## Related Files

- `withdrawal-request-form.md` / `.html` — The form you give to people who want to withdraw
- `withdrawal-response-templates.md` — Email templates for acknowledgement and completion
- `withdrawal-log-tracker.md` / `.csv` — The log to track every request
- `withdrawal-vendor-notification.md` — Template to notify vendors

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
*This is not legal advice. Review with a qualified professional before use.*
