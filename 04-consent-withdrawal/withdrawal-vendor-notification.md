# Withdrawal Vendor Notification Template

**When a person withdraws consent, you must notify every vendor who holds their data. Use these templates to do that.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.
> All fields in [SQUARE BRACKETS] must be filled in before use.

---

## Why Vendor Notification Is Required

Section 6(5) of the DPDP Act states:

> Upon withdrawal of consent, the Data Fiduciary and each of its Data Processors shall cease processing the personal data within a period and in a manner as may be prescribed.

"Data Processors" includes every vendor, partner, or third party you have shared the person's data with — your courier, email marketing platform, CRM provider, AI API, client company, payroll partner, background verification agency, and anyone else.

You cannot simply delete the data from your own systems and call the job done. You must notify the vendors and obtain confirmation that they have also deleted it.

**For labour and staffing companies:** This is especially important. When a worker withdraws consent, you must notify every **client company** who has received a copy of their profile. Those client companies must then delete the worker's data from their own systems.

This file connects to the [DPDP Vendor Compliance Kit](https://github.com/specuslabs/dpdp-vendor-compliance-kit) — if your vendors are not yet covered by a Data Processing Agreement (DPA) or vendor compliance checklist, do that work in parallel with your consent withdrawal process.

---

## Step 1 — Build Your Vendor List for This Individual

Before sending any notification, identify every vendor who holds this specific person's data.

Use this checklist:

**For D2C / E-commerce:**
- [ ] Courier / delivery partner (name, address, phone shared)
- [ ] Payment gateway (name, email, transaction records)
- [ ] Email marketing platform (name, email, subscription history)
- [ ] SMS platform (phone number)
- [ ] WhatsApp Business API provider (phone number)
- [ ] Analytics platform (if linked to individual — anonymise or delete)
- [ ] Customer support tool (name, email, chat history)
- [ ] Returns / exchange platform (if applicable)
- [ ] E-commerce platform (Shopify, WooCommerce — note their own retention policies)

**For Labour / Staffing:**
- [ ] Every client company where the worker was placed (name, photo, ID, work history)
- [ ] EPFO — for PF records (notify but data must be retained — inform the worker)
- [ ] ESIC — for ESI records (same as above)
- [ ] Payroll partner / bank (name, bank details, salary records)
- [ ] Background verification agency (name, ID documents, work history)
- [ ] Insurance provider (name, DOB, designation)
- [ ] Biometric attendance system provider (if applicable)

**For AI SaaS:**
- [ ] AI API provider (OpenAI, Anthropic, Google Vertex, etc.)
- [ ] Cloud hosting provider (AWS, GCP, Azure)
- [ ] Analytics platform (Mixpanel, Amplitude, etc.)
- [ ] Customer support tool
- [ ] Email provider

**Document this list.** Add it to the withdrawal log under "Vendors Notified."

---

## Step 2 — Send the Notification

Use the appropriate template below based on the type of vendor.

---

### Template A — Standard Vendor Notification (Email)

Use for: couriers, email platforms, SMS providers, analytics tools, support tools, AI API providers.

---

**Subject:** Data Deletion Request — [REQUESTOR NAME] — Ref: [REFERENCE NUMBER] — Action Required

---

Dear [VENDOR CONTACT NAME / Data Privacy Team],

We are writing to notify you of a data deletion and consent withdrawal request we have received from one of our customers / users / workers, whose personal data we have previously shared with you.

**Requestor details:**

| Field | Details |
|-------|---------|
| Full name | [REQUESTOR NAME] |
| Email address | [REQUESTOR EMAIL] |
| Phone number | [REQUESTOR PHONE — if shared] |
| Our reference number | [WDR-XXXX-XXX] |
| Date of withdrawal request | [DATE] |

**Data we shared with you:**

We previously shared the following data with your organisation:

- [LIST THE SPECIFIC DATA — e.g., Name, email address, phone number / Name, delivery address, phone for order #XXXX]

**Action required:**

Under the Digital Personal Data Protection Act, 2023 (India), we are required to notify you of this withdrawal and request that you:

1. **Delete all personal data** relating to [REQUESTOR NAME] from your systems within [7 working days]
2. **Confirm deletion** by replying to this email with the date and method of deletion
3. **Notify any sub-processors** you have shared this data with and ensure they also delete it

**Statutory retention:**

If your organisation is required to retain any of this data under Indian law (e.g., GST records, financial transaction records), please retain only what is legally required and confirm what you are retaining and on what legal basis.

**Response required by:** [DATE — 7 days from this email]

Please reply to this email with confirmation of deletion. If you have any questions, contact:

[YOUR NAME]
[YOUR DESIGNATION]
[YOUR EMAIL]
[YOUR PHONE]
[COMPANY NAME]

Thank you for your cooperation.

Regards,
[YOUR NAME]
[COMPANY NAME]

---

*This notification is issued under Section 6(5) of the Digital Personal Data Protection Act, 2023.*

---

### Template B — Client Company Notification (Labour / Staffing)

Use for: client companies where a worker was placed.

This is the most operationally sensitive notification. Client companies may resist deletion if the worker is currently on their site. Handle these with care.

---

**Subject:** Worker Data Deletion Request — [WORKER NAME] — Ref: [REFERENCE NUMBER] — DPDP Act Compliance Required

---

Dear [CLIENT COMPANY CONTACT NAME],

We are writing regarding a data deletion and consent withdrawal request we have received from [WORKER NAME], who [was placed at / is currently placed at] your facility.

**Worker details:**

| Field | Details |
|-------|---------|
| Full name | [WORKER NAME] |
| Worker ID (our ref) | [WORKER ID] |
| Placement period | [FROM DATE] to [TO DATE / Present] |
| Our reference number | [WDR-XXXX-XXX] |
| Date of withdrawal request | [DATE] |

**Data we shared with you:**

As part of the placement process, we shared the following worker data with your organisation:

- Name, photograph, and contact details
- Identity documents (Aadhaar number, PAN number)
- Work history, skills, and qualifications
- [Other data shared — e.g., medical fitness certificate / biometric template]

**Our obligations under the DPDP Act:**

The Digital Personal Data Protection Act, 2023 requires us to notify you of this withdrawal and request that you delete this worker's personal data from your records. This is our legal obligation under Section 6(5) of the Act.

**Action required from you:**

1. **Delete all copies** of the worker's personal data from your systems — including digital records, email attachments, physical files, and any access control or attendance systems
2. **Confirm deletion** by replying to this email
3. **Notify any sub-contractors or site managers** who have received a copy of this worker's data

**If the worker is currently on site:**

If [WORKER NAME] is currently placed at your facility, please note:

- You may retain the minimum data necessary for safety and on-site identity purposes until the placement ends
- Upon end of placement, all data must be deleted
- Please confirm the expected end date so we can set a deletion deadline

**Statutory retention:**

Data you are legally required to retain (e.g., wage records, ESI/PF compliance records) may be retained only for the legally required period. Please confirm what you are retaining and on what basis.

**Response required by:** [DATE — 7 working days from this email]

If you have any questions about your obligations under the DPDP Act, we recommend consulting the [DPDP Vendor Compliance Kit](https://github.com/specuslabs/dpdp-vendor-compliance-kit), which we use to manage vendor compliance.

Please reply to this email with:
1. Confirmation of deletion (or a deletion timeline if still in placement)
2. A list of any data retained and the legal basis

Contact us at:

[YOUR NAME]
[YOUR DESIGNATION]
[YOUR EMAIL]
[COMPANY NAME]

Regards,
[YOUR NAME]
[COMPANY NAME]

---

*This notification is issued under Section 6(5) of the Digital Personal Data Protection Act, 2023.*

---

### Template C — AI API Provider Notification

Use for: OpenAI, Anthropic, Google Vertex, or any AI API provider.

Note: Most AI providers do not offer individual data deletion for API-processed inputs once processed. Check the provider's privacy policy. Your notification is still required — and your completion response to the user should be transparent about the API provider's limitations.

---

**Subject:** Data Deletion Request — User Data Processed via API — Ref: [REFERENCE NUMBER]

---

Dear Data Privacy / Trust & Safety Team,

We are a business customer of [AI PROVIDER NAME] using your API ([API SERVICE NAME]) to power our product [PRODUCT NAME].

We have received a data deletion and consent withdrawal request from one of our users. Some of their personal data may have been processed through your API.

**Request details:**

| Field | Details |
|-------|---------|
| User identifier (as known to us) | [USER ID / EMAIL] |
| Approximate API call period | [DATE RANGE] |
| Our reference number | [WDR-XXXX-XXX] |
| Type of data processed | [e.g., User-submitted text documents / chat queries] |

**Action requested:**

Please confirm:

1. Whether data submitted via API calls from account [YOUR API ACCOUNT ID] during [DATE RANGE] was retained by your systems
2. If retained, whether you are able to delete it upon request
3. Your standard data retention period for API inputs
4. Whether you offer an individual deletion mechanism for API-processed data

We will communicate your response to the user as part of our withdrawal completion notice.

Please reply to: [YOUR PRIVACY / DATA EMAIL]

[YOUR NAME]
[COMPANY NAME]
[YOUR EMAIL]

---

*This notification is sent in connection with our obligations under the Digital Personal Data Protection Act, 2023 (India).*

---

## Step 3 — Log the Notifications

For each vendor you notify, record in the withdrawal log:

- Vendor name
- Date notification sent
- Method (email / letter / in-app form)
- Date confirmation received
- What they confirmed (deleted / retaining with legal basis / no data held)

---

## Step 4 — Handle Non-Responses

If a vendor does not respond within your deadline:

1. Send a follow-up email referencing your original notification
2. Note the non-response in the withdrawal log
3. Escalate internally — if a vendor persistently fails to comply, consider whether you should continue using them (vendor compliance is a separate issue covered in the [DPDP Vendor Compliance Kit](https://github.com/specuslabs/dpdp-vendor-compliance-kit))
4. Be transparent with the user in your completion response — if a vendor has not confirmed deletion, say so

---

## Cross-Repository Reference

This file is the connecting point between:

- **This repository** (dpdp-consent-notice-kit) — managing the consent and withdrawal lifecycle with your users
- **[DPDP Vendor Compliance Kit](https://github.com/specuslabs/dpdp-vendor-compliance-kit)** — managing your vendor relationships, Data Processing Agreements, and vendor audits

If you don't yet have DPAs in place with the vendors you're notifying, start there.

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
*This is not legal advice. Review with a qualified professional before use.*
