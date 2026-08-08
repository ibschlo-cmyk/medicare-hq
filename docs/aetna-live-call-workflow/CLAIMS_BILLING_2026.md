# 2026 Aetna D-SNP Claims, Bills & Member Reimbursement

**Status:** Exact-EOC public-source workflow baseline  
**Updated:** 2026-08-08  
**Scope:** `H9314-001`, `H9771-001`, `H1610-001`, `H6399-001`

> This file covers the **member-facing bill / request-for-payment workflow** found in Chapter 7 of the exact 2026 plan documents. It does not replace Aetna's internal claim-status, adjustment, correction, reprocessing, provider-call, or escalation workflow.

## First distinction: bill, EOB, or claim?

A fast live-call split is:

| What the member has | What it means operationally |
|---|---|
| **Provider bill** | Do not assume the member owes it. Identify provider, service/date, claim and documented member responsibility before advising payment. |
| **Part D Explanation of Benefits (EOB)** | A summary of Part D drug costs/payments. The exact EOCs explicitly say the EOB **is not a bill**. |
| **Member already paid** | Potential **request for payment / reimbursement** workflow. Collect the bill plus proof of payment and apply the exact plan's Chapter 7 filing rules. |
| **Provider-submitted claim** | Use the current internal claims system to locate/read the claim. The EOC does not replace internal claim-status or reprocessing procedures. |

## Canonical bill workflow

`BILL -> identify provider/service/date -> determine whether member already paid -> locate claim -> read claim disposition/member responsibility -> exact EOC Chapter 7 + internal claims workflow -> resolve / reimbursement / provider action / appeal`

### Core rule

A bill alone does **not** establish member liability. The exact EOCs tell members that network providers should bill the plan directly. When a network-provider bill appears to be wrong, the plan can contact the provider and address the billing problem. If the member already paid for a covered service, the EOCs provide a reimbursement/request-for-payment process.

## Member reimbursement / request-for-payment matrix

### Medical services, items and Part B drugs

| Plan | Filing deadline | Mailing address | Member Services |
|---|---:|---|---|
| Michigan HIDE `H9314-001` | **12 months** from service/item/Part B drug date | Aetna Medicare HIDE (HMO D-SNP) / Aetna Duals COE Member Correspondence / PO Box 982980 / El Paso, TX 79998 | **1-855-676-5772** |
| Illinois FIDE `H9771-001` | **12 months** | Aetna Medicare FIDE (HMO D-SNP) / Aetna Duals COE Member Correspondence / PO Box 982980 / El Paso, TX 79998 | **1-866-600-2139** |
| Virginia FIDE `H1610-001` | **12 months** | Aetna Medicare FIDE (HMO D-SNP) / Aetna Duals COE Member Correspondence / PO Box 982980 / El Paso, TX 79998 | **1-855-463-0933** |
| New Jersey FIDE `H6399-001` | **12 months** | Aetna Medicare FIDE (HMO D-SNP) / Aetna Duals COE Member Correspondence / PO Box 982980 / El Paso, TX 79998 | **1-844-362-0934** |

The Chapter 7 sections tell members to send the **bill plus proof of any payment**. Proof can include a receipt or copy of the check/payment record described by the plan. Members should keep copies for their records.

### Part D prescription drug reimbursement

| Plan | Filing deadline stated in exact 2026 EOC | Mailing address |
|---|---:|---|
| Michigan HIDE `H9314-001` | **36 months** from date Part D drug was obtained | Aetna Medicare HIDE (HMO D-SNP) / Aetna Integrated Pharmacy Solutions / PO Box 52446 / Phoenix, AZ 85072 |
| Illinois FIDE `H9771-001` | **36 months** | Aetna Medicare FIDE (HMO D-SNP) / Aetna Integrated Pharmacy Solutions / PO Box 52446 / Phoenix, AZ 85072 |
| Virginia FIDE `H1610-001` | **36 months** | Aetna Medicare FIDE (HMO D-SNP) / Aetna Integrated Pharmacy Solutions / PO Box 52446 / Phoenix, AZ 85072 |
| New Jersey FIDE `H6399-001` | **Not stated in the Chapter 7 payment-request section located in the exact EOC** | Aetna Medicare FIDE (HMO D-SNP) / Aetna Integrated Pharmacy Solutions / PO Box 52446 / Phoenix, AZ 85072 |

**Red-team rule:** do not automatically quote the 36-month Part D filing limit to New Jersey merely because the other three exact EOCs state it. The New Jersey Chapter 7 section located here gives the pharmacy mailing address but does not state that deadline. Use current controlled plan guidance for the NJ Part D filing limit.

## Claim form: useful, but generally not mandatory

Michigan, Illinois and New Jersey explicitly say the member **is not required** to use the claim/request-for-payment form, although using it can speed processing. Virginia says the form is available and helps provide the information needed for the decision; the request can be made by calling or in writing.

For a live call, the operational question is therefore not simply **"Do they have the form?"** It is:

`Do they have the bill + proof of payment + enough service/provider information for the request?`

Then follow the exact current internal process for form issuance/submission assistance.

## What happens after the request is received

Across the exact EOCs, Aetna treats the payment request as a **coverage decision**:

1. The plan reviews whether the service, item or drug is covered and whether plan rules were followed.
2. The plan may request additional information.
3. If covered and already paid, the plan reimburses the appropriate covered share/amount under the plan rules.
4. If not yet paid, the plan may pay the provider directly.
5. If the plan denies payment, it sends the reason and the member has **appeal rights**.

For Part D reimbursement, the exact EOCs caution that a member may not receive the full cash amount paid if, for example, the cash price exceeded the plan's negotiated price or an out-of-network pharmacy rule applies.

## Common situations that trigger Chapter 7

The exact EOCs repeatedly identify situations such as:

- emergency or urgently needed care from an out-of-network provider;
- a network provider bills the member by mistake;
- retroactive plan enrollment after the member already paid;
- out-of-network pharmacy use in a permitted circumstance;
- paying full prescription cost because the plan membership card was unavailable; and
- paying for a drug when coverage/restriction status was unclear.

Do not reduce these to one reimbursement promise. Coverage, network rules and required documentation still control.

## Operational split: provider bill vs. member-paid reimbursement

### Member has **not** paid

`Bill -> claim lookup -> verify provider/network/service -> verify documented member responsibility -> if improper bill, use current provider/claims correction path; Chapter 7 supports sending the bill to the plan rather than treating it as proof of debt.`

### Member **already paid**

`Bill + proof of payment -> determine medical/Part B vs Part D -> check filing window -> use correct request-for-payment path -> document -> if payment request denied, explain appeal rights / route under current A&G workflow.`

## EOB branch

For Part D, Michigan, Illinois and New Jersey exact EOCs explicitly describe the **Explanation of Benefits (EOB)** as a periodic summary of drug costs and payments and state that it **is not a bill**. Virginia likewise uses the Part D EOB as the plan's drug-cost/payment summary; if the member's concern is an EOB rather than a provider bill, first identify the line/drug/amount they are questioning rather than starting a reimbursement workflow.

## Still internal / unresolved

The following remain controlled-workflow items and should not be invented from public EOCs:

- exact claim-search screen and search keys;
- paid / denied / pending / adjusted / corrected status vocabulary;
- claim-line interpretation;
- provider call/conference rules;
- corrected claim vs adjustment vs reprocessing procedure;
- Medicaid crossover / coordination handling in the claims system;
- internal escalation queues and ownership;
- when a Member Services representative should issue a form versus transfer/conference;
- New Jersey Part D reimbursement filing deadline;
- required Aetna note-template language.

## Desk-aid version

The high-speed branch can be compressed to:

**BILL?** `Don't assume owed -> claim -> member responsibility -> provider action / Chapter 7`

**ALREADY PAID?** `Bill + proof -> Medical/Part B: 12 mo -> Part D: exact plan rule -> reimbursement request`

**EOB?** `Not a bill -> identify questioned drug/amount -> explain or route`

**DENIED REIMBURSEMENT?** `Coverage decision -> appeal path`
