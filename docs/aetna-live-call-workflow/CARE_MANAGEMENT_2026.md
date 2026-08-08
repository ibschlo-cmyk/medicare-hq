# 2026 Aetna SNP Care Management Workflow Baseline

**Status:** Current public-source operational baseline  
**Updated:** 2026-08-08  
**Scope:** Aetna HIDE/FIDE D-SNP and C-SNP Member Services workflow support

> Current controlled Aetna workflow remains the operational authority for finding the assigned Care Manager/Care Coordinator, warm transfers, referrals, queues, urgent escalation, and required note-template documentation.

## National Aetna SNP rule

Aetna's current Medicare care-management page states that members with an Aetna **C-SNP or D-SNP automatically get a care manager**. The care manager works with the member and providers to coordinate care, build a care plan, connect the member to community/support resources, and help prevent avoidable emergency-room visits or hospital stays.

This validates the substance of the trainer shorthand **"all members"** for the SNP call population. It does **not** mean every member receives the same intensity of care management, uses the same telephone number, or follows the same state workflow.

Public Aetna source: https://www.aetna.com/medicare/compare-plans-enroll/benefits-medicare-advantage-plan/managing-health.html

## Internal trainer cue

Trainer workflow note:

`Member CM Info Report -> Care Manager`

Working interpretation for the desk aid:

`Care/coordination need -> identify plan/state -> locate assigned CM/CC in current internal report -> connect/referral under current workflow -> confirm outcome -> required notes`

The exact report location, fields, permissions, and transfer/referral procedure are internal-workflow items and are intentionally not reconstructed from public sources.

## Plan-specific member routing

| Plan | Public care-management routing | Public-source operational finding |
|---|---|---|
| Michigan HIDE `H9314-001` | **1-855-676-5772 (TTY 711)** | Current HIDE materials route members through Member Services/Care Coordinator. Care management includes LTSS, waiver services, behavioral health, DME support, community transition and transportation coordination. |
| Illinois FIDE `H9771-001` | **1-866-600-2139 (TTY 711)** | All members are assigned a case manager; amount/frequency of case management varies by individual need. Current FIDE provider material also identifies **ILFIDECM@Aetna.com** for case-management referrals/escalated issues. |
| Virginia FIDE `H1610-001` | **1-855-463-0933 (TTY 711)** | Current Virginia FIDE page identifies care coordinators as nurses, social workers and licensed counselors who help with appointments, condition management, individualized care plans, agencies/resources and treatment-plan follow-through. |
| New Jersey FIDE `H6399-001` | **1-844-362-0934 (TTY 711)** | Current plan page says Care Managers are nurses/social workers who help connect members to care, teach about health and help with transportation; care-management help is available **8 AM-5 PM, 7 days/week**, while general Member Services is 8 AM-8 PM, 7 days/week. |

## Illinois case-management detail

Current Aetna Illinois FIDE provider materials say:

- **All members are assigned their own case manager.**
- The amount of care management depends on the member's individual needs.
- Case managers are typically nurses or social workers.
- They assess health/resources, develop a care plan with the member, coordinate with providers/caregivers and connect members with community resources.
- Referrals can be made at **1-866-600-2139** or **ILFIDECM@Aetna.com**.
- Current provider page says a case manager reviews/responds to a referral within **3-5 business days**.

This is a strong example of why "all members" must not be read as "all members get the same amount of contact."

## Health risk assessment / care-plan logic

Across integrated D-SNP materials, the health risk assessment/survey is a core input to the member's individualized care plan. The exact plan documents and current state materials use the assessment to identify needs, risks, goals and the appropriate level of care coordination.

High-speed workflow:

`New/changed needs -> check assigned CM/CC + HRA/care-plan status if relevant -> route to CM/CC -> document`

Do not create a new assessment or care plan from the desk aid; use the existing controlled system and assigned care-management team.

## When Care Management is a strong first route

The plan-specific sources support Care Management/Care Coordination for issues such as:

- complex or chronic-condition coordination;
- health-risk assessment and individualized care plan;
- post-hospital / transition-of-care needs;
- behavioral-health coordination;
- LTSS / MLTSS and waiver-service questions;
- transportation assistance when the member cannot navigate the plan/vendor route;
- community-resource needs;
- help coordinating multiple providers/services;
- certain plan-specific supplemental-benefit eligibility or setup, including Michigan's qualifying in-home support and PERS-related assistance where the EOC directs the member to Care Management.

## Michigan transportation relationship

For Michigan HIDE `H9314-001`, the safest public member-facing route is **Member Services/Care Coordinator at 1-855-676-5772**. Current HIDE provider-search material says members can call that number to set up a ride and should request the ride at least three business days in advance.

A separate current **Michigan Medicaid** page identifies MTM at `1-844-610-7437` and the same three-business-day rule. Another Michigan public page shows a different direct MTM number for the legacy/transition transportation context. Because those direct-vendor numbers do not align cleanly across product pages, the desk aid should route HIDE members through the HIDE Member Services/Care Coordinator workflow unless a current controlled Aetna procedure instructs otherwise.

## Trainer phone `844-596-6440`

The handwritten trainer note says:

`Care Management — 844-596-6440 — all members`

An exact-number public-source search did **not** produce an authoritative Aetna source tying `844-596-6440` to the current 2026 HIDE/FIDE/C-SNP care-management call population.

Therefore:

- **"all members" concept:** externally supported for Aetna C-SNP and D-SNP care management.
- **`844-596-6440`:** trainer-derived/internal only; do not publish as a universal care-management number.
- **Plan-specific public routing:** use the current plan numbers in the matrix above unless controlled internal guidance provides a dedicated internal line.

## High-speed desk-aid branch

**CARE / COORDINATION?**

`Plan/state -> assigned CM/CC (Member CM Info Report) -> identify need -> connect/refer via current plan workflow -> confirm action -> required notes`

**Use CM/CC especially for:** `HRA/care plan | LTSS/MLTSS | complex chronic needs | post-discharge | behavioral health coordination | transportation help | community resources | plan-specific support eligibility/setup`

## Still controlled/internal

- Exact `Member CM Info Report` navigation and fields
- Whether a specific call requires warm transfer, conference, task/message, referral or direct-number provision
- Urgent care-management escalation process
- Exact role of trainer line `844-596-6440`
- Care-manager assignment/status display
- Required note-template language
- Any state-specific internal queue or email not supported by a current controlled procedure
