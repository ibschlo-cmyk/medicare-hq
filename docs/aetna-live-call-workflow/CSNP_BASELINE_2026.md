# 2026 Aetna C-SNP Baseline

**Status:** Current Aetna public-source baseline; exact contract/PBP still pending  
**Updated:** 2026-08-08

> This file is intentionally limited to Aetna's current national C-SNP eligibility/verification framework. Do not use it to quote plan-specific allowances, copays, networks, vendors, or service limits until the exact 2026 contract/PBP and EOC are known.

## Aetna C-SNP qualifying-condition set

Aetna's current 2026 C-SNP page says a member must have at least one of the following qualifying conditions, verified by a provider:

- Diabetes mellitus
- Chronic heart failure (CHF)
- Cardiac arrhythmias
- Coronary artery disease
- Peripheral vascular disease
- Valvular heart disease

Source: https://www.aetna.com/medicare/compare-plans-enroll/csnp-chronic-condition-special-needs-plans.html

## Verification requirement

Aetna's public C-SNP page says the treating PCP or specialist must confirm/attest to the qualifying condition. Aetna then sends a **Verification of Chronic Condition (VCC)** form to the provider.

The current Aetna VCC form states that, for the member to continue enrollment, the plan must verify with a health care provider that the member has one or more qualifying chronic conditions. Without provider verification, the member will be disenrolled within **60 days of enrollment**.

VCC form: https://www.aetna.com/content/dam/aetna/pdfs/aetnacom/healthcare-professionals/documents-forms/verification-of-chronic-condition-form.pdf

The public C-SNP page expresses the same operational deadline as verification being required **before the end of the second month** of enrollment.

## Current VCC condition structure

The VCC form groups the qualifying diagnoses as:

- Diabetes mellitus
- Chronic heart failure (CHF)
- Cardiovascular disorder, with the applicable subtype(s):
  - Cardiac arrhythmias
  - Coronary artery disease
  - Peripheral vascular disease
  - Valvular heart disease

The form also contains a provider option to indicate that the patient does not have any of the listed qualifying conditions.

## Operational call rule

For a C-SNP call, the plan-type label alone is not enough. The workflow should be:

`Identify exact C-SNP contract/PBP -> confirm qualifying-condition verification status when relevant -> open exact 2026 EOC -> handle benefit/claim/vendor issue using that plan's rules`

## Public Aetna C-SNP features that still require plan verification

Aetna's current public C-SNP materials describe features such as:

- a personal care team;
- an Extra Benefits / Extra Supports Wallet;
- certain $0 PCP and specialist visits;
- dental, vision, and hearing benefits;
- $0 Tier 1 chronic-condition drugs at in-network pharmacies;
- preferred diabetic supplies.

These are **not** safe as exact member-level promises without the member's contract/PBP and EOC. Aetna itself states that SSBCI eligibility standards and benefit conditions vary by benefit and plan.

## `Market Prominence -> C-SNP` trainer-note clarification

The phrase **MarketProminence** has a strong public match to **MHK MarketProminence®**, a Medicare Advantage / Part D administration platform. MHK publicly describes MarketProminence as supporting:

- enrollment and member maintenance;
- premium billing;
- financial reconciliation; and
- web-portal/workflow functions for Medicare Advantage and Part D plans.

Public MHK source: https://info.mhk.com/hubfs/web-documents/MHK-Product-Literature-Corporate-Overview-Brochure-230706.pdf

### What this does — and does not — establish

**Established externally:** `MarketProminence` is a Medicare plan administration/enrollment platform name, not a C-SNP category or geographic “market” term.

**Reasonable interpretation of the handwritten note:** `Market Prominence -> C-SNP` may be a reminder to use a MarketProminence system/workflow when handling C-SNP enrollment/member-maintenance information.

**Not established:** the public MHK material does not prove Aetna's specific internal implementation, screen path, permissions, or that this is the only C-SNP system used by the Member Services queue. The trainer note therefore remains **internal-workflow derived** until a current Aetna screen or controlled procedure confirms the exact usage.

This finding also means the phrase should **not** be used to infer the C-SNP's state, market, contract number, or PBP.

## Still unresolved

- Exact 2026 C-SNP contract/PBP handled by this Member Services queue
- Exact Aetna internal purpose/path for MarketProminence on C-SNP calls
- Exact state/market for the C-SNP call population
- Exact EOC/Member Handbook
- Exact Extra Benefits Card amount/categories
- Plan-specific vision/hearing/dental vendors and limits
- Plan-specific claims, appeals/grievances, transportation, PA, and care-management routing

## Next capture needed

The highest-value next item is a non-PII screen/photo showing the **C-SNP contract/PBP** and state/market. A second high-value capture is the screen that shows where **MarketProminence** appears in the actual C-SNP workflow. Once the contract/PBP is known, this generic baseline should be replaced by the exact plan EOC branch just as with `H9314-001`, `H9771-001`, `H1610-001`, and `H6399-001`.
