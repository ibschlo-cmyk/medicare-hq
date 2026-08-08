# 2026 Claims Status & Billing Intake Quick Reference

**Status:** Public-safe operational summary derived from current-at-capture training material plus the existing exact-EOC claims/billing baseline.  
**Updated:** 2026-08-08

> This file intentionally omits internal system paths, scripts, queue information, proprietary routing details, and any member information. Internal claim-screen terminology must still be confirmed against the current production workflow before use as a universal rule.

## Fast bill intake

When a member says **"I got a bill"**, collect enough information to identify the correct provider account and claim before concluding liability:

- provider name;
- date of service;
- amount being billed;
- provider/account number when available; and
- billing-office contact information when provider outreach is required.

Then use the existing canonical sequence:

`Bill -> claim -> disposition -> member responsibility -> plan/QMB/network/auth context -> provider correction / reimbursement / appeal as applicable`

A bill by itself does **not** establish that the member owes the amount.

## Claim-identification minimums

Current-at-capture training material reinforces three high-value matching fields:

- **date of service**;
- **provider**; and
- **billed amount**.

These should be used to make sure the representative is discussing the correct claim before explaining payment or denial information.

## Claim-status vocabulary observed in the C-SNP workflow

The captured C-SNP training screen uses five practical status groups:

| Status group | Working meaning |
|---|---|
| **Approved / Final** | Claim reached an adjudicated end state; later adjustment may still be possible under the applicable workflow. |
| **Denied** | Claim was adjudicated but payment was denied because of an applicable benefit/policy determination. |
| **Pending / Needs Review / In Process** | Claim is not final and requires additional review before final adjudication. |
| **Needs Repair** | Claim information is incomplete or invalid and must be corrected before adjudication can complete. |
| **Rejected** | Claim failed minimum information/business-rule requirements and was not accepted for normal adjudication. |

These labels are **internal workflow terminology**, not universal Medicare regulatory definitions. Confirm the current production claim screen before relying on exact wording outside the captured C-SNP context.

## Red-team warning

Do **not** publish or teach a blanket rule that every HIDE/FIDE member is "covered at 100%" or can never receive any legitimate member responsibility. Instead verify:

- the exact plan/EOC;
- claim disposition;
- documented member responsibility;
- QMB status on the date of service when relevant;
- network and authorization context; and
- current controlled Aetna workflow.

## What remains internal / unresolved

- exact claim-search screen and search keys;
- where member responsibility appears;
- exact denial/reason-code interpretation;
- corrected-claim vs adjustment vs reprocessing procedure;
- escalation ownership and routing;
- whether the five captured C-SNP status labels map identically across the D-SNP claim systems.
