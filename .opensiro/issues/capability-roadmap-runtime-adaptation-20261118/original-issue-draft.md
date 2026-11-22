# Proposal: optional Deacon runtime-compatibility canary and feedback for Gas Town — Opensiro VSM architecture review

## Problem Statement

A Gas Town operator can already configure which agent runtime a role uses, choose an agent for an individual task, and inspect operational health. A *hypothetical* future change—such as a provider announcing that a runtime's resume, hook, or compaction behavior will change—requires the operator to notice the change, decide whether to try a permitted alternative, assess an actual subsequent task, and then keep or revert the selection. A configured runtime catalog and current-task router do not by themselves automate this outside/future signal → lawful alternative → subsequent task → returned evidence cycle.

This is **not** a reported production incident or a claim that Gas Town must become autonomously self-upgrading. If the existing Deacon and role settings already close that specific future-evaluation loop, no new API is justified.

## Proposed Solution

Consider an **opt-in town-scoped Deacon patrol wisp for future agent-runtime compatibility**, constructed by the operator within an explicit allowlist of runtimes, roles and next-session permissions. Given a dated, attributable external runtime compatibility notice, the composed watcher could choose to *retain the current preset*, *prepare one authorized next-session canary*, or *hold/escalate* instead of altering a running session. It would record the choice in Beads, use existing role/runtime selection and `gt sling --agent` for **one new eligible session only**, consume the actual Witness/doctor/worker result, and return an evidence-backed keep/rollback recommendation to the Mayor or operator. A future role mapping change must remain separately authorized by the owner.

The missing first-party construction, *if native composition proves insufficient*, is a minimal guard and linkage between a dated outside compatibility receipt, a policy-scoped decision, a future-session canary, its real task result, and an authorized future configuration update or rollback. Do **not** create a second global agent scheduler, mint provider credentials, silently switch existing running sessions, or replace the Overseer's ultimate permissions.

## Alternatives Considered

- **Existing manual configuration and `gt sling --agent`:** the lowest-cost alternative. An operator can already pick a runtime and decide when to upgrade or roll back; this may be all users need.
- **Static new runtime preset / current-task cost router:** useful but cannot alone show a prospective, independently chosen alternative based on *future external change* and the outcome of the next actual task.
- **Use existing Deacon + Beads + role configuration unchanged:** preferred if a source-grounded integration can implement the complete choice, effect and return without a new first-party port. Such an equivalent path falsifies this proposal.
- **Automatic provider switching in all sessions:** rejected; it would overstep parent policy, increase blast radius and change in-flight work.

## Use Case

HYPOTHETICAL: A dated, official change notice announces altered resume behavior in an allowed CLI agent runtime. A Deacon wisp compares it to the pinned [agent preset metadata](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/config/agents.go), chooses between two **already authorized** runtimes, and schedules a single future Polecat canary. The resulting actual worker execution and Witness/doctor feedback are correlated with that decision. If the permitted candidate fails, no existing session is changed and the old role mapping remains; if it succeeds, the wisp reports evidence for an operator-approved future role mapping adjustment. This is proposed behavior—not a current feature or a measured benefit.

## Additional Context

The seven short sections below explain the source-specific design, accepted historical assessment, limits and research provenance. The existing first-party provider template headings above are retained; the extra material is methodological context, not a requirement that Gas Town adopt VSM.

### Proposal in the project's own terms

**What exists today:** [Agent presets and hooks](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/config/agents.go), [role configuration](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/config/loader.go), [CLI configuration](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/cmd/config.go), [Deacon patrol formula](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/formula/formulas/mol-deacon-patrol.formula.toml), and native Beads/mail and Witness result paths handle current choices, operational monitoring and returns.

**What may be missing:** A developer-composable, first-party link from a **dated external future compatibility signal** to an independently selected, owner-authorized *next-session* trial and its observed task outcome, followed by a revision of future choices.

**Closest existing project-native solution:** Use current presets, Deacon patrol, manual `gt upgrade`, and `gt sling --agent`; consider a small wisp-based composition before adding first-party configuration/decision plumbing.

**Existing discussion:** [Original Issue #4402](https://github.com/gastownhall/gastown/issues/4402) (OPEN) concerns first-class agent/runtime selection; [#2784](https://github.com/gastownhall/gastown/issues/2784) (CLOSED) concerns current task-based routing; [#1143](https://github.com/gastownhall/gastown/issues/1143) (OPEN) concerns long-term execution costs. [PRs #3841](https://github.com/gastownhall/gastown/pull/3841) and [#4368](https://github.com/gastownhall/gastown/pull/4368) were closed unmerged; [#4981](https://github.com/gastownhall/gastown/pull/4981) remains open. These are relevant native alternatives but do not establish the proposed external-notice-to-subsequent-task loop as shipped. If #4402 is the preferred home for discussion, please consolidate rather than duplicate ongoing design decisions.

### How we reached this proposal — Opensiro VSM assessment

Opensiro uses Stafford Beer's Viable System Model (VSM) as a **reviewable engineering hypothesis** about organizational decisions and feedback owners, not as an agent maturity, safety or quality score.

**Historical assessment:** [Accepted Opensiro Index assessment](https://github.com/opensiro/vsm-harness-index/blob/b812936829394d2f1a80fb95915688f20cc1d622/assessments/ga/gastown.md), immutable Index commit `b812936829394d2f1a80fb95915688f20cc1d622`, assessment blob `63864bc37d10e192d0ae8a96d1bfd6307bb03a09`, original review ref `649b832b7672bc7a2dbef26f5983aba6198b819b`, reviewed 2026-09-19; historical Profile `0.2.3` and Skills methodology `0.3.5`. These grades are dated and are **not a regrade of the current code**.

**Boundary:** One first-party Gas Town installation including Polecats, Refinery, Mayor, Witness, Deacon, sessions, Beads and role configurations. The Overseer/operator, external runtime providers, their credentials and human maintainer organization remain outside the selected autonomous policy boundary.

**Current original HEAD:** [`gastownhall/gastown@94cc82289d2ead275a62e1db4ef1d4ada4a1f98e`](https://github.com/gastownhall/gastown/commit/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e), source-checked independently on 2026-11-22, separate from the frozen Index evidence.

| Function / plain-language role | Native ownership example | Historical state | Source-backed present boundary / limitation |
| --- | --- | --- | --- |
| **S1 · Operations** | Polecats execute primary work | A | Hooked tasks run in isolated [worktrees](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/templates/roles/polecat.md.tmpl) |
| **S2 · Coordination** | Refinery reconciles concurrent changes | A | Merge/rebase sequencing already coordinates current worker interference |
| **S3 · Current management** | Mayor directs active commitments | A | [Mayor](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/templates/roles/mayor.md.tmpl) handles present task priorities/escalations |
| **S3* · Independent audit** | Refinery separately checks candidate work | A | Verification is already part of existing return/correction routes |
| **S4 · Future adaptation** | Deacon patrol and preset registry | — | No verified first-party prospective outside-signal → choice → next-session effect → real returned feedback loop |
| **S5 · Identity and policy** | Human Overseer holds ultimate authority | — | A local autonomous provider-policy authority is not evidenced and is **not requested** |

The Skills states denote function ownership/constructibility, not quality ranks: `A` = first-party autonomous closure; `C` = first-party developer-composable function-specific construction; `P` = supported parent-governed closure for S3–S5; `A(P)` and `C(P)` = separately evidenced accompanying parent modes; `—` = no material function path evidenced at the reviewed boundary; `?` = insufficient evidence. No requirement to implement all six functions follows.

### Why this particular construction?

**Whole-repository prioritization:** Historical S1/S2/S3/S3* are already `A`; this case proposes *only* a distinct optional prospective S4 constructor. S5 permissions remain with the operator. This is not a new universal controller or a mandatory autonomous upgrade.

**Construction hypothesis:** Historical `S4=— -> S4=C` **only if** a composed future-focused watcher can choose among lawful alternatives from external evidence, produce a real later operational effect and receive its outcome for the next decision. The proposal-stage decision is `GO / NEEDS_EVIDENCE`; neither code nor the accepted Index have changed.

**Native building blocks:** Existing first-party `AgentPresetInfo`, Deacon patrol formula, Beads/mail, `gt sling --agent`, Witness/doctor returns, role configuration and the Mayor's escalation path.

**Minimal proposed addition:** An *opt-in* bounded Deacon wisp, typed/attributable notice and decision receipts, one authorized future-session canary and correlated returned feedback; implement any necessary small first-party glue only if the native composition baseline cannot do this safely.

**Scope exclusions:** No secret/credential provisioning, unattended provider preference changes, dynamic S5 policy grant, global scheduler, automatic rollout, mutation of in-flight sessions or assumption of maintainer endorsement. Supported design intent for an S4 omission is NOT_STATED.

### Proposed approach and validation

1. Construct a test baseline using manual preset selection plus unchanged Deacon/Beads/mail paths, with one synthetic **dated external compatibility notice** and two operator-allowed runtime choices.
2. Compare an opt-in Deacon wisp with that baseline. Check that one valid alternative is selected, only one **new** Polecat session uses the approved canary, and actual Witness/doctor/task return is correlated to a later retain/rollback decision.
3. Negative controls: untrusted/stale notice, revoked operator, forbidden preset, missing or forged task outcome, concurrent config drift, disallowed running-session change, duplicate event and failure to roll back. Disabled-option deployments should behave exactly as before.

**Hypothesized benefit:** Fewer manual future-runtime compatibility decisions and more source-linked evidence for a later authorized role change. Actual effectiveness, user demand, correctness and performance are **NOT_MEASURED**.

**How to falsify:** If a shipped first-party native composition already supplies the complete future-outside-event → lawful choice → future-task effect → outcome-return loop, or the proposed scoped session cannot safely apply or report its effect, there is no justified new S4=C port. A simpler native fix is preferable where sufficient.

**Cost status:** NOT_MEASURED; proposed tests NOT_RUN. Cost reduction remains a hypothesis until matched implementation, review, integration, test and maintenance costs can be observed.

### Feedback requested

Would a narrowly opt-in Deacon compatibility watcher be useful for an owner-authorized **future-session canary**, or can current Deacon, config and Beads capabilities already support the same safe decision/return loop? Should this be discussed under [#4402](https://github.com/gastownhall/gastown/issues/4402) rather than a new feature Issue? Corrections on first-party boundaries and intentional parent ownership are welcome. Maintainers own adoption or rejection.

### Three independent ways to participate

- **Improve Gas Town natively:** use/extend the existing Deacon and runtime configuration paths only if maintainers consider a new native integration worthwhile.
- **Challenge Opensiro's interpretation:** review the source-backed S4 ownership claim in [Profile](https://github.com/opensiro/vsm-harness-profile) / [Skills](https://github.com/opensiro/vsm-harness-skills) without presuming the historical Index is today's truth.
- **Test an optional domain fork:** compare a permitted prototype against manual configuration without imposing a new dependency on Gas Town.

### Research attribution and AI disclosure

[Opensiro Upstream](https://github.com/opensiro/upstream) · [same-case Gas Town Roadmap receipt](https://github.com/opensiro-contributions/gastown/blob/c0122a222b98449f68b0ebef9882417489d546b4/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/roadmap.md) · [accepted historical Index assessment](https://github.com/opensiro/vsm-harness-index/blob/b812936829394d2f1a80fb95915688f20cc1d622/assessments/ga/gastown.md).

**AI involvement:** An AI assistant reviewed public first-party source, existing Issues/PRs and the frozen Opensiro assessment, and drafted this optional design proposal. There is no product implementation, executed native test, measured benefit, current Index grade change or Gas Town maintainer endorsement.
