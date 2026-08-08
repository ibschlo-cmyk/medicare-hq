# Aetna Live-Call Workflow — Placeholder Framework (2026)

**Status:** Deliberate placeholders for missing controlled/internal source material  
**Updated:** 2026-08-08  
**Purpose:** Keep the live-call aid build moving without inventing procedures. Every `[PENDING SOURCE]` block is a slot to replace when a current Aetna source is captured.

> Rule: placeholders are not instructions. Until replaced, use the current controlled Aetna production workflow and exact 2026 EOC/Member Handbook.

## Placeholder status legend

- `[PENDING SOURCE]` — no current controlled source captured yet
- `[PARTIAL SOURCE]` — some current material exists, but the exact screen/path/field is still missing
- `[VERIFIED]` — current source captured and reconciled
- `[HISTORICAL ONLY]` — useful older material exists but must not drive current handling

---

## 1. IVR / Incoming Call Identification

**Status:** `[PENDING SOURCE]`

**Known now:** use the IVR cue to identify state/plan context before benefit handling.

**Placeholder workflow:**

`Incoming call -> [IVR CUE PLACEHOLDER] -> [PLAN/STATE DISPLAY PLACEHOLDER] -> confirm HIDE/FIDE/C-SNP -> open exact plan source`

**Capture needed:**
- exact wording shown/spoken by IVR;
- where state/plan type appears;
- whether contract/PBP appears;
- any queue/line identifier that changes handling.

**Do not infer:** exact IVR phrasing from trainer memory.

---

## 2. Internal EOC / Member Handbook Lookup

**Status:** `[PENDING SOURCE]`

**Placeholder workflow:**

`Exact plan/state -> [EOC LOOKUP ENTRY POINT] -> [SEARCH FIELD] -> [CONTRACT/PBP MATCH] -> [2026 DOCUMENT CONFIRMATION] -> open EOC`

**Capture needed:**
- system/page used;
- search terms;
- how plan year is confirmed;
- how contract/PBP is displayed;
- what to do if more than one result appears.

**Interim safe rule:** exact plan EOC/Member Handbook remains the benefit authority.

---

## 3. Required Aetna Call Tracking / Notes Template

**Status:** `[PENDING SOURCE]`

**Hard rule:** do **not** substitute a custom note template.

**Placeholder fields:**

- `[REQUIRED OPENING FIELD]`
- `[CALL REASON FIELD]`
- `[VERIFICATION/AUTH FIELD AS PER CURRENT AETNA TEMPLATE]`
- `[SYSTEMS/SOURCES USED FIELD]`
- `[ACTION TAKEN FIELD]`
- `[TRANSFER/CONFERENCE/ESCALATION FIELD]`
- `[OUTCOME/RESOLUTION FIELD]`
- `[FOLLOW-UP/NEXT STEP FIELD]`
- `[REQUIRED DISPOSITION/CODE FIELD]`
- `[REQUIRED CLOSING FIELD]`

**Capture needed:** blank/current template, required fields, mandatory disposition/resolution coding, and any special notes requirements by workflow.

---

## 4. Claims — Lookup / Status / Liability / Reprocessing

**Status:** `[PARTIAL SOURCE]`

**Known current structure:** `FIND -> READ -> DETERMINE -> ACT`

**Placeholder workflow:**

`Member issue -> [CLAIM SEARCH SCREEN] -> [CLAIM IDENTIFIER] -> [STATUS FIELD] -> [DISPOSITION/REASON FIELD] -> [MEMBER RESPONSIBILITY FIELD] -> [NETWORK/AUTH CONTEXT] -> choose action`

**Status placeholders to map exactly:**
- `[PAID STATUS]`
- `[DENIED STATUS]`
- `[PENDING STATUS]`
- `[ADJUSTED/CORRECTED STATUS]`
- `[NOT FOUND STATUS]`
- `[VOID/REVERSED STATUS IF APPLICABLE]`

**Action placeholders:**
- `[PROVIDER CORRECTION/REBILL PATH]`
- `[ADJUSTMENT/REPROCESSING PATH]`
- `[MEMBER REIMBURSEMENT PATH]`
- `[APPEAL PATH]`
- `[ESCALATION PATH]`

**Capture needed:** current claim screen, status vocabulary, denial/reason codes, member-liability location, reprocessing steps, and escalation criteria.

---

## 5. "I Got a Bill" — Internal Resolution Path

**Status:** `[PARTIAL SOURCE]`

**Known safe structure:**

`Bill -> provider/service/date -> claim -> disposition -> QMB on DOS if relevant -> documented member responsibility -> action`

**Placeholders:**
- `[WHERE MEMBER RESPONSIBILITY IS DISPLAYED]`
- `[PROVIDER BILLING ERROR PATH]`
- `[SECONDARY/MEDICAID COORDINATION PATH]`
- `[BALANCE-BILLING ESCALATION PATH]`
- `[MEMBER ALREADY PAID PATH]`
- `[SEND BILL/PROOF OF PAYMENT WORKFLOW]`

**Hard rule:** bill received ≠ member liability.

---

## 6. ProPAT — PA Requirement Check

**Status:** `[PENDING SOURCE]`

**Known trainer cue:** ProPAT is used to check whether PA is required.

**Placeholder workflow:**

`Exact plan -> exact service/procedure -> [OPEN PROPAT] -> [ENTER SERVICE/CODE] -> [PLAN/DATE INPUT] -> [PA REQUIRED RESULT] / [PA NOT REQUIRED RESULT] -> [NEXT ACTION]`

**Capture needed:** exact navigation, fields, code lookup behavior, result language, date-of-service logic, exceptions, and what to document.

---

## 7. MedCompass — Prior Authorization

**Status:** `[PENDING SOURCE]`

**Known trainer cue:** MedCompass -> Prior Auth create/check.

**Placeholder workflow:**

`Member/service -> [OPEN MEDCOMPASS] -> [PA SEARCH] -> [AUTH STATUS] -> [REASON/DETAIL] -> [CREATE/CHECK ACTION] -> [PROVIDER/MEMBER NEXT STEP] -> notes`

**Status placeholders:**
- `[APPROVED]`
- `[PENDING]`
- `[DENIED]`
- `[VOID/CANCELLED]`
- `[NO AUTH FOUND]`
- `[MORE INFORMATION NEEDED]`

**Capture needed:** exact search fields, auth number location, service dates, units, provider details, decision reason, create/check path, escalation.

---

## 8. MedCompass — Rx / Pharmacy

**Status:** `[PENDING SOURCE]`

**Known trainer cue:** MedCompass -> RX.

**Placeholder workflow:**

`Rx issue -> [OPEN RX AREA] -> [DRUG/CLAIM/RESTRICTION LOOKUP] -> classify -> [PA / QL / ST / NON-FORMULARY / LIS-BAE / REIMBURSEMENT / APPEAL] -> current action`

**Placeholders:**
- `[FORMULARY STATUS]`
- `[PA STATUS]`
- `[QUANTITY LIMIT]`
- `[STEP THERAPY]`
- `[PHARMACY REJECTION/CLAIM MESSAGE]`
- `[LIS/BAE DISPLAY]`
- `[COVERAGE DETERMINATION PATH]`
- `[REDETERMINATION/APPEAL PATH]`

---

## 9. Appeals & Grievances — Intake / Status / Transfer

**Status:** `[PARTIAL SOURCE]`

**Known structure:** classify Medicare vs Medicaid, medical/service vs Part D, appeal vs grievance, standard vs expedited, and continuation/aid-pending triggers before routing.

**Placeholder workflow:**

`Issue -> [G&A INTAKE SCREEN] -> [CASE TYPE] -> [JURISDICTION] -> [STANDARD/EXPEDITED] -> [CONTINUATION/AID-PENDING CHECK] -> [QUEUE/ROUTE] -> [STATUS LOOKUP] -> [NEXT LEVEL] -> notes`

**Placeholders:**
- `[MEDICARE MEDICAL APPEAL ROUTE]`
- `[MEDICAID APPEAL ROUTE BY STATE]`
- `[PART D APPEAL ROUTE]`
- `[GRIEVANCE ROUTE]`
- `[EXPEDITED ROUTE]`
- `[CONTINUATION/AID-PENDING ACTION]`
- `[G&A STATUS FIELD]`
- `[TRANSFER/CONFERENCE RULE]`

**Do not use:** one universal `Aetna -> Maximus -> State Hearing` ladder.

---

## 10. Care Management / Care Coordinator

**Status:** `[PENDING SOURCE]`

**Known trainer cue:** Member CM Info Report -> Care Manager.

**Placeholder workflow:**

`Need identified -> [MEMBER CM INFO REPORT] -> [ASSIGNED CM/CC FIELD] -> [CONTACT/STATUS] -> [WARM TRANSFER / MESSAGE / REFERRAL] -> confirm outcome -> notes`

**Capture needed:** assignment field, phone/queue, availability/status, referral process, urgent criteria, warm-transfer rules, documentation.

---

## 11. Vendor Handling — Conference vs Transfer vs Give Number

**Status:** `[PARTIAL SOURCE]`

**Known:** plan-specific vendor/contact data is substantially mapped; **handling behavior** remains incomplete.

For each vendor category, fill:

| Category | Plan | Give number? | Cold transfer? | Warm transfer? | Conference? | Rep schedules? | Source |
|---|---|---|---|---|---|---|---|
| OTC / Extra Benefits | `[PLAN]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[PENDING]` |
| Transportation | `[PLAN]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[PENDING]` |
| Dental | `[PLAN]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[PENDING]` |
| Vision | `[PLAN]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[PENDING]` |
| Hearing | `[PLAN]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[PENDING]` |
| PERS | `[PLAN]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[PENDING]` |
| In-home support | `[PLAN]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[PENDING]` |

---

## 12. C-SNP `H1206-004` / MarketProminence

**Status:** `[PARTIAL SOURCE]`

**Known plan:** Illinois — Aetna Medicare Prime Chronic Care (HMO C-SNP) — `H1206-004`.

**Placeholder workflow:**

`C-SNP call -> identify H1206-004 -> [MARKETPROMINENCE ENTRY POINT] -> [MEMBER/ENROLLMENT LOOKUP] -> [CHRONIC CONDITION VERIFICATION STATUS] -> [ENROLLMENT/DISENROLLMENT STATUS] -> exact 2026 EOC -> issue workflow`

**Placeholders:**
- `[MARKETPROMINENCE URL/ENTRY]`
- `[MEMBER LOOKUP FIELDS]`
- `[VCC/QUALIFYING CONDITION STATUS]`
- `[PENDING VERIFICATION STATUS]`
- `[VERIFIED STATUS]`
- `[FAILED/NO VERIFICATION STATUS]`
- `[ENROLLMENT STATUS]`
- `[DISENROLLMENT PATH]`

**Still needed:** exact Aetna-hosted 2026 EOC PDF URL and current internal MarketProminence screens/path.

---

## 13. Provider Calls

**Status:** `[PARTIAL SOURCE]`

**Known current principle:** provider calls must be handled through the current provider-call workflow; member callers should not simply be transferred into provider-only destinations.

**Placeholder workflow:**

`Provider call -> [PROVIDER AUTHENTICATION] -> [MEMBER LOOKUP] -> [NETWORK/PROVIDER CONTEXT] -> classify eligibility/benefit vs claim vs PA vs pharmacy vs appeal -> [CORRECT PROVIDER ROUTE]`

**Placeholders:**
- `[PROVIDER AUTH FIELDS]`
- `[ELIGIBILITY/BENEFIT PATH]`
- `[CLAIM STATUS PROVIDER PATH]`
- `[MEDICAL PA PROVIDER PATH]`
- `[PHARMACY PROVIDER PATH]`
- `[PROVIDER APPEAL PATH]`

---

## 14. Closing / Required End-of-Call Steps

**Status:** `[PENDING SOURCE]`

**Placeholder close:**

`Confirm issue addressed -> [RESTATE OUTCOME] -> [NEXT STEP/EXPECTED TIMEFRAME] -> [CONTACT/VENDOR ACTION CONFIRMATION] -> [REQUIRED CLOSING SCRIPT IF ANY] -> complete Aetna notes -> [DISPOSITION]`

**Capture needed:** required closing language, documentation timing, disposition/codes, unresolved-call escalation, follow-up commitments.

---

# Replacement protocol

When a source is uploaded:

1. Identify source title/revision/effective date.
2. Tag it as controlled Aetna, trainer-provided, exact EOC/plan-specific, verified external, historical, or unresolved.
3. Replace only the matching `[PENDING SOURCE]` / `[TBD]` fields supported by that source.
4. Preserve conflicts instead of silently reconciling them.
5. Red-team the replacement against the exact plan/EOC and newer controlled sources.
6. Keep proprietary screen-by-screen details in the private second-brain layer; publish only safe high-level dependencies here.

# Completion target

The placeholder framework is complete when the live-call aid can answer:

**WHAT PLAN? -> WHAT IS THE MEMBER/PROVIDER CALLING ABOUT? -> WHERE DO I LOOK? -> WHAT DO I VERIFY? -> WHAT DO I CLICK/DO NEXT? -> HOW DO I DOCUMENT/CLOSE?**
