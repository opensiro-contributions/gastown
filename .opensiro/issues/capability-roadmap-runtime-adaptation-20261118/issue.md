# Gas Town — optional native S4 future-runtime adaptation (Opensiro roadmap)

**PLAN_ONLY · proposal-stage GO · research NEEDS_EVIDENCE · DRAFT — NOT PUBLISHED**

**One-sentence proposal:** Add an opt-in, town-scoped Deacon patrol wisp that evaluates a dated external agent-runtime compatibility change, tests one authorized future session, and uses its real result to keep or roll back a proposed role-runtime adjustment.

**Canonical decision receipt:** [roadmap.md](roadmap.md) — sole source for the accepted vector, P0/P1/P2, evidence and verdict.
**Technical companion:** [constructor-sufficiency.md](constructor-sufficiency.md) — source-native construction and acceptance.
**Working fork:** `opensiro-contributions/gastown` · **Case:** `.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/` on `opensiro/meta`.

## 1. Why Opensiro and central accepted VSM assessment

Opensiro uses a testable VSM engineering hypothesis: explicit organizational functions, native construction paths and evidence may make agent-harness development more systematic. **Savings, adoption and any superiority over the original design are not established.** This is an optional research proposal, not a deficiency report.

### Central starting point — accepted Index, not the target

> **ACCEPTED HISTORICAL INDEX — not current-HEAD grades or proposed after-states**
>
> **`S1=A · S2=A · S3=A · S3*=A · S4=— · S5=—`**
>
> [Accepted assessment](https://github.com/opensiro/vsm-harness-index/blob/b812936829394d2f1a80fb95915688f20cc1d622/assessments/ga/gastown.md) · Index `b812936829394d2f1a80fb95915688f20cc1d622` · assessment blob `63864bc37d10e192d0ae8a96d1bfd6307bb03a09` · `review_ref=649b832b7672bc7a2dbef26f5983aba6198b819b` · reviewed `2026-09-19` · historical Profile `0.2.3` / Skills procedure `0.3.5`.

**Repository-wide audit:** [Original `main@94cc822`](https://github.com/gastownhall/gastown/commit/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e), observed 2026-11-20; one first-party Gas Town workspace, Mayor, Polecats, Refinery, Witness, Deacon, Beads, rigs, runtime presets, session controls and supported modes. Reviewed repository source inventory (1,565 tracked files), runtime/config/role interfaces, design and tests, MIT license and original Issues/PRs. The human Overseer, external providers and adjacent maintainer/dogfood governance are not automatically in the installed town's functional boundary.

| Function / plain-language role | Historical Index state | Current source-backed owner/closure | Candidate / justified no-target / uncertainty and rank |
| --- | --- | --- | --- |
| **S1 · Operations** — workers doing primary work | A | [Polecats](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/templates/roles/polecat.md.tmpl) execute hooked tasks in isolated worktrees | NO_TARGET: existing autonomous closure |
| **S2 · Coordination** — avoids worker interference | A | Separate Refinery rebase/merge queue sequences changes | NO_TARGET: existing autonomous closure |
| **S3 · Current management** — active commitments | A | [Mayor](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/templates/roles/mayor.md.tmpl) directs current rigs/work, consumes escalations | NO_TARGET: existing autonomous closure |
| **S3* · Independent review** — corrective feedback | A | Refinery verifies landed-candidate work and returns failures to workers | NO_TARGET: existing independent audit |
| **S4 · Future adaptation** — outside/future conditions | — | [Agent preset registry](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/config/agents.go) and [Deacon patrol](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/formula/formulas/mol-deacon-patrol.formula.toml) exist, but no verified prospective autonomous release-to-future-session return loop | P0 hypothetical S4=C path |
| **S5 · Identity/policy** — ultimate legitimate authority | — | Human Overseer decides ultimate policy and provider allowlist | NO_TARGET: parent-governed boundary, intention unverified |

**Interpretation:** `A` = autonomous closed first-party function; `C` = first-party developer-composable autonomous constructor; `P` = supported parent-governed mode; `A(P)` / `C(P)` = independently evidenced additional parent mode; `—` = bounded lack of evidenced material path; `?` = unresolved evidence. These are **ownership categories, not quality ranks** and do not require all functions to be implemented.

**Priority rationale:** Only S4 offers a source-mapped new construction hypothesis at the selected workspace boundary after screening all six functions. A Deacon wisp could reuse current registry, patrol, session and feedback channels; product utility remains hypothetical. S1/S2/S3/S3* already have autonomous ownership and a new S5 authority would cross the Overseer's boundary.

**Deliberate exclusions / methodology challenge:** No source evidence that the lack of a separate S4 is intentional; treat intent as UNVERIFIED. No autonomous S5 delegation or forced provider migration is proposed. If a real first-party prospective loop already exists, re-evaluate the interpretation through the independent Index/Skills route.

**Contributor / maintainer interests (OPTIONAL):** [Original #4402](https://github.com/gastownhall/gastown/issues/4402) seeks unified runtime selection; [#3147](https://github.com/gastownhall/gastown/issues/3147) directs a particular pool strategy toward Gas City. No attributable maintainer endorsement of this S4 proposal: NOT_STATED.

## 2. Selected construction hypothesis and operator outcome

**Target transition:** S4=— -> S4=C

**Function-specific disturbance:** HYPOTHETICAL dated external agent/runtime release or deprecation changes hook/resume/compaction compatibility for a preset currently used by a Gas Town role.

**Proposed C capability (P0):** A developer may opt in to a Deacon future-runtime evaluation wisp, preauthorize a bounded set of agent presets/roles, let the composed agent choose retain / one next-session canary / rollback, and return evidence from that actual subsequent task to Mayor before changing future role mapping.

**Best native operator alternative:** An operator can already select an agent via [config](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/cmd/config.go) and `gt sling --agent`, or manage upgrades manually. Existing [#2784](https://github.com/gastownhall/gastown/issues/2784) concerns current task-based routing, not a confirmed shipped future-release feedback owner.

**Expected user benefit:** HYPOTHETICAL continuity when a supported agent runtime changes. No measured failure reduction, savings, demand or maintainer adoption is asserted.

**Architectural sufficiency argument:** Current `AgentPresetInfo`, Deacon patrol, Beads and `gt sling --agent` provide native observation/action substrates. A small optional, authorized **future-event decision → one later real task → result-fed subsequent decision** bridge would add distinct S4 closure. The indispensable missing integration is the policy-bounded notice/canary/return coupling, not another generic VSM supervisor.

## 3. Existing native work versus missing construction

**Track A — native coverage:** SHIPPED: registry/role config, present-session dispatch, patrol, Witness, Beads/mail; ISSUE_ONLY: [#4402](https://github.com/gastownhall/gastown/issues/4402), [#1143](https://github.com/gastownhall/gastown/issues/1143); historical unmerged PRs: [#3841](https://github.com/gastownhall/gastown/pull/3841), [#4368](https://github.com/gastownhall/gastown/pull/4368); OPEN_PR: [#4981](https://github.com/gastownhall/gastown/pull/4981). Do not credit designs/PRs as shipped.

**Track B — independent on-top C construction:** Add an opt-in future-runtime evaluation step to the Deacon wisp, a dated and authenticated notice receipt, and a guarded future-task trial whose Witness/doctor outcome is returned to the same wisp and Mayor. Reuse the present registry/config/Beads interfaces; never alter running sessions or unauthorized policy.

| C-sufficiency requirement | Already present / proposed in original (A) | What still must be constructed (B) |
| --- | --- | --- |
| External/future signal and autonomous permitted choice | Runtime metadata, present Deacon patrol, allowed role config | Dated source receipt and explicit future-runtime choice within owner allowlist |
| Lawful downstream effect and returned feedback | `gt sling --agent`, Witness outcomes, Beads/mail | One new-session canary + linked result + authorized future role-config keep/rollback |

**Distinctness and falsifier:** If first-party source already closes the same external-change-to-next-task S4 choice and feedback loop, there is no new constructor. A static preset fix, warning dashboard or current task router alone does not complete the claimed S4 function.

## 4. Priorities and minimum sufficient result

- **P0:** Optional complete source-native Deacon future-runtime compatibility decision/canary/return path for proposed S4=C.
- **P1:** Explicit owner allowlist and opt-in; trusted notice; one-session isolation, safe rollback, returned real-task feedback and native negative tests.
- **P2:** Optional release-feed adapters after P0 evidence; no mandatory second function.

**Proposed C-sufficiency verdict:** PROPOSED_C_SUFFICIENT as a falsifiable architecture hypothesis; not shipped, tested or adopted, and not a changed Index grade.

## 5. Proposed acceptance and stop gates

**Future positive test:** With two owner-approved presets and one dated incompatible-release notice, the Deacon wisp chooses one permitted new-session canary; actual worker execution produces Witness/doctor feedback; the result drives an authorized later role mapping decision or rollback.

**Future negative test:** Reject stale/untrusted notice, disallowed preset, revoked owner, concurrent settings change, missing task outcome and active-session mutation; preserve old role config on failure.

**Proposed falsifier:** No lawful autonomous alternative, no actual later task return, an equivalent first-party S4 path already shipped, or an unavoidable violation of the Overseer's boundary.

**Validation state:** NOT_RUN. These are proposed native tests; no executed tests or measured benefit.

## 6. Independent paths

**Original-native contribution:** Prefer existing runtime registry, Deacon and source Issue discussion before proposing a new external design; no original communication authorized.

**Profile / Skills:** Revisit S4 closure methodology only if a real source/recursion counterexample is demonstrated; this Roadmap does not change the general Index.

**Domain fork:** NONE selected; Gas City is a separate original and must not silently substitute for Gas Town.

## 7. Cost hypothesis

Compare manual present role/upgrade management with the proposed future-runtime wisp on the same dated notice and next task, including engineering, verification, rollback, maintenance and review effort. **Cost status: `NOT_MEASURED`**; no cost-reduction result is claimed.

## 8. Decision / handoff

**Proposal-stage decision:** GO

**Research disposition:** NEEDS_EVIDENCE

**Decision reason / next permitted step:** Native architectural S4 construction appears coherent, but future lifecycle signals, bounded authority and returned real-task feedback must be tested before implementation or any original-facing PR. The maintainer alone decides product fit. No implementation or publication is authorized by GO.

**Agent/developer handoff:** [constructor-sufficiency.md](constructor-sufficiency.md) and [canonical roadmap.md](roadmap.md), with the accepted vector and one P0 kept in the receipt.

**Rights and publication:** Original MIT license; other contributor disclosure/formalities require live verification. Fork control was `ACTIVE / ALLOW` for internal metadata at the last source check, not outward consent. This is an unpublished revised Human draft; historical [fork Issue #1](https://github.com/opensiro-contributions/gastown/issues/1) was not updated. Exact current-conversation approval remains necessary for any public fork or external Issue/PR/comment.

**AI disclosure:** Prepared with AI assistance. Native validation, independent human review, economic benefit and product adoption were not performed or established.
