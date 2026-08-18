# ECHO Pre-Submission Review Rubric — CORE v0.1.5 (DRAFT, pending SME validation)

DRAFT for GO Brussels SME review — nothing here is authoritative until initialled. The label
v0.2 is reserved for the version that returns from that review.

## What changed in v0.1.5, and why

Business feedback on the sample review (2026-08-11): too much of it was deterministic validation —
totals, character limits — and too little substantive engagement with the narrative, in particular
whether the proposal argues its case against the needs assessment and against horizontal guidance.

That was a structural problem, not a weighting one. v0.1.4 had five fully-specified deterministic
criteria, each cheap to compute and each firing on every proposal, against narrative criteria of a
single line apiece. The imbalance had a cause the rubric itself recorded: its module table listed
horizontal guidance as "not yet in corpus". With four universal documents there was nothing to
ground a horizontal criterion in, so the criteria that *could* be grounded crowded out the ones
that could not.

The knowledge base now holds 19 universal and 25 conditional references, each carrying verbatim
anchor quotes with page references. Four consequences:

1. **The deterministic group moves to Annex 1.** Every check still runs and still blocks — a
   FORM-01 failure stops submission in APPEL and stays in the verdict. It is reported as a results
   table rather than as findings competing for attention with judgement. `CAP-CHECK` stops being a
   finding at all and becomes what it always was: a constraint on how a fix is written.
2. **Needs assessment becomes a group (NEEDS-01…05), not one line.** It is the business's named
   priority and the Technical Annex asks three distinct questions about it.
3. **New CORE H · Horizontal guidance compliance**, each criterion naming the manifest `ref_id`
   that grounds it.
4. **Those criteria are ◆, not ◇.** They cite loaded documents, so the MEDIUM/FLAG cap that applies
   to generalisations from the worked example does not apply to them. Substantive narrative findings
   can carry real weight — which was the actual ask.

**The guard against overcorrecting.** "More substantive" must not become "more opinion". Every
CORE H and NEEDS finding cites a loaded document by manifest `ref_id`, page and anchor quote — the
same discipline the corpus build enforces on itself. A narrative criterion that cannot cite a
document is reported as "not assessable against loaded documents", exactly as before.

## Provenance marks

Criteria surfaced through a worked example (proposal 204289, LAC 2026) rather than derived from the
framework directly carry a provenance mark and a *Basis:* line stating what grounds them, so the SME
can see which criteria are ECHO's own words and which are generalisations awaiting validation:
- ◆ document- or mechanically-grounded — the requirement is verbatim in the resolved HIP/TA, verbatim
  in a manifest-registered reference, or computed from the form. Only failure mode is a wrong
  citation or a false arithmetic flag, both checkable in seconds; full severity range applies.
- ◇ inference-grounded — a generalisation drawn from one proposal, not yet in any document. This
  is the class that can hallucinate (the CAPRADE error was here); capped at MEDIUM/FLAG until SME
  sign-off — allowed to raise a question, never to declare a blocker.
Both marks share one property: never passed human review, and so deserve the hardest SME scrutiny.

## Using a reference as a basis

`load_class` in the manifest governs what a document may do:
- `binding` — may ground a finding at any severity.
- `background` — informs and gives context, but is **never the sole basis for a finding**. Several
  are addressed to Member States or EU institutions rather than to partners; a finding that treats
  one as an obligation on an IOM country office is wrong.
- `reference_tool` — an instrument. Use it to test whether a proposal would satisfy the instrument,
  not as a source of prose obligations.

Cite `[R]` bullets for "requirement not met". `[G]` supports "recommended practice not followed",
which is MEDIUM at most. `[D]` is the distiller's reading and never grounds a finding on its own.

Structure: **Core** applies to every proposal. **Sector modules** apply only when routing matched
that sector. The rubric states WHAT to check; the resolved HIP/TA supplies the answer (deadlines,
amounts, named bodies). A criterion that cannot be assessed because the resolved documents are
silent is reported as "not assessable against loaded documents", never guessed.

Severity: blocker = explicit requirement not met · HIGH = will draw a desk-officer question or is
time-critical · MEDIUM = weakens the proposal · LOW = improvement · FLAG = may be legitimate,
needs a human.

**Silence is not automatically non-compliance.** Where a proposal says nothing at all about a
horizontal theme, the finding is MEDIUM with the gap named and the Single Form section that was
checked stated — never a blocker on silence alone. Whether silence means non-compliance or genuine
non-applicability needs country knowledge the reviewer does not have, and that limitation belongs in
"what this review could not assess".

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

**REL-04 → superseded by the NEEDS group below.** Retained as an ID so earlier reviews remain
comparable; do not use it for new findings.

### CORE A/NEEDS · Needs assessment basis (TA §4.2-1, expanded)

The Technical Annex asks three distinct questions about needs assessment, not one. v0.1.4
compressed them into a single line, which is why reviews said little about the substance the
business most wants examined. Each criterion below is ◆ — grounded in the TA's own wording.

*Group basis: the resolved Technical Annex §4.2-1 asks, verbatim: "Has a joint needs assessment
been used for the proposed intervention? Have other recent and comprehensive needs assessments been
used? How have the local partners been included in the needs assessment efforts?" Quote the resolved
TA for THIS proposal; the wording above is from the -AM 2026 TA and must be re-read per region.*

**NEEDS-01 ◆ — An assessment is named, dated and attributable.** Is a specific needs assessment
identified — who conducted it, when, covering which geography and population? A proposal that
refers to "recent assessments" without naming one cannot be verified by a desk officer. Unnamed or
undated: MEDIUM. No assessment referenced anywhere in the needs sections: HIGH.

**NEEDS-02 ◆ — Joint versus single-agency.** The TA asks specifically whether a *joint* assessment
was used. Where the assessment is single-agency, does the proposal say so and explain why — or does
it reference the inter-agency assessment for that crisis (HNO, MSNA, RMRP or equivalent) and
position itself against it? Single-agency without acknowledgement: MEDIUM.

**NEEDS-03 ◆ — The stated needs actually follow from the assessment.** This is the substantive
check and the one most often skipped. Do the needs asserted in the narrative trace to the assessment
cited, or does the proposal cite an assessment and then describe needs it does not evidence? Look
for: needs figures with no source; a caseload that does not follow from the assessment's findings;
severity claims stronger than the assessment supports. Assessment cited but not used: MEDIUM,
rising to HIGH where the targeting or budget rests on the unevidenced figure.

**NEEDS-04 ◆ — Disaggregation supports the targeting claimed.** Does the assessment evidence
support the age, sex and disability breakdown the proposal targets, or is the disaggregation
asserted independently of it? Where the action claims to prioritise a specific group, is that
group's need evidenced rather than assumed? Targeting unsupported by the assessment: MEDIUM.
*Cross-reference: consistency of the numbers themselves is CONSIST-02 in Annex 1 — this criterion
is about whether the evidence supports them, not whether they add up.*

**NEEDS-05 ◆ — Local partners included in the assessment effort.** The TA asks this directly, and
it is the criterion most likely to be answered with a generic sentence. Does the proposal say
specifically how local and national actors participated — in design, data collection, analysis, or
validation — or does it assert inclusion without describing it? Generic assertion: MEDIUM.
*Cross-reference: LOC-03 covers localisation in delivery; this one is about the assessment phase.*

**NEEDS-06 ◇ — Affected people consulted.** Whether the assessment reflects consultation with
affected people, and whether their stated priorities appear in the intervention logic.
*Basis: not stated in the resolved TA §4.2-1; drawn from AAP expectations in the universal corpus
(`the-inclusion-of-persons-with-disabilities-in-eu-funded`, `guidance-note-on-the-protection-from-sexual-exploitation`)
which address participation but not needs assessment specifically. Capped at MEDIUM/FLAG pending SME
sign-off.*

**Known limitation of this group, for SME attention.** The corpus contains no partner-facing needs
assessment requirements document. The one universal needs-assessment reference
(`needs-assessment-european-civil-protection-and-humanitarian`) is `background`: it describes the
Commission's own allocation process and its distillation records "None identified" for partner
expectations. So NEEDS-01…05 ground in the resolved TA and sector guidance, not in a dedicated
methodology document. If DG ECHO publishes partner-facing needs assessment guidance, adding it would
strengthen this group materially — this is a documented corpus gap, not an oversight.

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

## CORE H · Horizontal guidance compliance

Applies to EVERY proposal — these documents are `applicability: universal` in the manifest, so they
route regardless of sector. Each criterion names the reference that grounds it; a finding here must
cite that reference by `ref_id`, page and anchor quote. Where the proposal is simply silent on a
theme, see the silence rule in the header: MEDIUM with the section checked named, never a blocker.

**GAM-01 ◆ — Gender-Age Marker substantiation.** The marker has four assessment criteria and a
scoring scale, and the toolkit maps each criterion to the Single Form sections it is assessed
against. Does the proposal contain the evidence its claimed GAM score requires — gender/age
analysis, adapted assistance, participation, and disaggregated monitoring — in the sections the
toolkit names? A claimed score the narrative cannot support is the characteristic failure.
*Basis: `gender-age-marker-toolkit` (reference_tool, universal). Marker instrument: test whether the
proposal satisfies the instrument, do not treat the toolkit as prose obligation.*

**GEN-01 ◆ — Gender analysis and adapted assistance.** Are gender-differentiated needs analysed
rather than asserted, and does the response differ accordingly? Generic "women and girls will be
prioritised" without analysis or differentiated activity: MEDIUM.
*Basis: `dg-echo-thematic-policy-document-n-6-gender-different-needs` (binding, universal). Note its
2013 date and the currency questions recorded in that reference's Uncertainty section.*

**DIS-01 ◆ — Disability inclusion: twin-track and barrier analysis.** Does the proposal show both
mainstreamed accessibility and targeted action where needed, and is there a barrier analysis rather
than a statement of intent? Where data collection is described, is the Washington Group Short Set
used or its absence explained?
*Basis: `the-inclusion-of-persons-with-disabilities-in-eu-funded` (binding, universal).*

**DIS-02 ◆ — Disability inclusion reflected in the right Single Form sections.** DG ECHO publishes
a direct mapping of disability-inclusion expectations to specific Single Form sections. Check the
named sections rather than searching the narrative generally, and report which sections were checked.
*Basis: `tips-on-how-to-reflect-mainstreaming-of-disability` (binding, universal) — its whole value
is the section mapping.*

**PSEA-01 ◆ — PSEAH expectations towards partners.** Does the proposal evidence the PSEAH measures
the guidance note expects — policy, reporting channels accessible to affected people, investigation
arrangements, staff obligations — or does it name PSEAH without substance?
*Basis: `guidance-note-on-the-protection-from-sexual-exploitation` (binding, universal).*

**PM-01 ◆ — Protection Mainstreaming KOI.** DG ECHO's guidance states a recommendation covering all
actions providing direct assistance; check the reference for its exact modal force before asserting
a requirement. Where the PM KOI applies: is it included, with the mandatory survey questions,
disaggregation bands and monitoring arrangements the guidance and toolkit define?
*Basis: `dg-echo-protection-mainstreaming-key-outcome-indicator-and` (binding, universal) for the
rules; `dg-echo-protection-mainstreaming-key-outcome-indicator-pm` (reference_tool) for the eight
mandatory questions and calculation.*

**ENV-01 ◆ — Minimum Environmental Requirements.** The MERS guidance states requirements a proposal
must meet, including a project-level environmental screening for defined cases, and it is organised
by sector. Apply the requirements for the proposal's sectors — never generalise a sector-specific
requirement across sectors.
*Basis: `guidance-on-the-operationalisation-of-the-minimum` (binding). Registered conditional across
nine sectors, so in practice it routes to almost every action; confirm it routed before citing it.*

**RESIL-01 ◆ — Resilience marker substantiation.** The marker has four scoring criteria and a
criteria-to-Single-Form-section mapping. Does the proposal's resilience-marker claim have evidence
in the sections the guidance names?
*Basis: `resilience-marker-general-guidelines-2022` (reference_tool, universal).
Cross-reference: COORD-04 covers the resilience argument narratively; this one tests the marker claim.*

**KRI-01 ◆ — Single Form 7.3 indicator selection rules.** Compulsory KRIs marked with an asterisk
must be used where the sub-sector requires them; custom indicators only where the rules permit.
*Basis: `changes-in-single-form-chapter-7-3-selecting-key-result` (binding, universal, Nov 2025).
Overlaps RESULTS-01, which compares against the KRI catalogue embedded in the form — RESULTS-01 is
the mechanical lookup, KRI-01 is compliance with the selection rules. Do not double-count.*

**DIV-01 ◆ — Aid diversion reporting awareness.** Where the operating context carries diversion
risk, does the proposal's risk analysis engage with it, given the quarterly monitoring and aid
diversion reporting partners are subject to?
*Basis: `echo-quarterly-monitoring-and-aid-diversion-reporting-annex` (reference_tool, universal).
That reference's Uncertainty section records the evidence that this template is donor-wide rather
than Syria-specific; read it before relying on this criterion.*

**HORIZ-99 — Horizontal themes the resolved HIP/TA names.** The resolved documents may require
horizontal themes beyond this list (nature-based solutions, DRR mainstreaming, climate integration,
digitalisation). Check whichever the resolved HIP/TA require and report what was checked.
*Cross-reference: REL-06 covers the same ground from the relevance side — assess once, cite once.*

**Background-class documents do not appear as criteria here.** Ten universal and conditional
references are `load_class: background` — Commission communications, Council conclusions, staff
working documents. Several are addressed to Member States or EU institutions rather than to
partners. They inform interpretation and may be cited alongside a binding basis, but no CORE H
criterion rests on one, and a finding must never present one as an obligation on a country office.

---

## SECTOR MODULE · Disaster Preparedness
*Applies when routing matched sector "Disaster Risk Reduction / Disaster Preparedness". Basis:
`dg-echo-guidance-note-disaster-preparedness-thematic-policy` (binding, conditional →
`disaster_preparedness`) + the resolved HIP/TA.*

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

## SECTOR MODULES — now grounded (v2 corpus)

v0.1.4 listed these as "not yet in corpus". They are now registered, so a module for each sector
can be derived from its reference's **Assessment questions** section, which is already
reviewer-facing and anchored to page references. Written modules follow the DP pattern above; until
each is written out and SME-reviewed, apply the reference's own Assessment questions directly and
mark findings ◆ with the `ref_id` cited.

| Trigger | Grounding reference(s) — manifest `ref_id` | load_class |
|---|---|---|
| sector `health` | `health-response-in-humanitarian-settings-dg-echo-policy`; `annex-5-technical-guidelines-annex-to-dg-echo-health-policy`; `list-of-kris-key-result-indicators-for-health` | binding |
| sector `wash` | `dg-echo-thematic-policy-document-n-2-water-sanitation-and`; `single-form-wash-indicators-guidance` | binding |
| sector `nutrition` | `dg-echo-thematic-policy-document-n-4-nutrition-addressing`; `infant-and-young-children-feeding-in-emergencies-guidance`; `addressing-undernutrition-in-emergencies-a-roadmap-for` | binding |
| sector `protection` | `dg-echo-thematic-policy-document-n-8-humanitarian`; `dg-echo-protection-key-outcome-indicator-pkoi-technical` | binding |
| sector `shelter` / `cccm` | `dg-echo-thematic-policy-document-n-9-humanitarian-shelter`; `humanitarian-shelter-and-settlements-guidelines-annex-7-1` | binding |
| sector `food_security` | `humanitarian-food-and-livelihood-assistance-hfla-dg-echo` | binding |
| sector `education` | `technical-guidance-on-the-use-of-the-revised-dg-echo` | binding |
| sector `logistics` | `dg-echo-humanitarian-logistics-policy-operational-guidance` | binding |
| modality `cash` / `voucher` | `dg-echo-thematic-policy-document-no-3-cash-transfers`; `10-common-principles-for-multi-purpose-cash-based` | binding |
| modality `in_kind`, sectors `health`/`food_security` | `provisions-on-medical-and-food-supplies-applicable-to` | binding |
| condition `programmatic_partnership` | `guidance-to-dg-echo-partners-programmatic-partnerships-2024` | binding |

**Gaps that remain open.** The visibility / communication rules document (VIS-01) and the budget
eligibility rules document (BUDGET-01) are still **not in the corpus** — neither appears in the
GO-reviewed catalogue. Those two criteria therefore still cannot be grounded, and a review must say
so rather than improvising. This is the same class of gap the v0.1.4 table recorded; it has narrowed,
not closed.

---

## ANNEX 1 · Deterministic results (compute, never judge)

*Formerly CORE G. Moved here in v0.1.5 following business feedback that the sample review carried
too much deterministic validation relative to narrative substance. Nothing is removed: every check
still runs on every proposal, and a FORM-01 failure still blocks submission. What changed is
presentation — these are reported as a results table after the findings, not as findings competing
with judgement for the reader's attention. Blockers are still surfaced in the summary verdict,
because a submission that APPEL will reject is the most actionable thing a review can say.*

**FORM-01 ◆ — Execute the embedded form rules.** Evaluate the executable subset of the export's
own validation rules (mandatory-if, numeric identities, bounds). Any failure will block
submission in APPEL: HIGH, with the form's own error text as the finding. **Surfaced in the verdict
even though reported in this annex.**
*Basis: executes the export's own embedded validation rules. The form is the source; the finding text is ECHO's own error message.*

**CONSIST-01 — Cross-field arithmetic.** Sector budgets vs donor request; direct+indirect vs
total cost; funding sources vs total cost (form tolerance €0.01); result amounts vs totals (gap
may be legitimate → FLAG); beneficiary reconciliation across areas, age/gender and category
splits.

**CONSIST-02 ◆ — Target vs disaggregation.** Every indicator target vs the disaggregation in its
comment field — free text, so no form rule catches order-of-magnitude errors here. Magnitude
mismatch: HIGH; otherwise MEDIUM.
*Basis: computed — indicator target vs its free-text disaggregation. Catches order-of-magnitude errors no form rule sees.
Cross-reference: NEEDS-04 asks whether the evidence supports these numbers; this asks whether they reconcile.*

**FORM-02 ◆ — Required references filled.** HIP/Decision reference (1.5) populated; markers
answered; visibility questions answered or justified.
*Basis: mechanical field-population check (1.5 reference, markers, visibility answers).*

**CAP-CHECK ◆ — Character-cap pressure. Not a finding.** Usage vs cap for every section a fix
touches; above ~90% the fix must be a substitution and the review says so per fix. In v0.1.5 this
stops being reported as a finding at all: it is a **constraint on how fixes are written**, reported
once in the character-cap constraint block, not as an observation about the proposal.
*Basis: computed — character usage vs the form's own field cap. Pure measurement.*

---

## ANNEX 2 · §4.2 verbatim — THIS INSTANCE (Technical Annex to ECHO/-AM/BUD/2026/91000, v1)

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

**Corpus gaps — a criterion cannot be grounded**
- VIS-01 (visibility / communication rules) and BUDGET-01 (budget eligibility rules): neither
  document appears in the GO-reviewed catalogue. Still ungroundable; a review must say so.
- No partner-facing **needs assessment methodology** document exists in the corpus. The NEEDS group
  therefore grounds in the resolved TA §4.2-1 and sector guidance. Since needs assessment is the
  business's named priority, adding such a document — if DG ECHO publishes one — would strengthen
  the group more than any rubric edit could.
- L3 (donor feedback, rejection letters, past reports) remains out of scope; LESSONS-01 is partial
  by design.

**Validation status of the new material (v0.1.5)**
- The NEEDS group and CORE H have **never been run against a real proposal**. They are derived from
  the resolved TA's own wording and from the universal references' Assessment questions, but the
  severity calibration is untested — the risk is over-firing at MEDIUM on proposals that are
  substantively fine. The 204289 re-run is the first test.
- CORE H criteria are marked ◆ because they cite loaded documents. That raises their permitted
  severity above the ◇ cap. SMEs should check that the raise is warranted criterion by criterion,
  particularly GAM-01, RESIL-01 and DIV-01, where the basis is a *reference tool* rather than prose
  requirements and the inference from "the instrument expects X" to "the proposal must show X"
  is the reviewer's, not the document's.
- Sector modules beyond DP are listed as grounded but **not written out**. Applying a reference's
  Assessment questions directly is a reasonable interim, but those questions were written by
  distillation agents against one document each, and have not been reconciled across overlapping
  documents (e.g. HFLA 2025 vs Nutrition 2013 both cover nutrition, with different dates and
  possibly different expectations).

**Currency conflicts the corpus surfaced, unresolved**
- WASH: SWD 2012 (background) vs Thematic Policy n°2 2014 (binding) vs Single Form WASH indicators
  2025 (binding). No document states precedence.
- Nutrition: Thematic Policy n°4 2013 vs HFLA Policy Guidelines 2025. No supersession statement.
- Logistics: Thematic Policy 2022 (background) vs Operational Guidance for Partners 2023 (binding).
- Where two loaded documents conflict, the review reports the conflict rather than picking a winner.

**Other**
- Built against one worked example (regional DP action, LAC 2026). Core criteria are believed
  region-generic; sector coverage beyond DP/Support-to-operations is untested.
- The form-rule catalogue is form-version-specific (eSF 1.1 / FPA 2021); re-derive from each
  export rather than assuming.

---
*Version history: v0.1 initial · v0.1.1 multi-region restructure · v0.1.2 six-criterion alignment, groups E/F added · v0.1.3 HIP/TA attributions corrected (criteria, deadlines, 10.6, duration = TA; DP priorities, SG CAN, EU-LAC MOU, funding scope = HIP) · v0.1.4 basis lines added, inference-grounded criteria severity-capped · v0.1.5 business-feedback rebalance: deterministic group → Annex 1, REL-04 → NEEDS group, CORE H added, sector modules grounded against the v2 corpus. Details in the manifest changelog.*
