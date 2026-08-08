# Aetna Medicare Member Services — Live-Call Workflow Baseline

**Status:** Working, sanitized project baseline  
**Date:** 2026-08-08  
**Scope:** Aetna Medicare HIDE/FIDE D-SNP and C-SNP Member Services workflow support  

> This public repository copy intentionally excludes member information, credentials, internal-only screenshots, proprietary note-template content, and unverified internal routing details.

## Current plan anchors

| State | Plan type | Contract/PBP |
|---|---|---|
| Michigan | Aetna Medicare HIDE (HMO D-SNP) | `H9314-001` |
| Illinois | Aetna Medicare FIDE (HMO D-SNP) | `H9771-001` |
| Virginia | Aetna Medicare FIDE (HMO D-SNP) | `H1610-001` |
| New Jersey | Aetna Medicare FIDE (HMO D-SNP) | `H6399-001` |

Aetna C-SNP remains in operational scope; a specific 2026 C-SNP contract/PBP has not yet been added to this baseline.

## Canonical call-start skeleton

1. **Incoming call**
2. **Listen to the IVR plan/state cue**
3. **Identify the exact plan context** — state, HIDE/FIDE/C-SNP, contract/PBP when available
4. **Pull the correct 2026 Evidence of Coverage (EOC) / Member Handbook**
5. **Use the employer-provided required note template** — do not substitute a homemade template
6. **Identify the member's call reason**
7. **Follow the issue-specific workflow**
8. **Resolve, conference, transfer, or escalate according to current controlled guidance**
9. **Complete required documentation**

## Priority call-reason branches

### Extra Benefits Card / food / OTC

Working pattern:

`Identify exact issue -> confirm plan -> open EOC/current benefit source -> verify eligibility/allowance/category -> resolve or vendor-route -> document`

Common issue classes include card declines, balance questions, eligible-item questions, replacement-card issues, food/OTC/utilities eligibility, and vendor/retailer problems.

### Member received a bill

Working pattern:

`Identify bill source -> date/service -> locate corresponding claim -> read claim disposition -> determine documented member responsibility -> choose next action`

A bill by itself is not proof that the member is responsible for the billed amount.

### Claims

Working pattern:

`Find -> Read -> Determine -> Act`

The controlled internal workflow must supply the exact claim-screen steps, status terminology, denial/reprocessing procedures, and escalation path.

### Appeals and grievances

Working pattern:

`Classify issue -> appeal or grievance -> standard/expedited if applicable -> correct routing -> document -> next level/escalation`

Exact routing and deadlines remain controlled-source dependent.

### Vendor / scheduling assistance

Working pattern:

`Identify need -> verify benefit -> identify correct vendor -> conference/transfer/schedule as required -> confirm outcome -> document`

Priority categories include transportation, dental, vision, hearing, OTC/extra benefits, in-home support, and personal emergency response.

### Care Management

Working pattern:

`Identify coordination need -> locate assigned care-management resource -> route/escalate according to current internal guidance`

## EOC research workstream

A dedicated internet-research function is responsible for finding the exact 2026 Aetna plan documents for every contract/PBP.

Research order:

1. Aetna-owned domains first (`aetna.com`, `aetnabetterhealth.com`)
2. Match exact contract/PBP, year, state, and plan type
3. Prefer the full **Evidence of Coverage / Member Handbook**
4. Capture Summary of Benefits, ANOC, Extra Benefits Card guide, OTC catalog, and formulary as supporting documents
5. Reject similarly named plans with a different PBP
6. Use CMS/state sources as secondary verification when needed

### Current public-source anchors

- Aetna's 2026 plan-document portal states that the **Evidence of Coverage** contains full plan coverage and rules and can be accessed without logging in by selecting plan details.
- `H9314-001` Michigan HIDE: official 2026 Aetna Summary of Benefits located.
- `H9771-001` Illinois FIDE: official 2026 Aetna Summary of Benefits and ANOC located.
- `H1610-001` Virginia FIDE: Aetna plan page and official 2026 Aetna Summary of Benefits located; the plan page exposes an Evidence of Coverage entry.
- `H6399-001` New Jersey FIDE: exact 2026 full EOC remains an active research target.

## Source-control rules

Every proposed desk-aid statement should be classified as one of:

- Current Aetna controlled source
- Trainer-provided instruction
- Internal workflow
- EOC / plan-specific
- Verified external authority
- Unresolved / needs confirmation

No unverified benefit amount, vendor rule, phone/fax number, appeal route, internal system step, or state-specific handling should be generalized across plans.

## Design target

The eventual desk aid should answer, in seconds:

> **What plan is this? Where do I look? What do I verify? What do I do next?**

Workflow accuracy and speed take priority over broad Medicare education.