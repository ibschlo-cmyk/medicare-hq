# 2026 Aetna C-SNP Baseline

**Status:** Current 2026 plan anchor identified; exact Aetna-hosted EOC file URL still being retrieved  
**Updated:** 2026-08-08

> Do not use this file to quote plan-specific allowances, copays, networks, vendors, service limits, or internal routing unless the statement is tied to current Aetna material or the exact 2026 EOC/current controlled workflow.

## Current C-SNP plan anchor

The current working C-SNP for this Member Services project is:

- **Plan:** Aetna Medicare Prime Chronic Care (HMO C-SNP)
- **Contract/PBP:** `H1206-004`
- **State:** Illinois
- **Plan year:** 2026
- **Current Aetna plan page:** https://www.aetna.com/medicare/plan.H1206.004.html

Aetna's plan page was current for 2026 when reviewed and exposes entries for the plan's Annual Notice of Change, Summary of Benefits, Evidence of Coverage, and Drug List.

A 2026 Aetna-branded Summary of Benefits identifies:

- existing-member contact: **1-833-595-1008 (TTY 711)**;
- plan name: **Aetna Medicare Prime Chronic Care (HMO C-SNP)**; and
- chronic-condition focus including **cardiovascular disorders, chronic heart failure, and/or diabetes**.

The Summary directs readers to the Aetna H1206-004 plan page for the full Evidence of Coverage. The exact Aetna-hosted EOC PDF file URL remains a dedicated retrieval target.

## Why this is an upgrade

An internal mixed-age plan-code sheet first surfaced `H1206-004` as the Illinois C-SNP lead. Because that source contains both old and current material, the plan code was not promoted on internal evidence alone. Fresh 2026 Aetna public material now independently validates the contract/PBP and plan identity.

The old project status **“exact C-SNP contract/PBP pending”** is therefore retired.

## Aetna C-SNP qualifying-condition framework

Aetna's current C-SNP page says a member must have at least one qualifying chronic condition verified by a provider. Aetna's national condition framework includes:

- Diabetes mellitus
- Chronic heart failure (CHF)
- Cardiac arrhythmias
- Coronary artery disease
- Peripheral vascular disease
- Valvular heart disease

Source: https://www.aetna.com/medicare/compare-plans-enroll/csnp-chronic-condition-special-needs-plans.html

For `H1206-004`, use the exact plan's eligibility language once the EOC is retrieved; do not assume every national C-SNP condition necessarily maps identically to every PBP.

## Verification requirement

Aetna's public C-SNP page says the treating PCP or specialist must confirm/attest to the qualifying condition. Aetna then sends a **Verification of Chronic Condition (VCC)** form to the provider.

The current Aetna VCC form states that, for the member to continue enrollment, the plan must verify with a health care provider that the member has one or more qualifying chronic conditions. Without provider verification, the member will be disenrolled within **60 days of enrollment**.

VCC form: https://www.aetna.com/content/dam/aetna/pdfs/aetnacom/healthcare-professionals/documents-forms/verification-of-chronic-condition-form.pdf

The public C-SNP page expresses the same operational deadline as verification being required **before the end of the second month** of enrollment.

## Current VCC condition structure

The VCC form groups qualifying diagnoses as:

- Diabetes mellitus
- Chronic heart failure (CHF)
- Cardiovascular disorder, with the applicable subtype(s):
  - Cardiac arrhythmias
  - Coronary artery disease
  - Peripheral vascular disease
  - Valvular heart disease

The form also contains a provider option to indicate that the patient does not have any of the listed qualifying conditions.

## C-SNP live-call operating rule

`Identify H1206-004 -> confirm the issue -> if eligibility/continued enrollment is involved, check chronic-condition verification status in the current system -> open exact 2026 EOC/current plan material -> follow the C-SNP-specific call branch -> document using the required Aetna template`

A C-SNP label is not enough to quote an allowance, copay, vendor, or network rule.

## New controlled-workflow finding: disenrollment differs from QNXT D-SNP

A controlled internal source dated **2025-10-16** shows a material operational distinction:

- **C-SNP disenrollment requests use the C-SNP/GPS-controlled workflow.**
- They should not be processed through the same COE Member Services submission route used for QNXT D-SNP disenrollment.

The exact proprietary navigation is intentionally excluded from public GitHub; the important public-safe takeaway is that **C-SNP and QNXT D-SNP disenrollment are different workflows**.

## Public Aetna C-SNP features that still require exact-plan verification

Aetna's current public C-SNP materials describe features such as:

- a personal care team;
- an Extra Benefits / Extra Supports Wallet;
- certain $0 PCP and specialist visits;
- dental, vision, and hearing benefits;
- $0 Tier 1 chronic-condition drugs at in-network pharmacies; and
- preferred diabetic supplies.

These are **not** safe as exact member-level promises without the member's contract/PBP and EOC. Aetna itself states that SSBCI eligibility standards and benefit conditions vary by benefit and plan.

## `MarketProminence -> C-SNP` trainer-note clarification

The phrase **MarketProminence** has a strong public match to **MHK MarketProminence®**, a Medicare Advantage / Part D administration platform. MHK publicly describes MarketProminence as supporting enrollment/member maintenance, premium billing, financial reconciliation, and workflow functions.

Public MHK source: https://info.mhk.com/hubfs/web-documents/MHK-Product-Literature-Corporate-Overview-Brochure-230706.pdf

### What this does — and does not — establish

**Established externally:** `MarketProminence` is a Medicare plan administration/enrollment platform name, not a C-SNP category or geographic “market” term.

**Reasonable interpretation of the handwritten note:** `Market Prominence -> C-SNP` may be a reminder to use a MarketProminence system/workflow for C-SNP enrollment/member-maintenance information.

**Not established:** public MHK material does not prove Aetna's specific screen path, permissions, or whether this is the only C-SNP system used by the Member Services queue. Exact implementation remains a controlled-workflow question.

## Still unresolved

- Exact Aetna-hosted 2026 EOC PDF URL for `H1206-004`
- Exact internal MarketProminence/GPS navigation for C-SNP calls
- Exact Extra Benefits Card amount/categories from the controlling EOC
- Plan-specific vendor/routing details that have not yet been tied to current 2026 controlled or Aetna public material
- Exact claims, appeals/grievances, PA, Rx, and care-management system navigation

## Next research target

Retrieve and extract the exact 2026 Aetna Evidence of Coverage for `H1206-004`, then build the C-SNP branch at the same level of specificity as `H9314-001`, `H9771-001`, `H1610-001`, and `H6399-001`.
