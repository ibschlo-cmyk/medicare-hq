# 2026 Aetna D-SNP Rx / Part D Workflow Baseline

**Status:** Exact-EOC public-source baseline  
**Updated:** 2026-08-08  
**Scope:** Michigan `H9314-001`, Illinois `H9771-001`, Virginia `H1610-001`, New Jersey `H6399-001`

> The trainer note `MedCompass -> RX` remains an internal workflow cue. This file supplies the plan-level Part D decision logic from the exact 2026 EOCs; it does not replace MedCompass, the formulary tool, pharmacy claim data, or current controlled Aetna routing.

## High-speed Rx branch

`RX issue -> identify exact drug + pharmacy message -> Part D vs Medicaid-only drug -> Drug List / restriction / PA / quantity / step therapy check -> current internal Rx system -> explain / coverage decision / reimbursement / appeal`

## Critical distinction: pharmacy rejection vs. formal coverage decision

A pharmacy saying that a prescription cannot be filled as written is not, by itself, the end of the coverage-decision process. The EOCs direct the member to the plan for a formal Part D coverage decision when coverage, formulary status, or a restriction is disputed.

A formal initial Part D decision is called a **coverage determination**.

Common reasons for a coverage determination include:

- drug is not on the Drug List;
- member wants an exception;
- plan restriction needs to be set aside;
- plan approval is required before coverage;
- member asks the plan to pay for a drug already purchased.

## Standard vs. fast Part D coverage decision

Across the exact EOC workflow, the core deadlines are:

- **Standard coverage decision:** generally within **72 hours** after the plan receives the prescriber's supporting statement when one is required.
- **Fast / expedited coverage decision:** generally within **24 hours** when the health-based expedited criteria are met.

A fast coverage decision is for a drug the member **has not already obtained**. If the issue is payment back for a drug already purchased, use the Chapter 7 reimbursement/payment-request workflow rather than treating it as an expedited pre-service coverage determination.

## Exception requests

When an exception requires clinical support, the exact EOCs instruct the doctor or other prescriber to provide a **supporting statement** explaining the medical reason for the exception. The prescriber can provide the statement by the plan-accepted phone/fax/mail pathway.

Operationally:

`Exception request -> verify restriction/formulary issue -> obtain/support prescriber statement -> submit through current Part D coverage-decision workflow -> standard or expedited clock as applicable`

## Part D reimbursement branch

If the member **already paid** for the drug:

`receipt / paid claim -> Chapter 7 request for payment -> Aetna Integrated Pharmacy Solutions -> coverage decision -> reimbursement or denial -> appeal if denied`

The exact Part D reimbursement mailing address used by all four current EOCs is:

Aetna Integrated Pharmacy Solutions  
PO Box 52446  
Phoenix, AZ 85072

Exact filing windows:

- Michigan `H9314-001`: **36 months**
- Illinois `H9771-001`: **36 months**
- Virginia `H1610-001`: **36 months**
- New Jersey `H6399-001`: the exact Chapter 7 section located gives the mailing address but **does not state the Part D filing deadline**; confirm through current controlled guidance rather than copying the 36-month rule from another plan.

## Part D EOB branch

The Part D **Explanation of Benefits (EOB)** is a summary of prescription-drug costs and payments. Michigan, Illinois and New Jersey exact EOCs explicitly state that the Part D EOB **is not a bill**.

If the caller says "I got an EOB":

`identify drug/line/amount -> determine whether concern is price, coverage, pharmacy claim, LIS/cost-share or denied drug -> use current Rx system -> explain or route`

Do not start the provider-bill workflow merely because the member says "EOB."

## Virginia: exact Part D coverage-decision contact path

Virginia `H1610-001` is unusually explicit in Chapter 2:

- Part D coverage decisions: **1-855-463-0933**
- hours for Part D coverage-decision line: **24/7**
- fax: **1-877-270-0148**
- mail: **Part D Coverage Determination Pharmacy Department, 4750 S 44th Pl Suite 150, Phoenix, AZ 85040**

Virginia Part D appeals use the same phone and fax, with mail directed to **Part D Appeals Pharmacy Department** at the same Phoenix street address.

This is plan-public contact information, not a substitute for the representative's internal MedCompass workflow.

## Michigan / Illinois / New Jersey public call anchor

The exact Member Handbooks/EOC route drug coverage-decision questions back through the plan's Part D / Chapter 9 process and plan Member Services context:

- Michigan `H9314-001`: **1-855-676-5772**
- Illinois `H9771-001`: **1-866-600-2139**
- New Jersey `H6399-001`: **1-844-362-0934**

Use the current controlled internal Rx workflow for the exact screen, pharmacy-claim messaging, coverage-determination intake path, and transfer/queue behavior.

## Trainer-note resolution: Michigan fax `1-855-259-2087`

The previously uncertain handwritten Michigan fax is **not a mystery number anymore**.

The exact Michigan `H9314-001` EOC lists **1-855-259-2087** as:

- the plan's **Member Services fax** in the EOC contact section; and
- the fax for **Best Available Evidence (BAE)** documentation used to correct LIS / prescription copayment-level information.

The same number also appears as the general Member Services fax in the Virginia FIDE EOC.

### Consequence

Do **not** label `1-855-259-2087` as the Michigan medical prior-authorization fax. Michigan's verified 2026 medical PA fax is **1-844-241-2495**. The `1-855-259-2087` trainer note should be classified as **valid public plan contact / exact trainer context still to be identified**.

## Best Available Evidence / LIS clue

Michigan's EOC says BAE documentation can be sent to:

- fax **1-855-259-2087**; or
- the EOC-listed BAE/LIS mailbox.

When a member says their prescription copay / Extra Help level looks wrong, this creates a distinct branch from a formulary rejection:

`wrong LIS/cost-share level -> verify eligibility/system status -> BAE/LIS workflow if applicable -> do not treat as ordinary PA or formulary denial`

Exact internal handling remains controlled-source dependent.

## Rx issue classifier for the eventual desk aid

| Caller issue | First operational bucket |
|---|---|
| "Pharmacy says not covered" | Drug List / restriction / formal coverage-decision check |
| "Needs prior authorization" | Part D restriction + current Rx/PA workflow |
| "They only gave me X tablets" | Quantity-limit / days-supply / formulary-rule check |
| "They want me to try another drug" | Step-therapy / exception workflow |
| "I paid cash" | Chapter 7 Part D reimbursement |
| "My copay is wrong" | LIS / cost-share / eligibility / BAE check before assuming pharmacy error |
| "I got an EOB" | EOB explanation; EOB is not a bill |
| "I need this drug now" | Determine whether expedited coverage-decision criteria apply; reimbursement for an already-purchased drug is a different path |
| "They denied it" | Determine whether there is a formal coverage determination; if yes, Part D appeal/redetermination path |

## Still internal / unresolved

- exact MedCompass `RX` navigation and fields;
- pharmacy paid/rejected claim-message interpretation;
- formulary lookup tool used by this queue;
- internal Part D coverage-determination transfer/queue process for MI/IL/NJ;
- internal BAE/LIS intake process;
- plan-specific handling of Medicaid-only drugs vs Medicare Part D drugs;
- exact New Jersey Part D reimbursement filing deadline;
- required note-template language for Rx calls.
