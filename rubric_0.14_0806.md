# ECHO Pre-Submission Review Rubric — CORE v0.1.4 (DRAFT, pending SME validation)

DRAFT for GO Brussels SME review — nothing here is authoritative until initialled. The label
v0.2 is reserved for the version that returns from that review.

Structure follows the six assessment criteria of the Technical Annex §4.2 (embedded verbatim in
the annex below). Criteria surfaced through a worked example (proposal 204289, LAC 2026) rather
than derived from the framework directly carry a provenance mark and a *Basis:* line stating what
grounds them, so the SME can see which criteria are ECHO's own words and which are generalisations
awaiting validation:
- ◆ document- or mechanically-grounded — the requirement is verbatim in the resolved HIP/TA or is
  computed from the form. Only failure mode is a wrong citation or a false arithmetic flag, both
  checkable in seconds; full severity range applies.
- ◇ inference-grounded — a generalisation drawn from one proposal, not yet in any document. This
  is the class that can hallucinate (the CAPRADE error was here); capped at MEDIUM/FLAG until SME
  sign-off — allowed to raise a question, never to declare a blocker.
Both marks share one property: never passed human review, and so deserve the hardest SME scrutiny.

Structure: **Core** applies to every proposal. **Sector modules** apply only when routing matched
that sector. The rubric states WHAT to check; the resolved HIP/TA supplies the answer (deadlines,
amounts, named bodies). A criterion that cannot be assessed because the resolved documents are
silent is reported as "not assessable against loaded documents", never guessed.

Severity: blocker = explicit requirement not met · HIGH = will draw a desk-officer question or is
time-critical · MEDIUM = weakens the proposal · LOW = improvement · FLAG = may be legitimate,
needs a human.

---

## CORE A · Relevance and coverage (TA §4.2-1)

**REL-01 — HIP objective alignment.** Objectives and priorities match the resolved HIP/TA
sections for the sector(s). Judge against the TA's actual named priority list; generic alignment
language without matching it: MEDIUM.

**REL-02 ◆ — Allocation round and deadline.** From the resolved TECHNICAL ANNEX, identify each country
block's allocation round and its indicative receipt date. Where rounds differ, the earliest
applies (regional/multi-country clause). State the operative deadline explicitly; wrong or
unstated deadline assumption: HIGH, time-critical.
*Basis: verbatim in the resolved Technical Annex (allocation-round / earliest-deadline clause). Discovery via 204289 revealed it applies to multi-country actions; the requirement is ECHO's.*

**REL-03 ◆ — Funding-line eligibility per country block.** Check each country block against the
resolved HIP/TA funding scope for its sector (some HIPs exclude sub-regions from specific budget
lines in a given year). A block outside the funded scope needs an explicit justification in the
proposal; unjustified: HIGH.
*Basis: verbatim in the resolved HIP (per-country-block funding scope). The worked example surfaced the Panama block; the rule is the HIP's.*

**REL-04 — Needs assessment basis.** Joint/recent needs assessments used and named; local
partners included in assessment efforts. Generic or undated needs language: MEDIUM.

**REL-05 — Duration rules.** Check duration against the resolved TA's allocation-round text
(e.g. minimum initial durations for DP and EiE actions unless justified).

**REL-06 — Horizontal requirements named in the resolved HIP/TA.** E.g. nature-based solutions,
DRR mainstreaming, climate/environment integration — check whichever the resolved documents
require. Absent without justification: LOW.

## CORE B · Capacity, expertise and localisation (TA §4.2-2)

**CAP-01 — Operational capacity evidenced.** Presence, staffing, prior actions, named units —
specifics, not adjectives.

**LOC-01 ◆ — Section 10.6 completeness.** Percentage of funding managed by local actors, share of
overheads transferred, and — if incomplete — a dated timeline for the missing information.
"To be determined" without a timeline: HIGH blocker.
*Basis: §4.2-5 requires 10.6 completeness; checkable directly against the form fields.*

**LOC-02 ◆ — Localisation internal consistency.** Declared Grand Bargain compliance vs recorded
amounts (EC budget to local partners, indirect costs transferred). "Yes" beside EUR 0.00
overheads: HIGH.
*Basis: computed from the form — declared compliance vs recorded amounts. Arithmetic, not inference.*

**LOC-03 — Localisation substance.** Share through local/national actors; capacity strengthening
beyond a single partner; risk-transfer mitigation. Thin substance on a large action: MEDIUM, with
the option to argue the ceiling explicitly if the action is analytical.

## CORE C · Methodology and feasibility (TA §4.2-3)

**MET-01 — Intervention logic.** Results chain coherent; outputs vs outcomes distinguished;
activities map to results.

**RESULTS-01 ◆ — Indicator quality and KRI usage.** Compare every result indicator against the
official KRI catalogue embedded in the Single Form; sub-sectors flagged "- KRI" in the form's own
dictionary expect official indicators. Activity counts posing as outcomes: MEDIUM. Custom
indicators are permitted where genuinely needed.
*Basis: compared against the KRI catalogue embedded in the Single Form; mechanical lookup.*

**MET-02 — Risk, access and feasibility.** Country-specific preconditions and risks with matched
mitigations; security/logistics/access addressed; remote-management questionnaire if applicable.

**MET-03 ◇ — Monitoring and evaluation arrangements.** Monitoring framework, disaggregation,
field access; for large multi-year actions, no evaluation/audit/study in 9.4 is a predictable
question: MEDIUM unless justified.
*Basis: inference from worked example 204289 — a large multi-year action with no 9.4 evaluation reads as a predictable desk-officer question. Not stated in any document; capped at MEDIUM/FLAG pending SME sign-off.*

## CORE D · Coordination and post-intervention (TA §4.2-4)

**COORD-01 ◇ — Correct coordination architecture.** The coordination bodies and frameworks named
in the proposal must match the action's actual geography and the bodies the resolved TA names
for it. Bodies belonging to a different sub-region suggest text reuse: MEDIUM (capped pending SME sign-off).
*Basis: the TA names the coordination bodies, but the inference that mismatched bodies imply text reuse is a generalisation from 204289 — this is where the CAPRADE error occurred. Capped at MEDIUM/FLAG pending SME sign-off; verify every named body against the resolved TA before asserting.*

**COORD-02 — Response-plan alignment and national systems.** Relevant plans (HRP/RMRP or
equivalent) named per country; national authorities named; embedding in existing mechanisms
rather than parallel structures.

**COORD-03 ◇ — Text-reuse artifacts.** Narrative content belonging to a different action
(components the action does not have, wrong geography, wrong population). Each instance MEDIUM;
note the pattern if repeated.
*Basis: inference from worked example 204289 (narrative fragments belonging to another action). A generalised pattern, not a documented rule; capped at MEDIUM/FLAG pending SME sign-off.*

**COORD-04 — Sustainability and resilience.** Exit/embedding argument; resilience marker
substantiation; interoperable beneficiary registries where relevant: LOW if relevant and
unaddressed.

**LESSONS-01 — Lessons incorporated (partial in POC).** Internal signals only: predecessor
actions named and built on; un-updated reuse flagged. Direct verification needs L3 (out of
scope); say so.

## CORE E · Transparency, cost-effectiveness and efficiency (TA §4.2-5)

**TRANS-01 ◇ — Cost breakdown documented.** Are the breakdowns in sections 2 and 13.2 complete
and accurate (extent checkable without the financial annex: fields filled, categories used,
narrative explains the structure)? Detailed value-for-money stays out of scope; completeness does
not. Materially incomplete: MEDIUM.
*Basis: §4.2-5 requires a documented cost breakdown, but the completeness judgement here is a generalisation; capped at MEDIUM/FLAG pending SME sign-off.*

**TRANS-02 — Section 10.6 transparency (anchor).** The 10.6 percentage-and-overheads check
formally belongs to this criterion; assessed as LOC-01/LOC-02 under group B — cross-reference,
do not double-count.

**CASH-01 — Cash line completeness.** For any action including cash transfers (modality or
sector): the "in cash" line of 2.4.5 filled with EUR amount and number of targeted
beneficiaries. Missing: HIGH (explicit §4.2-5 check). Where cash is zero, the no-cash
explanation must exist (also a form rule).

**MPCT-01 — TCTR.** For Multi-Purpose Cash Transfer actions: TCTR filled in 2.4.7, methodology
explained (ideally 2.5), and in line with DG ECHO cash policy or justified. Not applicable →
say so.

**CE-01 — Resources-to-results relationship.** Does the intervention display an appropriate
relationship between resources, activities and objectives? Computable signals feed this
judgement: cost per direct beneficiary, share of budget outside the results structure, support
vs delivery ratio. Report the numbers as FLAG-level context; the judgement itself is SME
territory and should stay conservative.

**COFIN-01 ◆ — Co-financing.** Grants must involve co-financing; 100% grant financing is
allowed only where essential and justified in section 10.4. Computable: ECHO amount vs total
funding. 100% without a 10.4 justification: HIGH blocker (and a form rule).
*Basis: form rule plus §4.2-5 — co-financing required, 100% grant only if justified in 10.4. Computed: ECHO vs total funding.*

## CORE F · Compliance with other criteria in the resolved HIP (TA §4.2-6)

**COMP-01 — Risk analysis compliance.** Where applicable, identified risks (security, access,
aid diversion, SEAH, …) analysed with realistic, context-relevant mitigations — assessed as
MET-02 under group C; cross-reference, do not double-count.

**COMP-02 — Continuation actions.** Where the action continues a previous one, note that DG ECHO
may conduct a field visit to assess feasibility of the follow-up; the proposal should make the
continuation link and its lessons explicit (feeds LESSONS-01).

**COMP-03 — Catch-all.** Any further criteria the resolved HIP/TA define beyond the standard six
(check the TA's §4.3 and the HIP's response section); list what was checked.

## CORE G · Deterministic checks (compute, never judge)

**FORM-01 ◆ — Execute the embedded form rules.** Evaluate the executable subset of the export's
own validation rules (mandatory-if, numeric identities, bounds). Any failure will block
submission in APPEL: HIGH, with the form's own error text as the finding.
*Basis: executes the export's own embedded validation rules. The form is the source; the finding text is ECHO's own error message.*

**CONSIST-01 — Cross-field arithmetic.** Sector budgets vs donor request; direct+indirect vs
total cost; funding sources vs total cost (form tolerance €0.01); result amounts vs totals (gap
may be legitimate → FLAG); beneficiary reconciliation across areas, age/gender and category
splits.

**CONSIST-02 ◆ — Target vs disaggregation.** Every indicator target vs the disaggregation in its
comment field — free text, so no form rule catches order-of-magnitude errors here. Magnitude
mismatch: HIGH; otherwise MEDIUM.
*Basis: computed — indicator target vs its free-text disaggregation. Catches order-of-magnitude errors no form rule sees.*

**FORM-02 ◆ — Required references filled.** HIP/Decision reference (1.5) populated; markers
answered; visibility questions answered or justified.
*Basis: mechanical field-population check (1.5 reference, markers, visibility answers).*

**CAP-CHECK ◆ — Character-cap pressure.** Usage vs cap for every section a fix touches; above
~90%, the fix must be a substitution and the review says so per fix.
*Basis: computed — character usage vs the form's own field cap. Pure measurement.*

---

## SECTOR MODULE · Disaster Preparedness
*Applies when routing matched sector "Disaster Risk Reduction / Disaster Preparedness". Basis:
DG ECHO Disaster Preparedness Guidance Note (manifest id DP-NOTE) + the resolved HIP/TA.*

**DP-01 ◆ — Crisis Modifier compliance (Guidance Note Annex 2).** If a CM is present: dedicated
result, preferably last; sub-sector = "Contingency planning and preparedness for response";
activation options, triggers and thresholds stated; target population/area and numerical range;
preparedness measures in place; an indicator measuring time-lapse between trigger and activation
(24/48/72h framing); statement on unused budget; budget proportional (observed average ~10% —
smaller permitted, state the basis). Wrong sub-sector or missing time-lapse indicator: HIGH
blocker.
*Basis: near-transcription of the DG ECHO Disaster Preparedness Guidance Note, Annex 2. Discovery via 204289; the checklist is the Note's.*

**DP-02 — DP thematic coverage.** Check the action against the DP priorities the resolved TA
names (e.g. anticipatory action, early warning, contingency planning, local preparedness
systems); alignment claimed but not evidenced: MEDIUM.

**DP-03 — Mainstreaming vs targeted DP.** Identify whether the action is targeted DP (all
outputs DP) or DP-mainstreamed; apply the Guidance Note's expectations for that type.

## SECTOR MODULES — placeholders (add as the corpus grows)

| Module | Trigger sector | Depends on | Status |
|---|---|---|---|
| Cash & voucher / visibility | any with cash modality | visibility/C&V manual — **not yet in corpus** (VIS-01 gap) | pending |
| Budget eligibility | all | eligibility rules document — **not yet in corpus** (BUDGET-01 gap) | pending |
| EiE, Health, Protection, … | per sector | sector guidance uploads + manifest rows | pending |

---

## ANNEX · §4.2 verbatim — THIS INSTANCE (Technical Annex to ECHO/-AM/BUD/2026/91000, v1)

Per-instance content: on cloning to another region, replace with that region's TA §4.2. If the
resolved TA's wording ever differs from this annex, THE TA WINS and the manifest owner updates
the annex. Embedded so the review backbone never depends on knowledge retrieval.

1) Relevance of the intervention and the coverage — HIP-objective compliance; joint and recent
needs assessments, local partners included in assessment efforts; coordination with humanitarian,
local and national actors.
2) Capacity and expertise (including in support to the localisation approach) — partner and
implementing partners' country/regional/technical expertise; contribution to developing local
capacity.
3) Methodology and feasibility — quality of response strategy incl. intervention logic/logframe,
output & outcome indicators, monitoring, risks and challenges; feasibility incl. security,
logistics, access (incl. remote management); quality of monitoring arrangements.
4) Coordination and relevant post-intervention elements — quality of the localisation approach
and risk-transfer minimisation; building on ongoing local response and coordination (incl., where
relevant, single interoperable beneficiary registries); contribution to resilience and
sustainability incl. locally driven responses.
5) Transparency / Cost-effectiveness and efficiency — cost breakdown sufficiently
documented/explained incl. completeness and accuracy of sections 2 and 13.2; section 10.6 filled
(percentage of funding managed by local actors, share of overheads transferred; if incomplete, a
timing for missing information); for cash actions, the "in cash" line of 2.4.5 with EUR and
beneficiary numbers; for MPCT, TCTR in 2.4.7 with methodology (ideally 2.5) and consistency with
DG ECHO cash policy; appropriate relationship between resources, activities and objectives;
Programmatic Partnerships added value per dedicated guidance; co-financing required — 100% grant
financing only where essential, justified in section 10.4.
6) Compliance with other criteria as defined in the HIP — where applicable, analysis of
identified risks (security, access, aid diversion, SEAH, …) with realistic, context-relevant
mitigations; for continuation actions, DG ECHO may conduct a field visit on feasibility and
quality of the follow-up.

## Known gaps (for SME attention)

- VIS-01 and BUDGET-01 blocked on corpus gaps above.
- LESSONS-01 partial by design (L3 excluded).
- The 204289 worked review predates v0.1.2 and covers criteria 1–4 plus deterministic only;
  groups E and F have no worked example yet — first candidates for the next review run.
- Built against one worked example (regional DP action, LAC 2026). Core criteria are believed
  region-generic; sector coverage beyond DP/Support-to-operations is untested.
- The form-rule catalogue is form-version-specific (eSF 1.1 / FPA 2021); re-derive from each
  export rather than assuming.

---
*Version history: v0.1 initial · v0.1.1 multi-region restructure · v0.1.2 six-criterion alignment, groups E/F added · v0.1.3 HIP/TA attributions corrected (criteria, deadlines, 10.6, duration = TA; DP priorities, SG CAN, EU-LAC MOU, funding scope = HIP). Details in the manifest changelog.*
