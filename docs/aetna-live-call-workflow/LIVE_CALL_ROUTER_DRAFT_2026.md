# Aetna Medicare SNP — Live-Call Router Draft

**Working draft — 2026**  
**Audience:** Member Services peer quick reference  
**Design goal:** answer in seconds: **What plan? Where do I look? What do I verify? What do I do next?**

> Public-safe draft. Exact internal authentication elements, proprietary screen paths, transfer queues and note-template fields are intentionally omitted.

---

## 1. START EVERY CALL

`LANGUAGE NEED? -> AUTHENTICATE -> PLAN/STATE -> EXACT 2026 EOC -> CALL REASON -> WORKFLOW -> RESOLUTION -> REQUIRED AETNA NOTES`

### Plan selector

| IVR / plan cue | Contract/PBP | Exact 2026 plan source | Member Services |
|---|---|---|---|
| **Michigan HIDE** | `H9314-001` | MI D-SNP Member Handbook/EOC | 1-855-676-5772 |
| **Illinois FIDE** | `H9771-001` | IL D-SNP Member Handbook/EOC | 1-866-600-2139 |
| **Virginia FIDE** | `H1610-001` | VA 2026 EOC | 1-855-463-0933 |
| **New Jersey FIDE** | `H6399-001` | NJ 2026 EOC | 1-844-362-0934 |
| **C-SNP** | **PENDING** | Exact contract/PBP required before quoting plan benefit | — |

**Hard rule:** HIDE/FIDE/C-SNP tells you which workflow branch to enter. It does **not** prove the exact benefit.

---

## 2. WHY IS THE MEMBER CALLING?

### EXTRA BENEFITS CARD / “FOOD CARD” / OTC

**LOOK HERE**  
Exact EOC + current card/OTC benefit source.

**VERIFY**

- exact plan;
- OTC Wallet vs Extra Supports Wallet;
- current balance;
- qualifying Extra Supports/SSBCI status when food/utilities/transport/personal-care spending is requested;
- participating merchant + eligible item/category;
- current benefit month.

**2026 monthly OTC Wallet**

- MI `H9314-001` — **$220/month**
- IL `H9771-001` — **$225/month**
- VA `H1610-001` — **$280/month**
- NJ `H6399-001` — **$255/month**

Unused monthly amount does not roll over in current plan materials.

**DO THIS**

`Decline -> activation -> correct wallet -> balance -> merchant -> item/category -> benefit period -> current card-support workflow`

**DON'T**

- Do not promise food/utilities solely because the member has a D-SNP.
- Do not confuse Extra Supports transportation spending with NEMT ride scheduling.
- Do not route every card issue to an old trainer-number shortcut.

---

### “I GOT A BILL”

**LOOK HERE**  
Claim + exact EOC Chapter 7/payment rules.

**VERIFY**

- provider/facility;
- date of service;
- claim status/disposition;
- network status **on date of service**;
- authorization/continuity exception if relevant;
- documented member responsibility;
- whether member already paid.

**DO THIS**

`Bill -> claim -> responsibility -> provider correction / payment request / appeal as applicable`

If already paid:

`Bill + proof of payment -> medical/Part B vs Part D -> filing window -> reimbursement request`

**DON'T**

**A bill alone does not prove the member owes it.**

---

### CLAIM

**FIND -> READ -> DETERMINE -> ACT**

**VERIFY**

- exact claim/service date;
- paid / pending / denied / adjusted status;
- member responsibility;
- denial/disposition reason;
- network/authorization context;
- whether corrected claim, adjustment, reprocessing or appeal is appropriate.

Exact claim-screen interpretation and reprocessing steps remain controlled internal workflow.

---

### APPEAL / GRIEVANCE

**CLASSIFY FIRST**

`Medicare or Medicaid? -> Medical/service or Part D? -> Coverage decision, appeal or grievance? -> Standard or expedited? -> Exact plan/state route`

**Critical trigger:**

**SERVICE BEING REDUCED OR STOPPED? -> CHECK CONTINUATION / AID-PENDING DEADLINE FIRST.**

General findings from exact EOCs:

- standard grievance resolution: generally no later than **30 calendar days**;
- EOC-defined expedited grievance: **24 hours**;
- Medicare Level 2 may be an IRO/IRE;
- Medicaid Fair/State Hearing routes differ by state;
- **Maximus is not a universal Level-2 label.**

---

### RIDE / TRANSPORTATION

**LOOK HERE**  
Exact plan + state transportation source/current controlled workflow.

**DO THIS**

`Plan/state -> confirm transportation benefit -> plan-specific scheduling route -> conference/schedule per current workflow -> confirm outcome -> notes`

**DON'T**

Do not use one universal MTM/Modivcare number across all states.

Current safe routing anchors:

- MI HIDE — Member Services/Care Coordinator path first; current HIDE page uses 1-855-676-5772 and 3-business-day advance language for regular rides.
- IL FIDE — Member Services/Care Coordinator is the durable anchor; direct MTM source numbers conflict across current materials.
- VA FIDE — Medicare EOC confirms $0 NEMT but refers to Medicaid-side detail; use exact current plan route.
- NJ FIDE — current plan page routes ride setup help through 1-844-362-0934; EOC also identifies Medicaid FFS/Modivcare context.

---

### PROVIDER / PCP / NETWORK

**DO THIS**

`Exact plan -> PCP or specialist -> exact-plan network status -> accepting new patients -> referral? -> PA? -> continuity/OON exception? -> resolve`

**Key 2026 findings**

- All four plans allow PCP change through Member Services.
- Verify requested PCP is in the exact plan network and accepting new patients.
- All four exact EOCs state members can use a network specialist without a PCP referral, though service-specific orders/PA may still apply.
- Routine unauthorized OON care may be denied; emergency/urgent/dialysis/network-unavailable/authorized continuity exceptions must be checked in the exact EOC.
- Provider participation today is not necessarily provider status on the date of service.

**Provider says “we don't take Aetna”**

Verify the **exact contract/network + location**. A provider may accept some Aetna products but not this D-SNP.

---

### PRIOR AUTHORIZATION

**DO THIS**

`Exact service -> exact plan -> EOC/PA requirement -> current internal PA lookup -> provider/current plan route -> status/next action`

Public 2026 plan-specific medical PA anchors:

| Plan | Public phone | Public PA fax |
|---|---:|---:|
| MI H9314-001 | 1-855-676-5772 | 1-844-241-2495 |
| IL H9771-001 | 1-866-600-2139 | 1-855-320-8445 |
| VA H1610-001 | 1-855-463-0933 | 1-833-280-5224 |
| NJ H6399-001 | 1-844-362-0934 | 1-833-322-0034 |

**Critical distinction:** a Member Services/coverage-decision fax is not automatically the provider PA-submission fax.

---

### RX / PHARMACY

**CLASSIFY**

- “Not covered” -> Drug List/restriction/coverage-decision check
- “Needs PA” -> Part D restriction + current internal Rx/PA workflow
- “Only gave X tablets” -> quantity limit / days supply
- “Must try another drug” -> step therapy / exception
- “I paid cash” -> Part D reimbursement
- “My copay is wrong” -> LIS/cost share / BAE branch
- “I got an EOB” -> EOB explanation; **not a bill**
- “I need it now” -> expedited criteria if drug not already obtained
- “They denied it” -> determine whether a formal coverage determination exists -> redetermination/appeal

Part D coverage decision clocks in exact EOCs are generally **72 hours standard / 24 hours expedited** once required supporting information is received.

---

### CARE MANAGEMENT

Aetna's current Medicare care-management material states C-SNP and D-SNP members automatically get a care manager; intensity varies by need.

**Strong CM/CC route triggers**

- HRA/care plan;
- complex chronic coordination;
- post-discharge needs;
- behavioral-health coordination;
- LTSS/MLTSS;
- community resources;
- multiple-provider coordination;
- transportation navigation;
- plan benefit eligibility/setup when EOC assigns Care Management responsibility.

**Working pattern**

`Need -> exact plan -> assigned CM/CC -> connect/referral under current controlled workflow -> confirm outcome -> required notes`

---

## 3. QUICK RED-TEAM STRIP

- **Benefit amount?** Exact EOC first.
- **Vendor number?** Verify state/plan; no universal vendor strip.
- **Bill?** Claim first; bill != liability.
- **OON?** Check exact exception/authorization/continuity rule.
- **Appeal?** Medicare vs Medicaid + medical vs Part D before routing.
- **Service stopping?** Aid-pending/continuation deadline first.
- **Rx copay wrong?** LIS/BAE is different from formulary denial/medical PA.
- **Food/utilities?** Extra Supports qualification first.
- **Gas/Uber vs doctor ride?** Card transportation category != NEMT.
- **Old training screenshot?** Check source date and current 2026 plan/workflow before using.

---

## 4. INTERNAL ITEMS STILL NEEDED BEFORE FINAL DESK AID

- exact IVR wording/plan cue presentation;
- exact internal EOC lookup path;
- required call-tracking/note template fields;
- claim lookup/status/reprocessing workflow;
- ProPAT navigation;
- MedCompass PA and Rx navigation;
- G&A intake/status/transfer workflow;
- assigned CM lookup/referral steps;
- current vendor conference/transfer rules;
- exact C-SNP state + contract/PBP + MarketProminence workflow.

Until those are captured, the public-source content is strong enough for plan facts and decision logic, but the private live-call aid should not invent internal clicks, queues or permissions.
