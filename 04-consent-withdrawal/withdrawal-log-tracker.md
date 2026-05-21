# Withdrawal and Data Rights Log — Tracker Guide

**How to maintain a log of every data rights request you receive — for compliance, audit, and your own operational records.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.

---

## Why You Need This Log

The DPDP Act requires you to honour data rights requests. If the Data Protection Board ever investigates a complaint against your organisation, the first thing they will ask for is evidence that you received the request and what you did about it.

This log is that evidence. Keep it updated, keep it secure, and review it regularly.

**Use the `.csv` version** (`withdrawal-log-tracker.csv`) to actually track requests — it opens in Excel, Google Sheets, or LibreOffice. This markdown file explains what each column means and how to use it.

---

## Log Structure — Column Definitions

### Column 1: Reference Number
**Format:** `WDR-[YEAR]-[NUMBER]` — e.g., `WDR-2024-001`

Assign this when the request arrives. Use it in all correspondence with the person. Never reuse a reference number.

---

### Column 2: Date Received
**Format:** `DD-MM-YYYY`

The date you actually received the request — not the date you opened it or processed it.

---

### Column 3: Received Via
Options: `Email` / `Web Form` / `WhatsApp` / `In Person` / `Post` / `Phone`

How did the request come in? Important for audit purposes.

---

### Column 4: Requestor Name
Full name of the person making the request.

---

### Column 5: Requestor Email
Their email address — this is how you'll respond.

---

### Column 6: Requestor Phone
Their phone number if provided.

---

### Column 7: Requestor Type
Options: `Customer` / `Worker` / `Former Customer` / `Former Worker` / `Other`

---

### Column 8: Request Type
Options: `Access` / `Correction` / `Erasure` / `Grievance` / `Multiple`

If a single request covers more than one type (e.g., "I want my data deleted and I want to file a grievance"), mark as `Multiple` and note the types in the Details column.

---

### Column 9: Request Details (Summary)
A brief one-line summary of what they asked for. Keep it factual and neutral.

Example: `"Requested deletion of all personal data and withdrawal of marketing consent"`

---

### Column 10: Acknowledgement Sent Date
**Format:** `DD-MM-YYYY`

Date you sent the acknowledgement email. Should be within 48 hours of receiving the request.

---

### Column 11: Acknowledgement Sent By
Name of the staff member who sent the acknowledgement.

---

### Column 12: Identity Verified
Options: `Yes` / `No` / `Pending`

Have you confirmed that the person making the request is who they say they are? Do not process erasure or deletion without verification.

---

### Column 13: Verification Method
Options: `Email match` / `Aadhaar last 4` / `Phone match` / `ID document` / `In person`

---

### Column 14: Internal Systems Checked
List the internal systems you checked for the person's data.

Example: `CRM, email platform, order system, support tickets`

---

### Column 15: Data Found
Options: `Yes` / `No` / `Partial`

---

### Column 16: Data Deleted — Internal
**Format:** `DD-MM-YYYY` or `N/A`

Date you completed deletion from your own internal systems.

---

### Column 17: Data Retained (Legal Basis)
If any data was retained, list the category and legal basis.

Example: `Transaction records retained — GST Act 7yr requirement`

---

### Column 18: Vendors Notified
List of vendors notified and dates.

Example: `Delhivery (15-01-2024), Mailchimp (15-01-2024)`

Leave blank if no vendor held the person's data.

---

### Column 19: Vendor Deletion Confirmed
List vendors who confirmed deletion and the date.

Example: `Mailchimp confirmed 17-01-2024`

---

### Column 20: Completion Response Sent Date
**Format:** `DD-MM-YYYY`

Date you sent the final completion email to the requestor. Should be within 7 working days of receiving the request.

---

### Column 21: Completed Within 7 Days
Options: `Yes` / `No`

If `No`, note the reason in the Notes column.

---

### Column 22: Outcome
Options: `Completed` / `Rejected` / `Partial` / `Pending` / `Escalated`

- `Completed` — Request was fully processed
- `Rejected` — Request was rejected with a valid reason (e.g., could not verify identity)
- `Partial` — Some data retained under legal obligation; explained to requestor
- `Pending` — Still in progress
- `Escalated` — Requestor escalated to the Data Protection Board

---

### Column 23: Notes
Any additional information about this request — complications, delays, unusual circumstances, follow-up actions required.

---

## Operational Guidelines

**Who should maintain this log?**
One named person should own this log. Typically the Grievance Officer or Compliance Manager. Others can add entries but one person should review it weekly.

**Where should it be stored?**
- A password-protected folder or drive accessible only to relevant staff
- Not in a shared folder accessible to all employees
- Back it up regularly

**How long should you keep the log?**
Keep the log itself for at least 7 years. The log is your compliance evidence — treat it as you would a financial record.

**What if the requestor escalates to the Data Protection Board?**
Update the log with `Escalated` in the Outcome column. Keep all correspondence and records related to the request. You may be required to produce them.

---

## Monthly Review Checklist

At the end of each month, the log owner should confirm:

- [ ] All requests received this month have a reference number
- [ ] All acknowledgements were sent within 48 hours
- [ ] All completions were sent within 7 working days
- [ ] No requests are left in `Pending` status for more than 7 working days without a reason
- [ ] All vendors were notified for every erasure request
- [ ] The log is stored securely and backed up

---

## Sample Log Entry

| Field | Example |
|-------|---------|
| Reference Number | WDR-2024-001 |
| Date Received | 10-01-2024 |
| Received Via | Email |
| Requestor Name | Priya Sharma |
| Requestor Email | priya.sharma@email.com |
| Requestor Type | Customer |
| Request Type | Erasure |
| Summary | Requested deletion of all data and withdrawal of marketing consent |
| Acknowledgement Sent | 11-01-2024 |
| Identity Verified | Yes — email match |
| Systems Checked | CRM, Mailchimp, order system |
| Data Deleted | 16-01-2024 |
| Retained | Transaction records (orders #1042, #1087) — GST 7yr |
| Vendors Notified | Mailchimp 16-01-2024, Delhivery 16-01-2024 |
| Completion Sent | 16-01-2024 |
| Within 7 Days | Yes |
| Outcome | Partial (legal retention noted) |
| Notes | Customer acknowledged retention in reply. Case closed. |

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
*This is not legal advice. Review with a qualified professional before use.*
