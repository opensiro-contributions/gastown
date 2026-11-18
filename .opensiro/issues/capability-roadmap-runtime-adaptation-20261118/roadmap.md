# Capability Roadmap Receipt — Gas Town (source-pinned, plan-only)

## Identity and pins

- Original repository: gastownhall/gastown
- Original HEAD: 94cc82289d2ead275a62e1db4ef1d4ada4a1f98e
- Observed at: 2026-11-18
- Accepted Index assessment: https://github.com/opensiro/vsm-harness-index/blob/03b3cd41621b85cb4c2418eab574db030493512c/assessments/ga/gastown.md
- Accepted assessment blob SHA: 63864bc37d10e192d0ae8a96d1bfd6307bb03a09
- Accepted review ref: 649b832b7672bc7a2dbef26f5983aba6198b819b
- Accepted reviewed at: 2026-09-19
- System in focus: One first-party Gas Town workspace, including canonical Mayor, Polecat, Refinery, Witness, Deacon, rigs, Beads state and runtime/config/session boundaries; external models and third-party GitHub outside claimed ownership
- Historical profile and assessment procedure: 0.2.3 / 0.3.5; **S1=A · S2=A · S3=A · S3*=A · S4=— · S5=—**; 60 days since accepted review, recommend source-pinned Index re-review without assuming a new grade.
- Original default branch: main, source: https://github.com/gastownhall/gastown/commit/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e; working fork: https://github.com/opensiro-contributions/gastown, correct parent confirmed.
- Human Issue: https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/issue.md
- AI/developer contract: https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/constructor-sufficiency.md

## Rights and authority

- Root source license: MIT (read actual text, [LICENSE](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/LICENSE)); external source is readable and forkable.
- [Contributing policy](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/CONTRIBUTING.md): external contributors use fork feature branches and PRs; significant changes require prior issue; native `go build -o gt ./cmd/gt && go test ./...`.
- Formalities: no affirmative claim that personal CLA/DCO or AI disclosure requirements are waived; recheck before outside publication.
- Fork `opensiro/meta`: case metadata only; exact public fork Issue text requires distinct current-conversation approval. Original external issue/PR needs another exact approval. No human attestation performed.

## Existing work / overlap

- SHIPPED: [runtime presets](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/config/agents.go), [config and cost tiers](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/cmd/config.go), [agent-provider integration](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/docs/agent-provider-integration.md), [Mayor S3 owner](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/templates/roles/mayor.md.tmpl).
- MERGED: [cost-tier #1564](https://github.com/gastownhall/gastown/pull/1564).
- OPEN ORIGINAL ISSUES: [#232 rate-limit failover](https://github.com/gastownhall/gastown/issues/232); [#4332 provider transition](https://github.com/gastownhall/gastown/issues/4332); [#1143 cost/outcome learning](https://github.com/gastownhall/gastown/issues/1143).
- CLOSED ORIGINAL ISSUE: [#3147 pool proposal](https://github.com/gastownhall/gastown/issues/3147), closed with maintainer Gas City transition note.
- CLOSED UNMERGED: [#1729 cost learning PR](https://github.com/gastownhall/gastown/pull/1729).
- OPEN ORIGINAL PR: [#4981 pricing update](https://github.com/gastownhall/gastown/pull/4981).
- No overlapping fork-local Issue before case creation; fork Issue tracker was disabled on fresh fork and enabled for explicitly requested local Issue path. These observations are dated, not permanent claims of current statuses.

## Function ownership

- Historical S1=A Polecats (operational decisions), S2=A Refinery (inter-Polecat merge interference), S3=A Mayor (current town resources and work commitments), S3*=A Refinery (independent verification); each excluded from mandatory C target.
- Historical S4=—: no qualifying external/future option→adaptation→current-control feedback path at reviewed pin. Current-main proof still incomplete; conditional C hypothesis, not a defect assertion.
- Historical S5=—: no separate ultimate-purpose policy closure at assessed boundary; preserved operator rights, no manufactured S5.
- S4 disturbance/decision/return proposal: prospective runtime deprecation or compatibility change → developer-bound S4 autonomous actor selects approved retain/migrate/hold alternative → first-party authorization and future session apply → session result returned to Mayor S3.

## Capability priority

- **P0 S4:** smallest useful function-specific developer-composable prospective runtime adaptation path, if a material residual task survives source overlap.
- **P1:** verified future event + versioned legal options + developer decision binding + guarded native config/session application + truthful later session feedback; may execute before P0.
- **P2: NONE:** no separately justified S3 or S5 enhancement.
- **Conditional C sufficiency:** all five linked proposed ports and positive/alternative/negative/feedback tests are required to prove one complete supported first-party pathway; roadmap design is not accepted Index C.
- **Decision:** NEEDS_EVIDENCE: clarify maintainer Gas City ownership, specific operator need and real current-main S4 gap; simplest native alternative may win.

## Implementation options

- Prefer native issues/PR integration rather than parallel VSM architecture: assess original #4332, #232, #1143 and future target owner; retain compatibility with provider registry and cost-tier settings.
- Smallest source-native implementation, **only after separate authorization**, would reuse `internal/config/agents.go`, `internal/config/loader.go`, `internal/cmd/config.go`, existing role/formula/session state; add only justified missing future signal, decision, rights, application and receipt.
- Acceptance scenarios in [AI companion](https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/constructor-sufficiency.md): real later session with different lawful choice; negative unapproved provider/revocation/stale revision; preserving active assignments; failed launch return; native baseline control.
- Test commands are proposed, NOT EXECUTED: `go build -o gt ./cmd/gt`, `go test ./internal/config/...`, `go test ./internal/cmd/...`, `go test ./...`.
- Stop at **NO_USEFUL_CHANGE** if already-shipped provider configuration or Gas City covers same user task with no material additional benefit.

## Specification and domain alternatives

- Profile/Skills feedback only if fresh evidence reveals ambiguity in S4/S3 semantics or C-construction methodology.
- Legally permissible domain-scoped experimental fork is an independent alternative; no default adoption or original maintainer authority.
- Do not optimize historical grades or infer `A → C` conversion; native user need outranks taxonomy.

## Cost experiment

- Compare identical upcoming provider migration via manual presets/role configuration vs source-native developer-composed S4 controller.
- Record implementation, integration, review, validation, repeated migration, compatibility/support, human escalation, maintenance costs and later first-party execution success. No values independently measured.
- Cost status: NOT_MEASURED

## Delivery and publication

- Result: NEEDS_EVIDENCE
- Route: PLAN_ONLY; existing source-linked Human and AI materials are discussion proposals only.
- Fork public Issue: **AWAITING EXACT CURRENT-CONVERSATION APPROVAL**; draft body at [issue.md](https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/issue.md).
- External issue: DRAFT — NOT PUBLISHED
- Original implementation, fork-local review PR, third-party Issue/PR, native test and autonomous VSM grade change: NOT PERFORMED.
- Next permitted action: current owner confirms exact public fork Issue title/body; then use first-party issue creation and readback. No original maintainer communication without separate approval.
