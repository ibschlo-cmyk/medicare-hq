# Benefits Information Script — 2026 Reconciliation

**Updated:** 2026-08-08  
**Source layer:** supplied Aetna COE Member Services training screenshots + current 2026 Aetna plan documents  
**Public-safe:** yes — proprietary scripting, authentication fields, internal URLs and screen-by-screen instructions intentionally omitted.

## Source status

The supplied internal source is titled approximately:

**Aetna Better Health Center of Excellence — COE Member Services — Call Script: Benefits Information**

Visible revision date: **02/23/2025**.

The source is useful as a call-structure reference, but its visible plan list and several operational examples are not a safe 2026 plan baseline. It includes legacy/MMP products and Ohio references that are outside the current four-plan D-SNP queue documented in this project.

Current plan anchors:

- Michigan HIDE `H9314-001`
- Illinois FIDE `H9771-001`
- Virginia FIDE `H1610-001`
- New Jersey FIDE `H6399-001`

## Keep — durable workflow behaviors

The following behaviors remain aligned with the 2026 workflow architecture:

1. **Use the most current plan-specific Member Handbook / EOC to quote benefits.**
2. **Tailor the benefit answer to the exact enrolled plan; do not quote one plan's benefit as another plan's.**
3. **Use current plan sources for covered-service limitations, restrictions and prior-authorization requirements.**
4. **Use the current internal PA lookup workflow for service-specific prior-authorization questions.**
5. **Care Manager / Service Coordinator involvement is appropriate when the benefit or service is care-management dependent.**
6. **Member Services should help the member navigate the plan handbook/website rather than rely on memory alone.**
7. **Close the call only after checking for remaining questions and completing the required Aetna call-tracking/documentation workflow.**

## Replace / red-team — dated or unsafe to generalize

### 1. Legacy plan scope

The 2025 script visibly includes older MMP/Ohio and legacy product references. Do not use that plan list as the 2026 routing map.

**2026 rule:** IVR / plan cue -> exact state + contract/PBP -> exact 2026 EOC -> plan-specific workflow.

### 2. Generic transition-of-care timeframes

The 2025 script contains generic 90-day / 365-day transition language for some out-of-network situations.

That is **not safe as a universal 2026 rule**. Exact 2026 plan documents materially differ:

- Michigan H9314-001 uses a transition/care-plan framework tied to new-enrollee continuity and care coordination.
- Illinois H9771-001 has plan-specific continuity periods, including different periods depending on prior D-SNP status and active treatment.
- Virginia H1610-001 includes a minimum 90-day new-enrollee transition protection for active courses of treatment.
- New Jersey H6399-001 has service/provider-specific continuity rules and timeframes.

**Desk-aid rule:** never quote a generic transition period without checking the exact plan/state source.

### 3. Urgent care network rule

The 2025 script frames urgent care primarily as PCP/in-network urgent-care use. Current 2026 Michigan plan material explicitly states urgently needed services do **not** require prior authorization and do **not** have to be in-network. Other plans have their own urgently-needed-care language and service-area rules.

**Desk-aid rule:** emergency/urgent care is a plan-document exception branch; do not use the old blanket "urgent care must be in-network" phrasing.

### 4. Out-of-network care

The 2025 script correctly treats routine out-of-network care as restricted, but some examples are state/product-specific and include obsolete Ohio language.

**2026 durable rule:** routine OON care usually requires exact-plan authorization/coverage confirmation; emergency, urgently needed care, dialysis while temporarily outside the service area, network-unavailable care, and continuity exceptions must be checked against the exact EOC.

### 5. Member Services hours and contact routing

The older script contains generalized D-SNP hours. The four current plans have plan-specific Member Services contacts. Do not hard-code one generic phone/time-zone line into the final desk aid.

## Public-source cross-checks used in reconciliation

- 2026 Michigan H9314-001 Summary of Benefits: urgent care is $0, does not require PA, and does not have to be in-network.
- 2026 Virginia H1610-001 EOC: new enrollees receive a minimum 90-day transition period for an active course of treatment, including treatment begun with an OON provider; routine OON care otherwise generally requires a covered exception/authorization.
- Aetna Medicare current provider-directory guidance: emergency/urgent care may be covered in or out of network, while routine OON care is plan-dependent and may require prior authorization/pre-service determination.

## Final 2026 benefit-call pattern

`Authenticate under current controlled workflow -> identify exact plan/state -> open exact 2026 EOC -> identify exact benefit/service -> verify coverage + limits + PA + network rule -> use current internal system if needed -> coordinate with CM/SC/vendor when the plan assigns that role -> explain next action -> required Aetna documentation`

## Still controlled / internal

Do not publish or infer:

- exact authentication fields;
- QNXT screen navigation;
- ProPAT click path;
- exact CM/SC instant-message / warm-transfer mechanics;
- call-tracking template fields;
- current internal call codes;
- exact escalation or transfer queues.

Those belong in the private second-brain layer and current controlled Aetna desktop.
