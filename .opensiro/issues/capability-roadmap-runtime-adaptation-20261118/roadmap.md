# Gas Town — Wave 4 v0.18.1 independent source-native Roadmap (PLAN_ONLY)

## Identity and pins
- Original repository: gastownhall/gastown
- Original HEAD: 94cc82289d2ead275a62e1db4ef1d4ada4a1f98e
- Observed at: 2026-11-20
- Accepted Index assessment: https://github.com/opensiro/vsm-harness-index/blob/b812936829394d2f1a80fb95915688f20cc1d622/assessments/ga/gastown.md
- Accepted assessment blob SHA: 63864bc37d10e192d0ae8a96d1bfd6307bb03a09
- Accepted review ref: 649b832b7672bc7a2dbef26f5983aba6198b819b
- Accepted reviewed at: 2026-09-19
- Profile / Skills procedure: 0.2.3 / 0.3.5
- System in focus: one first-party Gas Town installation, its Mayor, Polecats, Refinery, Witness, Deacon, rig/session runtime, native Beads/convoy/mail/hook/config and patrol paths; the Overseer and external providers are outside its ultimate-policy boundary
- Receipt contract: proposal-gate
- Repository-wide source map: pinned README, LICENSE, CONTRIBUTING, Go cmd/config/agent/runtime/daemon/witness/refinery/deacon/patrol paths, Beads/rig/role hooks, tests and design docs, native original Issues #4402/#2784/#1143/#3147 and PRs #3841/#4368/#4981; 1,565 tracked original files inspected by source tree census
- Accepted VSM vector: S1=A · S2=A · S3=A · S3*=A · S4=— · S5=—
- Target transition: S4=— -> S4=C
- Priority rationale: S1/S2/S3/S3* already have first-party A owners and no independent C need; S5 is parent/Overseer authority; a narrowly prospective S4 role-runtime compatibility transition is constructible by connecting Gas Town-native Deacon patrol wisp, AgentPresetInfo, future-session dispatch, feedback and scoped role config, without a generic supervisory layer
- S1 disposition: ALREADY_A / NO_TARGET — Polecats act on hooked work in isolated rig worktrees and return gt done results
- S2 disposition: ALREADY_A / NO_TARGET — Refinery serializes rebase/merge conflict and dependency interference
- S3 disposition: ALREADY_A / NO_TARGET — Mayor directs present cross-rig commitments and consumes Witness/Deacon/escalation feedback
- S3* disposition: ALREADY_A / NO_TARGET — separate Refinery verifies post-rebase changes before landing and returns failures
- S4 disposition: HISTORICAL_ABSENCE / P0_C_CONSTRUCTOR — no shipped complete outside/future release-compatibility choice, authorized future session effect and returned operational evidence; proposed opt-in Deacon future-runtime wisp fills this specific chain
- S5 disposition: PARENT_SCOPE / NO_TARGET — Overseer chooses ultimate purpose, legal/provider allowance and publication; no autonomous constitutional decision inferred
- P1 dependencies: add explicit allowed agent/role scope and deterministic no-op/rollback behavior, authenticated or human-injected dated future-release receipt, one-session canary isolation and explicit negative authority tests
- P2 optional: later read-only release feed adapters and comparative repeated-task statistics; no new central control plane or mandatory provider integration
- Proposed C construction: Within Overseer-configured permitted runtimes, a new optional Deacon patrol wisp examines a dated external provider/runtime deprecation or lifecycle notice against native AgentPresetInfo hooks/compaction/resume/process metadata and town/rig role settings; independently chooses retain, scoped canary or rollback; records choice in a Beads wisp; triggers exactly one authorized next-session canary via existing gt sling --agent (not an in-flight replacement); consumes next-operation Witness/doctor/Refinery return, then adjusts only authorized future role-agent config or reverts and reports to Mayor through native Beads/mail; repeats upon later source change
- C sufficiency falsifier: if independent outside/future evaluation cannot choose between two permitted responses, cannot lawfully change a subsequent Gas Town operation or read its actual result, or an equivalent complete native S4 loop is already shipped, this proposed S4 C chain fails; lack of measured product benefit is NOT a constructor veto
- Scenario basis: HYPOTHETICAL
- Proposal-stage decision: GO
- Research disposition: NEEDS_EVIDENCE
- Proposed validation: native Go config/role resolution tests plus opt-in Deacon wisp simulation using a dated externally supplied runtime-compatibility signal; positively require a scoped alternative selected and a real later gt sling test task with Witness/doctor feedback and persisted rollback/commit; negatively require deny on unapproved preset, stale/untrusted signal, revoked owner, missing integration test result and in-flight session; disabled baseline unchanged
- Validation state: NOT_RUN
- Proposal falsifier: first-party code already implements prospective outside/future receipt -> autonomous policy-bounded decision -> enforceable next-session change -> actual return, or the proposed native Deacon path cannot be safely completed without assuming unrestricted host/provider/human authority

## Rights and authority
- Original: MIT LICENSE; repo public, unarchived. Clauses for any external CLA/DCO or AI disclosure not independently established; no external Issue/PR/comment or fork public Issue modification is authorized.
- Matching verified fork: opensiro-contributions/gastown, opensiro/meta. Latest metadata read before proposal: ACTIVE / ALLOW, original_repository matches gastownhall/gastown; recheck before any commit. User activation #58 does NOT permit third-party publication or native implementation.
- New proposal is architectural constructibility only; maintainers own product adoption. Accepted Index vector stays unchanged; current Profile README 0.2.4 is not used to overwrite pinned Profile 0.2.3 evidence.

## Whole-function source census
- S1: https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/templates/roles/polecat.md.tmpl and gt sling/gt done operational task closure.
- S2: https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/refinery/pr_provider.go and Refinery first-party merge queue, current branch arbitration.
- S3: https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/templates/roles/mayor.md.tmpl and Witness/Deacon state/escalations.
- S3*: https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/templates/roles/refinery.md.tmpl and rebase verification and corrective routing.
- S4: https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/config/agents.go, https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/config/loader.go, https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/cmd/config.go, https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/runtime/runtime.go, https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/formula/formulas/mol-deacon-patrol.formula.toml, https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/docs/design/model-aware-molecules.md (unshipped design); existing role/runtime capabilities, no shown prospective autonomous return loop.
- S5: human Overseer governs ultimate allowed providers and town policy; role definitions/agent presets do not constitute constitutional ownership.

## Existing work / overlap
- Current role/preset configuration, manual upgrade and current cost-tier routing already work; the first-party missing integration is *prospective external-change interpretation and a bounded future-session causal return*, not another agent registry. Original #4402 remains open and #2784 is a closed current-routing plan; the distinct native scope and original GitHub states are detailed in Track A/B below.

## Function ownership
- Existing first-party Polecat S1, Refinery S2/S3*, Mayor S3 and parent Overseer S5 boundary are retained; only a separate optional Deacon future-runtime evaluation responsibility is proposed for S4. No A vector is regraded by this proposal.

## Capability priority
- P0: source-native optional Deacon prospective role-runtime compatibility wisp with the complete source -> decision -> future operation -> task feedback chain. P1: envelope, canary and fail-closed controls. P2: external feed adapter if useful. Priority does not imply a maintainer need or product desirability.

## Implementation options
- A0: keep manual config/upgrade; A1: add static runtime preset or next-task router; A2: propose optional native Deacon future-runtime choice and canary/return integration. No implementation is part of this run; A2 is hypothetical.

## Specification and domain alternatives
- The Index owns accepted current/historical VSM grades, Profile owns semantics, and original maintainers own product direction. Gas City is an independently assessed original; do not transfer its policies/code or treat a maintainer comment on pool strategy as an automatic veto on architectural constructibility.

## Cost experiment
- If an implementation is ever approved, match the same dated external notice, allowed agent pair and later coding task across baseline manual role selection, existing current routing and the optional S4 candidate. Compare actual task completion, reversions and running-session safety without claiming measured benefit today.

## Parallel contribution-on-top review
- Evaluation object: existing stable Gas Town capability-roadmap-runtime-adaptation-20261118, narrower post-v0.18.1 native-specific future runtime compatibility constructor, not a second unrelated case or a product recommendation
- Existing-work overlap: shipped static role agent config, cost tiers, CLI override, live status and patrol; original Issue #4402 OPEN proposes runtime registry and role selection, #2784 CLOSED concerns current task-intelligent agent routing, #1143 OPEN concerns longitudinal execution cost, #3147 CLOSED pool-strategy work with Gas City pointer; unmerged PRs #3841/#4368 propose specific runtime hooks/presets and open PR #4981 proposes model pricing; these neither prove shipped S4 nor establish product intent
- Our on-top contribution: optional original-native Deacon future-runtime evaluation wisp plus bounded current AgentPresetInfo/RoleAgents integration, Beads decision receipt, one next-session canary via gt sling --agent, Witness/doctor return, authorized role config adjustment and Mayor re-evaluation
- Incremental benefit: a new *architectural* external-change-to-subsequent-task evidence and decision loop, distinct from static cost tiers, manual upgrade and present-task routing; product outcome and cost advantage remain unmeasured
- Decision scope: v0.18.1 proposal-stage GO for possible S4=C construction only; no proof of shipped feature, no current Index regrade or automatic maintainer adoption, no native implementation

| S4 chain | First-party native path (Track A) | Minimum proposed addition (Track B) | Qualification / falsifier |
|---|---|---|---|
| Outside/future signal | binary staleness/manual gt upgrade, runtime preset metadata, design docs | dated provider/runtime release notice attached to optional Deacon wisp | no external source or stale signal must not authorize a choice |
| Autonomous legitimate choice | Deacon patrol and Mayor can reason about current runtime health; role settings are human-configured | wisp selects retain, allowed canary or rollback in explicit provider/role envelope | a generic monitor alone fails C |
| Real later effect | config loader, AgentPresetInfo, gt config agent set, gt sling --agent | scoped one-session future role trial, then guarded future mapping change | never mutate running sessions or parent policy |
| Return and learning | Witness monitors sessions, Beads/mail and Mayor receive operational returns | connect actual canary outcome to wisp and subsequent choice; rollback failures | no outcome return fails C |

## Native specificity and minimal integration
- Keep the real AgentPresetInfo registry as the source for hooks, resume, process detection and startup-fallback capabilities; do not build another agent-provider interface just for OpenSiro.
- Reuse the existing Deacon patrol formula/wisp lifecycle, not a new standing VSM authority. The new bounded work is an optional future-runtime evaluation step and a future-session trial/feedback receipt.
- Reuse role agent resolution and existing config persistence; a named preset alone is not a complete S4 function. Keep user-approved provider allowlist and active-session stability.
- This design can be useful only if the exact Gas Town lifecycle and role/config boundaries hold; a portable external provider adapter without these links is not qualified.

## Native acceptance / future work (NOT RUN)
1. Positive: a trusted dated deprecation/change notice for an allowed preset leads to a choice between two authorized role options, one isolated subsequent gt sling session, an observed task and post-task Witness/doctor report, a bounded future routing update or rollback and a response to Mayor.
2. Negative: current-session immutability, unavailable/unauthorized preset, revoked authority, stale source, no real task outcome, canary failure, concurrent config update and explicit owner PAUSE all block promotion, preserve prior mapping and return evidence.
3. Baseline: patch disabled, shipped defaults and current static/overseer config still work; compare with simplest native manual configuration and #4402 path before claiming user value.
4. No native tests or cost experiments executed here. Planning artifact is not a native feature, external PR or acceptance verdict.

## Historical comparison — ONLY AFTER independent first-pass seal
- Separate first-pass record completed before inspecting old case: SHA-256 6ad7c67ce294a30656d3260aa73646a2eae0a9ab41cdb9ff2966596e38cba067 (local source-only sealed research, 2026-11-20 UTC). It independently chose a Deacon-specific S4 loop and GO / NEEDS_EVIDENCE.
- Prior canonical case at opensiro-contributions/gastown@fea9afb21be7a32d31dfb2f63994be145d810375 returned NO_GO / NO_QUALIFIED_C_TARGET / NO_USEFUL_CHANGE (including 2026-11-19 repeat). That prior argument questioned whether an external signal, authorized actor, minimal effect and task return could be native, and considered Gas City direction. This review identifies exact shipped seams and one optional wisp/canary/return insertion for the **same case**, rather than inferring maintainer rejection or pretending the earlier negative was invalid evidence.
- Earlier files, event 20261119T230929Z--gastown-no-go-repeat-source-audit, and fork public Issue #1 are historical and unchanged by this plan-only report except the current case documents. No claim that Issue #1 reflects this updated proposal.
- Product choice, evidence of usefulness and official re-assessment remain independent decisions.

## Delivery and publication
- Result: NEEDS_EVIDENCE
- Validation: structural validator pending at authorship; native tests NOT_RUN; measured cost NOT_MEASURED
- External issue: DRAFT — NOT PUBLISHED
- Cost status: NOT_MEASURED
- Publication note: historical fork Issue #1 unchanged; no original communication
- Human: [issue.md](issue.md). AI: [constructor-sufficiency.md](constructor-sufficiency.md). Canonical: [roadmap.md](roadmap.md)
- Reporting: status-only Upstream PR NOT CREATED; short receipt/concurrency status belongs to existing Upstream #58. Optional supplementary links only in shared reporting document during a future consolidated maintenance change.
