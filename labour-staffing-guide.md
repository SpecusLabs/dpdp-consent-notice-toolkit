# Labour / Staffing / Manpower — DPDP Implementation Guide

**A consolidated implementation checklist and guide for labour supply, staffing, and facility management companies complying with the Digital Personal Data Protection Act, 2023.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.

---

## Who This Guide Is For

You supply workers to client companies. Or you run a manpower agency, facility management firm, or field workforce management operation. You collect Aadhaar, PAN, bank details, photographs, and work history from workers. You share this data with client companies and statutory bodies like EPFO and ESIC.

This sector has some of the highest DPDP compliance risk of any Indian industry — and some of the lowest current compliance rates.

---

## Why This Sector Is High Risk

| Risk Factor | Why It Matters |
|-------------|---------------|
| **Volume of sensitive data** | Aadhaar, PAN, bank details, biometrics — the most sensitive data categories under Indian law |
| **Paper-based collection** | No digital consent record, no version control, forms shared loosely |
| **Data shared with multiple client companies** | One worker's data may be copied to 5-10 client company HR departments |
| **Workers may not speak English** | Consent notices in English are meaningless to a worker who reads only Hindi or Marathi |
| **No deletion capability** | If a worker asks for deletion, most staffing companies cannot trace where the data has gone |
| **No Grievance Officer** | Workers have no named person to contact — and often don't know they have rights at all |

---

## Understanding Section 7 for This Sector

A large portion of the data you collect from workers falls under **Section 7(e) — Employment** of the DPDP Act. This means you do not need consent for:

- PAN number (TDS compliance — Income Tax Act)
- Aadhaar number (PF registration — EPFO)
- Bank account details (salary payment)
- ESI details (ESIC registration)
- Basic employment records (attendance, wage records)

**However:** Even when Section 7 applies and consent is not legally required, you should still issue a notice telling workers what you collect and why. This builds trust, reduces grievances, and protects you in any Board investigation.

Data collected on a **consent basis** (work history, skills profile, sharing with client companies) requires actual consent under Section 6.

See `01-dpdp-reference/section-7-legitimate-use.md` for the full breakdown.

---

## Phase 1 — Foundation

### 1.1 Appoint a Grievance Officer

- [ ] Identify the person (typically HR Head, Compliance Manager, or a designated senior)
- [ ] Give them a dedicated contact: email and a phone number (field workers need a number they can call)
- [ ] Ensure they speak the primary languages of your workforce — or have someone who does
- [ ] Train them on the withdrawal process (`04-consent-withdrawal/withdrawal-process-guide.md`)
- [ ] Publish their name, email, and phone on your website and on notice boards at your offices

### 1.2 Map Your Data — Workers

Complete a data map for every category of worker data you collect:

| Data | Collected On | Stored In | Shared With | Legal Basis |
|------|-------------|-----------|-------------|------------|
| Name, DOB, address | Paper registration form | HR database / paper file | Client company, EPFO, ESIC | Section 7(e) |
| Aadhaar number | Paper form + copy | HR database / file | EPFO, ESIC | Section 7(e) |
| PAN number | Paper form + copy | HR database | TDS filing | Section 7(e) |
| Bank account + IFSC | Paper form | Payroll system | Bank / payroll partner | Section 7(e) |
| Photograph | In-person or form | HR database | Client company, ID card | Section 7(e) |
| Work history | Paper form / interview | HR database | Client company | Section 6 — Consent |
| Skills and qualifications | Paper form | HR database | Client company | Section 6 — Consent |
| Biometrics (if any) | Biometric device | Attendance system | Client site system | Depends |

This map is the basis for your consent notice and privacy policy.

### 1.3 Map Your Client Companies

For every client company you have placed or currently place workers with:

- [ ] List the company name and your point of contact
- [ ] List what worker data you share with them (name, ID, photo, work history, etc.)
- [ ] Confirm whether they have a Data Processing Agreement (DPA) with you

If they do not have a DPA, this is a vendor compliance gap. Use the [DPDP Vendor Compliance Kit](https://github.com/specuslabs/dpdp-vendor-compliance-kit) to build one.

---

## Phase 2 — Consent Infrastructure

### 2.1 Revamp Your Worker Registration Form

Your current paper registration form collects data but almost certainly does not include a consent notice.

**What to do:**

Option A: Add the consent notice as a separate sheet — page 1 of every registration packet. The worker reads (or has read to them) the notice, then signs before filling in the form.

Option B: Redesign the form with the condensed consent notice built in at the top.

**Template to use:** `02-consent-notice-templates/consent-notice-labour-staffing.md`

**Printable HTML version:** `02-consent-notice-templates/consent-notice-labour-staffing.html`

**For walk-in / field registration:** `02-consent-notice-templates/consent-notice-offline-paper.html` — A4 print-ready.

### 2.2 Handle Workers Who Cannot Read

This is a real operational challenge. Many field workers may not be literate or may not read the language the form is written in.

- [ ] **Translate your consent notice** into the primary language(s) of your workforce (Hindi, Marathi, Tamil, Telugu, Bengali, Kannada — as applicable)
- [ ] **Train your field registration staff** to read the notice aloud and explain it before the worker signs
- [ ] **Add a "witnessed by" field** to your form — the staff member who explained the notice to the worker signs and dates it
- [ ] Consider a **verbal consent recording** on the worker's phone for any worker who cannot sign

### 2.3 Separate Consent for Skill Profile Sharing

When a worker gives you their work history and skills, you collect that data under consent (not statutory obligation). Your notice must explicitly say:

*"We will share your work history, skills, and qualifications with client companies for job placement purposes. You may withdraw this consent at any time by contacting [GRIEVANCE OFFICER]."*

The worker must tick or sign a specific consent for this — separate from the statutory data acknowledgement.

### 2.4 Digital Onboarding (if applicable)

If you use a digital onboarding app or WhatsApp flow:

- [ ] The consent notice must appear before any data entry begins
- [ ] A positive affirmative action is required (tap to confirm reading, tick a checkbox) — not just scrolling past
- [ ] Log the timestamp and the version of the notice shown

---

## Phase 3 — Privacy Policy

- [ ] Use `03-privacy-policy-templates/privacy-policy-labour-staffing.md` as your base
- [ ] Fill in every [SQUARE BRACKET] field
- [ ] Publish on your company website
- [ ] Print and post on notice boards at your offices and at worker collection / registration points
- [ ] Have it available in translated form at registration desks

---

## Phase 4 — Withdrawal and Deletion Process

This is the most operationally complex part of DPDP compliance for staffing companies.

When a worker withdraws consent:
1. You must delete their data from your systems
2. You must notify **every client company** who has a copy of their profile
3. You must notify EPFO, ESIC, payroll partners, BGV agencies, and any other vendor
4. You must retain statutory records (PF, ESIC, TDS, wage records) and explain this to the worker

- [ ] Set up a withdrawal channel: email address + phone number + in-person option
- [ ] Publish the withdrawal channel in your consent notice, privacy policy, and on notice boards
- [ ] Brief your Grievance Officer on the process: `04-consent-withdrawal/withdrawal-process-guide.md`
- [ ] Prepare your vendor notification templates: `04-consent-withdrawal/withdrawal-vendor-notification.md` (Template B — Client Company)
- [ ] Set up the withdrawal log: `04-consent-withdrawal/withdrawal-log-tracker.csv`
- [ ] Prepare response templates: `04-consent-withdrawal/withdrawal-response-templates.md`

**Key challenge:** Your client companies must delete worker data when notified. Most will not have a process for this. Start with your largest clients and work backwards. The [DPDP Vendor Compliance Kit](https://github.com/specuslabs/dpdp-vendor-compliance-kit) has DPA templates and vendor audit checklists for this.

---

## Phase 5 — Existing Worker Database

If you have a database of workers collected before DPDP compliance was in place:

- [ ] Send a retroactive notice to all workers (by SMS or WhatsApp to their registered numbers)
- [ ] Include: what data you hold, who you share it with, their rights, how to withdraw
- [ ] Give them 30 days to respond and withdraw if they wish
- [ ] Process any withdrawal requests received in that window
- [ ] Document that you sent the retroactive notice and when

Workers who do not respond may be treated as having continued consent — but document this clearly.

---

## Phase 6 — Staff Training

DPDP compliance for a staffing company is only as strong as the weakest link in your field registration chain.

- [ ] Train every staff member who collects worker data on the consent notice — they must be able to explain it verbally
- [ ] Train HR and compliance staff on how to handle withdrawal requests
- [ ] Conduct an annual refresher (set a calendar reminder)
- [ ] Designate a backup Grievance Officer in case the primary one is unavailable

---

## Compliance Checklist — Full Summary

### Foundation
- [ ] Grievance Officer appointed, published (website + notice boards), and reachable by phone
- [ ] Worker data map completed
- [ ] Client company list compiled with DPA status noted

### Consent Infrastructure
- [ ] Consent notice attached to worker registration form
- [ ] Notice translated into workforce languages
- [ ] Field staff trained to read and explain notice verbally
- [ ] "Witnessed by" field added to form
- [ ] Separate consent for work history and skills profile sharing

### Privacy Policy
- [ ] DPDP-compliant privacy policy published on website and posted at offices

### Withdrawal
- [ ] Withdrawal channel set up (email + phone + in-person)
- [ ] Withdrawal process documented and staff briefed
- [ ] Withdrawal log set up
- [ ] Response and vendor notification templates ready
- [ ] Client company notification process tested

### Existing Database
- [ ] Retroactive notice sent to existing workers
- [ ] Withdrawal requests from retroactive notice processed

### Training
- [ ] Field registration staff trained
- [ ] HR and compliance staff trained on withdrawal process

---

## Files to Use — Quick Reference

| Task | File |
|------|------|
| Consent notice (paper onboarding) | `02-consent-notice-templates/consent-notice-labour-staffing.md` |
| Consent notice (printable HTML) | `02-consent-notice-templates/consent-notice-labour-staffing.html` |
| Consent notice (offline A4 print) | `02-consent-notice-templates/consent-notice-offline-paper.html` |
| Privacy policy | `03-privacy-policy-templates/privacy-policy-labour-staffing.md` |
| Withdrawal request form | `04-consent-withdrawal/withdrawal-request-form.md` |
| Withdrawal process guide | `04-consent-withdrawal/withdrawal-process-guide.md` |
| Withdrawal log | `04-consent-withdrawal/withdrawal-log-tracker.csv` |
| Response templates | `04-consent-withdrawal/withdrawal-response-templates.md` |
| Vendor / client company notification | `04-consent-withdrawal/withdrawal-vendor-notification.md` |
| Section 7 reference (statutory data) | `01-dpdp-reference/section-7-legitimate-use.md` |

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
*This is not legal advice. Review with a qualified professional before use.*
