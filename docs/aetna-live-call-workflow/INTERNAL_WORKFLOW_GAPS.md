# Controlled Internal Workflow Sources — Public-Safe Gap Log

**Updated:** 2026-08-08  
**Purpose:** Track which internal Aetna workflow areas have source material available without publishing proprietary procedures, authentication logic, internal system navigation, restricted contacts, or member-record release procedures.

> This file intentionally contains **no member-authentication identifiers, internal screen-by-screen instructions, restriction/password handling, proprietary PHI-release steps, call-tracking templates, transfer queues, or internal email addresses**. Those details remain in the private working source layer and current controlled Aetna desktop.

## Verification Process — source status upgraded

Internal training screenshots identify a document titled approximately:

**Desktop: 4500.80D Verification Process — Dual Center of Excellence — COE Member Services — Member Services Representatives**

### Scope visible in the supplied source

The source states that the process applies to the four current Center of Excellence plan lines in this project:

- Illinois FIDE D-SNP
- Michigan HIDE D-SNP
- Virginia FIDE D-SNP
- New Jersey FIDE D-SNP

### Recency finding

Earlier project inventory treated the visible verification material as potentially dating to 2020. The later pages of the same supplied source show a change log continuing through:

- 03/2022 annual review
- 12/2022 organizational/header update
- **12/2025 annual review / header update**

That materially changes the source assessment: the supplied Verification Process was still being reviewed in late 2025. It remains an **internal training / controlled-workflow source**, not a public federal HIPAA rule, and current desktop guidance must supersede it if Aetna has changed the procedure since the supplied copy.

## PHI copy-request workflow — separate internal source

A second supplied internal document is titled approximately:

**Desktop: 4500.01D HIPAA Member or Authorized Representative Requests for a Copy of PHI — Dual Center of Excellence — COE Member Services**

### Scope

The source states that it applies to the same four COE plan lines: Illinois FIDE, Michigan HIDE, Virginia FIDE and New Jersey FIDE.

### Purpose

This is a **record-copy / PHI-access request workflow**, not the ordinary live-call authentication procedure. It addresses how Member Services handles a member or authorized representative asking the health plan for copies of member PHI/records such as claim records.

### Recency

The supplied change log shows updates through **12/2024**, when steps for **OneKit access** were added. Earlier entries include 2020 COE-standard changes, a 2021 Michigan-Medicaid-reference removal, 03/2022 privacy-office updates, and 12/2022 header changes.

### Public-safe operational takeaway

The workflow distinguishes a limited/simple records request from a broader or complex PHI-copy request and routes the latter through the plan's formal PHI-access process. It also requires caller verification, enrollment/date-range validation, approved fulfillment workflow, and call documentation.

The exact date-span thresholds, internal ordering system, form identifiers, internal email routing, data elements collected, and call-code/resolution-code details are intentionally excluded from the public repository.

## Public-safe live-call sequence

The desk aid may safely state only the high-level dependency:

`Authenticate under current Aetna process -> identify whether the member wants an explanation or an actual copy of records -> if copy requested, determine whether the request qualifies for the current simple-record fulfillment route or requires the formal PHI-access process -> submit through current controlled workflow -> document`

This prevents a common workflow error: treating **"explain my claim/EOB"** and **"send me copies of my PHI/claim records"** as the same task.

## Documentation source relationship

Both supplied internal sources route the representative back into Aetna's existing call-documentation standards and required templates. This reinforces the project rule:

**Do not create a replacement note template. Use the current Aetna-required template/workflow.**

## Current internal-source gap list

The following remain controlled/internal and should be captured from current Aetna screens or procedures before the private desk aid is finalized:

- exact IVR wording and plan cue presentation;
- exact internal EOC lookup path;
- current authentication / authorized-representative workflow version in production;
- current PHI-copy-request workflow version in production;
- current required Aetna call-tracking/note-template fields;
- claim lookup/status/reprocessing screens;
- ProPAT and MedCompass navigation;
- MedCompass Rx workflow;
- current G&A intake/queue/status workflow;
- assigned Care Manager lookup / referral workflow;
- current vendor conference/transfer instructions by plan;
- C-SNP MarketProminence workflow and exact contract/PBP.

## Publication rule

Internal screenshots and proprietary procedures are source material for the **private second-brain layer only**. Public GitHub may record that a controlled source exists, its visible scope/date, and the resulting high-level workflow dependency, but must not reproduce the operational procedure itself.
