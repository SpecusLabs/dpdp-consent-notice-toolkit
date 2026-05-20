# Section 6 — Consent Requirements

**A detailed plain English breakdown of what valid consent looks like under the DPDP Act, 2023 — and what doesn't count.**

> **Disclaimer:** This is not legal advice. Review with a qualified professional before use.

---

## What Section 6 Says

Section 6 of the DPDP Act defines what counts as valid consent. It then governs how consent must be managed after it is given — including the right to withdraw it.

The Act uses five specific words to describe valid consent. Every word matters.

---

## The Five Requirements of Valid Consent

### 1. Free
Consent is not valid if it is obtained under pressure, coercion, or as a non-negotiable condition.

**What this means in practice:**
- You cannot say "you must consent to marketing emails to use our platform" — unless the marketing emails are genuinely necessary to deliver the platform
- You cannot bundle multiple data uses into a single consent and require agreement to all of them
- You cannot make a service unavailable to someone who withdraws consent — unless the data is genuinely necessary for that service

**Common mistake:** Making the entire checkout process contingent on consent to a newsletter subscription. That is not free consent.

### 2. Specific
Each purpose of data use needs its own consent. You cannot get one blanket consent that covers everything.

**What this means in practice:**
- Order fulfilment → one consent
- Marketing SMS → separate consent
- WhatsApp promotional messages → separate consent
- Sharing data with a third-party analytics vendor → separate consent (or disclosure at minimum)
- Using data to train an AI model → separate, explicit consent

**Common mistake:** A single checkbox that says "I agree to the Terms and Privacy Policy." That is not specific consent.

### 3. Informed
The person giving consent must have actually read and understood the notice (Section 5). You cannot ask for consent before giving the notice.

**What this means in practice:**
- The notice must come before the consent action
- The consent action must reference the notice ("I have read and understood the data notice above")
- If your notice is buried or unclear, the consent obtained from it is not fully informed

### 4. Unconditional
Consent cannot be conditional on something else happening or not happening.

**What this means in practice:**
- No pre-conditions on the consent
- No "consent unless you opt out" (opt-out is not the same as consent under DPDP)
- No automatic renewal of consent without a fresh consent action

### 5. Unambiguous
There must be a clear, positive action from the user to indicate consent. Silence, inaction, or passive behaviour does not count.

**What this means in practice:**
- A pre-ticked checkbox does not count as consent — the user must tick it themselves
- "By using this website you agree to..." does not count as consent
- Scrolling past a notice does not count as consent
- The consent mechanism must be a deliberate, affirmative act: ticking a checkbox, clicking a clearly labelled button, signing a form

---

## The Consent Request

Section 6(1) specifies that the request for consent must be:
- In plain language
- Presented separately from any other information
- Not bundled inside terms and conditions
- Accompanied (or preceded) by the Section 5 notice

---

## Managing Consent After It Is Given

### The Consent Manager
The DPDP Act introduces the concept of a **Consent Manager** — a registered entity through which users can give, manage, and withdraw consent for multiple Data Fiduciaries. The Rules will define how this works. For now, you do not need to integrate with a Consent Manager, but your own withdrawal mechanism must work independently.

### Record Keeping
You must be able to prove that consent was given. Keep records of:
- When consent was given
- What version of the notice the user saw
- What they consented to
- The mechanism used (checkbox, signature, etc.)

This is especially important if you ever need to demonstrate compliance to the Data Protection Board.

---

## The Right to Withdraw Consent — Section 6(4) and 6(5)

This is one of the most operationally significant parts of the Act.

**Section 6(4):** A Data Principal (user) may withdraw their consent at any time.

**Section 6(5):** Upon withdrawal:
1. You must stop processing their personal data
2. You must cause your data processors (vendors) to stop processing it too
3. The consequences of withdrawal are to be borne by the Data Principal — meaning if they withdraw consent to data that is necessary for a service, they may lose access to that service. But you cannot penalise them beyond that.

**Critically:** Withdrawal must be as easy to do as giving consent. If consent took one click, withdrawal must also take one click (or close to it).

---

## What This Means Operationally

If you collect data from 10,000 customers and one of them sends you a withdrawal request:

1. You must stop using their data
2. You must delete it (subject to any legal retention requirements under Section 7)
3. You must notify every vendor you shared their data with
4. You must document that you did all of this

This is why the withdrawal process (see `04-consent-withdrawal/`) is as important as the consent collection process.

---

## Consent vs. Legitimate Use

Not everything requires consent. See `section-7-legitimate-use.md` for the specific situations where you can process data without consent (legal obligation, employment, state functions, etc.).

If you have a legitimate use basis, you do not need to go through the consent mechanism. But you should document your basis clearly.

---

## Checklist — Is Your Consent Mechanism Valid?

- [ ] The user sees the notice before the consent request
- [ ] The consent request is separate from terms and conditions
- [ ] Each purpose has its own consent (not one bundled checkbox)
- [ ] Checkboxes are unticked by default — user must actively tick them
- [ ] No "by using this site you agree to..." language
- [ ] Users can withdraw consent and the mechanism is as easy as giving consent
- [ ] You have a record of when consent was given and what version of the notice the user saw
- [ ] You have a process to stop using data when consent is withdrawn
- [ ] You have a process to notify vendors when consent is withdrawn

---

## Quick Reference — Valid vs. Invalid Consent

| Mechanism | Valid? | Why |
|-----------|--------|-----|
| Unticked checkbox user must tick | ✅ Yes | Unambiguous, affirmative action |
| Pre-ticked checkbox | ❌ No | Not unambiguous — user did not act |
| "By using this site you agree" | ❌ No | Not unambiguous, not specific |
| Signed paper form with notice attached | ✅ Yes | Affirmative, informed |
| Single checkbox for multiple purposes | ❌ No | Not specific |
| Separate checkboxes for each purpose | ✅ Yes | Specific and unambiguous |
| Opt-out mechanism (assumed consent) | ❌ No | Not unambiguous |
| WhatsApp "Reply YES to consent" | ✅ Yes (with caveats) | Affirmative — but keep the record |

---

*Template by Specus Labs · [specuslabs.com](https://specuslabs.com) · Free to use under CC BY 4.0*
