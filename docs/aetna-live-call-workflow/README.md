# Aetna Medicare Member Services — Live-Call Workflow Baseline

**Status:** Working, sanitized project baseline  
**Date:** 2026-08-08  
**Scope:** Aetna Medicare HIDE/FIDE D-SNP and C-SNP Member Services workflow support  

> This public repository copy intentionally excludes member information, credentials, internal-only screenshots, proprietary note-template content, and unverified internal routing details.

## Current plan anchors

| State | Plan type | Contract/PBP | Exact 2026 EOC / Member Handbook |
|---|---|---|---|
| Michigan | Aetna Medicare HIDE (HMO D-SNP) | `H9314-001` | `MI_DSNP_Handbook.pdf` — `H9314_001_NV15b_EOC2026_C` |
| Illinois | Aetna Medicare FIDE (HMO D-SNP) | `H9771-001` | `IL_DSNP_Handbook.pdf` — `H9771_001_NU11_EOC2026_C` |
| Virginia | Aetna Medicare FIDE (HMO D-SNP) | `H1610-001` | `H1610_001_DS17_EOC2026_C.pdf` |
| New Jersey | Aetna Medicare FIDE (HMO D-SNP) | `H6399-001` | `2026 Evidence of Coverage - English.pdf` — `H6399_001_DS70_EOC2026_C` |

Aetna C-SNP remains in operational scope; a specific 2026 C-SNP contract/PBP has not yet been added to this baseline.

## Exact Aetna EOC sources

- Michigan HIDE `H9314-001`: https://www.aetna.com/content/dam/aetna/medicaid/michigan-hide-dsnp/pdfs/2026/plan-documents/MI_DSNP_Handbook.pdf
- Illinois FIDE `H9771-001`: https://www.aetna.com/content/dam/aetna/medicaid/illinois-fide-dsnp/pdfs/2026/plan-documents/IL_DSNP_Handbook.pdf
- Virginia FIDE `H1610-001`: https://www.aetnabetterhealth.com/content/dam/aetna/medicaid/virginia-dsnp/pdf/H1610_001_DS17_EOC2026_C.pdf
- New Jersey FIDE `H6399-001`: https://www.aetnabetterhealth.com/content/dam/aetna/medicaid/new-jersey-hmosnp/pdf/2026%20Evidence%20of%20Coverage%20-%20English.pdf

These documents are the controlling public plan-level sources for the benefit facts summarized below. Current controlled Aetna internal procedures still govern exact system navigation, note-taking, transfers, and escalation steps.

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

### 2026 Extra Benefits Card matrix

| Plan | Base OTC Wallet | Qualifying chronic-condition effect |
|---|---:|---|
| Michigan `H9314-001` | **$220/month** | After qualification, the monthly amount becomes an **Extra Supports Wallet** with additional eligible categories |
| Illinois `H9771-001` | **$225/month** | After qualification, the monthly amount becomes an **Extra Supports Wallet** with additional eligible categories |
| Virginia `H1610-001` | **$280/month** | After qualification, the monthly amount becomes an **Extra Supports Wallet** with additional eligible categories |
| New Jersey `H6399-001` | **$255/month** | After qualification, the monthly amount becomes an **Extra Supports Wallet** with additional eligible categories |

Across these exact 2026 EOCs, qualifying Extra Supports Wallet categories include healthy foods, OTC items, transportation-related spending, utilities, and personal-care items/services subject to the plan's eligibility rules and detailed limitations. The EOCs direct members to `CVS.com/Aetna` or `1-844-428-8147` for approved Extra Benefits Card purchasing/order information.

**Operational rule:** do not quote one state's monthly amount or category rules on another state's call. Confirm the contract/PBP and current EOC first.

### Member received a bill

Working pattern:

`Identify bill source -> date/service -> locate corresponding claim -> read claim disposition -> determine documented member responsibility -> choose next action`

The four exact 2026 EOCs all provide strong protections against improper provider billing for covered services. Their detailed wording differs, but the common workflow principle is:

- A bill by itself is not proof that the member owes the amount.
- For covered in-network services, providers generally should bill the plan rather than the member.
- When a member receives a bill they do not understand or believe they do not owe, use the plan's Chapter 7 billing/payment workflow and current internal claims process rather than instructing the member to pay simply because a bill was issued.
- Reimbursement rules and exceptions depend on the exact service, provider status, coverage determination, and whether the member already paid.

### Claims

Working pattern:

`Find -> Read -> Determine -> Act`

The controlled internal workflow must supply the exact claim-screen steps, status terminology, denial/reprocessing procedures, and escalation path. The EOC supplies the member's plan-level coverage and billing rights; it does not replace the internal claims system.

### Appeals and grievances

Working pattern:

`Classify issue -> appeal or grievance -> standard/expedited if applicable -> correct routing -> document -> next level/escalation`

Each EOC contains the plan-specific coverage-decision, appeal, and grievance rules. Exact internal routing, queues, templates, and controlled procedures should be taken from the current Aetna workflow rather than reconstructed from an older training note.

### Vendor / scheduling assistance

Working pattern:

`Identify need -> verify benefit -> identify correct plan/state vendor -> conference/transfer/schedule as required -> confirm outcome -> document`

Priority categories include transportation, dental, vision, hearing, OTC/extra benefits, in-home support, and personal emergency response.

## Critical red-team finding: vendor routing is plan/state specific

A single vendor/contact strip is unsafe for this project. Exact 2026 EOCs already show material differences:

- **Illinois `H9771-001` transportation:** MTM Health, `1-855-814-1699`, Monday-Friday, 7 AM-8 PM local time, for rides to health-care visits and plan-approved locations.
- **New Jersey `H6399-001` non-emergency transportation:** Medicaid Fee-for-Service directly covers it; rides are arranged through **Modivcare**, `1-866-527-9933`.

Therefore, any trainer note containing a different transportation number must be treated as a lead to verify, not as a universal number for all FIDE/HIDE plans.

### Care Management

Working pattern:

`Identify coordination need -> locate assigned care-management resource -> route/escalate according to current internal guidance`

The EOCs repeatedly identify care coordinators/care managers as plan resources, but exact internal referral steps should come from controlled current guidance.

## EOC research workstream — current status

The dedicated internet-research workstream has now located the exact 2026 EOC / Member Handbook for all four current D-SNP plan anchors.

Research order remains:

1. Aetna-owned domains first (`aetna.com`, `aetnabetterhealth.com`)
2. Match exact contract/PBP, year, state, and plan type
3. Prefer the full **Evidence of Coverage / Member Handbook**
4. Capture Summary of Benefits, ANOC, Extra Benefits Card guide, OTC catalog, and formulary as supporting documents
5. Reject similarly named plans with a different PBP
6. Use CMS/state sources as secondary verification when needed

## Source hierarchy for this project

1. **Current controlled Aetna internal workflow** — controlling for exact navigation, notes, transfers, queues, and escalation
2. **Exact 2026 EOC / Member Handbook** — controlling public plan-level source for benefits, coverage, cost-sharing, member rights, billing, appeals, and plan-specific rules
3. **Current Aetna plan materials** — Summary of Benefits, ANOC, formularies, benefit guides, provider/member materials
4. **Trainer-provided material and handwritten notes** — operationally valuable but must be reconciled against current controlled sources and exact plan documents
5. **CMS/state authority** — regulatory validation and external context

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