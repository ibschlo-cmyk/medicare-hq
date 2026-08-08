# 2026 Aetna Extra Benefits Card Live-Call Workflow

**Status:** Current Aetna public-source + exact-plan baseline  
**Updated:** 2026-08-08  
**Scope:** Current Aetna D-SNP plan anchors and future C-SNP branch

> The card itself is not enough to determine what the member can buy. **Plan + wallet + eligibility + current balance + participating merchant/product** control the answer.

## Four-plan monthly OTC Wallet matrix

| Plan | 2026 monthly amount |
|---|---:|
| Michigan HIDE `H9314-001` | **$220/month** |
| Illinois FIDE `H9771-001` | **$225/month** |
| Virginia FIDE `H1610-001` | **$280/month** |
| New Jersey FIDE `H6399-001` | **$255/month** |

The allowance is available at the start of the applicable monthly benefit period and unused amounts do **not** roll over to the next month under the current plan materials.

## Wallet logic

Aetna's current Medicare material describes several possible Extra Benefits Card wallets. For this D-SNP workflow, the critical distinction is:

- **OTC Wallet / CVS OTC Wallet:** approved OTC health and wellness products only.
- **Extra Supports Wallet:** approved OTC products **plus** additional approved spending categories when the member meets the plan's qualifying chronic-condition / SSBCI rules. Categories can include healthy foods, personal-care products, utilities and transportation.

A D-SNP label by itself does **not** prove the member has the Extra Supports Wallet.

## High-speed live-call branch

`CARD ISSUE -> exact plan -> identify wallet -> verify qualification/status -> check balance -> check merchant/product/category -> resolve / CVS card support / Member Services / Care Management as appropriate -> required notes`

## Issue classifier

| Member says | First things to verify |
|---|---|
| **"My card was declined"** | Card activated? Correct wallet? Current balance enough? Merchant participates? Item/category eligible? Benefit period current? If all look correct, use current card-support workflow. |
| **"How much do I have left?"** | Exact plan + current wallet/balance. Current Aetna plan pages allow members to view allowances/balances at `CVS.com/Aetna`. |
| **"Can I buy food?"** | Do **not** answer from D-SNP status alone. Verify Extra Supports Wallet / qualifying-condition eligibility. OTC-only members cannot use the allowance for healthy foods. |
| **"Can I pay utilities?"** | Verify Extra Supports Wallet and approved utility/payment method. Do not promise late fees or non-approved bill types. |
| **"Can I buy gas / use Uber or Lyft?"** | Verify Extra Supports Wallet + plan-specific approved transportation category/payment method. This is separate from the plan's non-emergency medical transportation scheduling benefit. |
| **"What stores/items can I use?"** | Use participating-store and approved-product lookup at `CVS.com/Aetna` / current internal card tool. Not every product in a participating store is eligible. |
| **"I lost my card" / "I need another one"** | Current Aetna plan pages support replacement-card requests through `CVS.com/Aetna`; follow current internal replacement workflow if assisting directly. |
| **"How do I activate it?"** | Aetna says activation instructions are provided with the card; `CVS.com/Aetna` / CVS OTC Health Solutions tools can manage activation. |
| **"My money disappeared"** | Check benefit period and transaction history/balance. Current plan materials say unused monthly amounts do not roll over. |
| **"I have a chronic condition but food/utilities won't work"** | Verify whether the qualifying condition has actually been recognized for SSBCI/Extra Supports Wallet, not merely whether the member reports a diagnosis. Escalate/route under the plan's eligibility workflow. |

## Current Aetna card-management channels

Current Aetna Medicare / plan pages identify:

- **Online:** `CVS.com/Aetna`
- **OTC ordering / card-benefit support used in current Aetna materials:** **1-844-428-8147 (TTY 711)**
- Phone ordering hours on Aetna's current OTC page: **8 AM-8 PM local time, 7 days/week, excluding federal holidays**; automated ordering is available 24/7.

The online experience supports plan/card functions such as:

- activation;
- allowance and balance lookup;
- participating-store lookup;
- approved-product lookup;
- online ordering; and
- replacement-card requests.

Do not substitute an older trainer number for the current card-support path without plan/current-workflow confirmation.

## Trainer OTC number `1-866-799-3832`

The trainer note `OTC — 1-866-799-3832 — M-F 8a-8p` has plan-document support in Michigan and Illinois for a **fall-prevention/home-safety product ordering** channel. Current evidence does **not** establish it as the universal Extra Benefits Card help line.

Therefore:

- retain it as a specialized trainer/plan lead;
- do not use it for every decline, balance, replacement or Extra Supports question;
- use the current controlled card workflow / `CVS.com/Aetna` / current plan source first.

## New Jersey `H6399-001` — especially clear current workflow

The current New Jersey FIDE plan page, updated July 20, 2026, states:

- **$255/month** in 2026;
- qualifying members can use the allowance for healthy food, OTC items, transportation, utilities and personal-care items;
- members without a qualifying chronic condition can use the monthly allowance for **OTC items only**;
- the benefit is available on the **first day of each month**;
- unused amount **does not roll over**; and
- `CVS.com/Aetna` supports activation, balance/allowance, store/product lookup, online ordering and replacement.

A 2026 NJ provider-orientation source further says members already identified as qualifying through claims may not need additional action; members without a qualifying condition on file may contact Member Services regarding the condition / provider confirmation process. Treat that as a plan-specific operational clue, not a universal SSBCI adjudication rule.

## Virginia `H1610-001` — current plan page

Virginia's current FIDE benefits page likewise directs members to `CVS.com/Aetna` for:

- activation;
- allowances/balances;
- participating stores/approved products;
- online ordering; and
- replacement cards.

It also identifies healthy foods, OTC, utilities, transportation and personal-care products as Extra Supports categories for qualifying members and limits non-qualifying members to OTC purchasing.

## Critical distinction: card transportation vs. NEMT ride benefit

The **Extra Supports Wallet transportation category** can include approved spending such as gas at the pump, public transportation or rideshare under applicable plan rules.

That is **not the same thing** as the plan's covered **non-emergency medical transportation (NEMT)** benefit, which has separate state/vendor scheduling rules.

Desk-aid split:

`"Can I use my card for gas/Uber?" -> Extra Supports Wallet`

`"I need a ride to my doctor" -> NEMT / plan-state transportation workflow`

## What cannot be answered from public sources alone

- Exact internal balance/card screen used by Member Services
- Internal decline reason codes
- Transaction-history screen and reversal/refund workflow
- Whether the representative should conference or transfer to CVS OTC Health Solutions for each issue type
- Exact SSBCI eligibility flag / claims logic shown in internal systems
- Lost/stolen-card internal replacement procedure
- Required note-template wording
- Any C-SNP wallet amount until the exact C-SNP contract/PBP is identified

## Desk-aid version

**DECLINE?** `activate -> wallet -> balance -> merchant/item -> current card support`

**FOOD / UTILITIES / GAS?** `Extra Supports eligibility first`

**BALANCE / STORES / ITEMS / REPLACEMENT?** `CVS.com/Aetna / current card tool`

**RIDE TO APPOINTMENT?** `NEMT branch, not card branch`

**NEVER:** promise a spending category from `D-SNP` or `C-SNP` alone.
