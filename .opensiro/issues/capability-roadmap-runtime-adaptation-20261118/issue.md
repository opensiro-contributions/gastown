# Gas Town — source-native S4 runtime adaptation roadmap (OpenSiro plan-only)

**OpenSiro pilot · PLAN_ONLY / NEEDS_EVIDENCE · architecture discussion, not an implementation request.**  
**Human layer:** this document. **[AI/developer construction contract](https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/constructor-sufficiency.md)** · **[Source-pinned roadmap receipt](https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/roadmap.md)** · **[case index](https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/README.md)**.

## 1. Why OpenSiro and central accepted VSM assessment

OpenSiro tests whether reusable, VSM-informed organizational specifications can standardize AI-agent harness development and **reduce total implementation, integration, review and maintenance costs**. The method organizes current Gas Town features and external proposals into a native, composable capability path rather than asking maintainers to adopt a VSM architecture. **Lower cost, adoption and superior outcomes are hypotheses, not results.**

**HISTORICAL STARTING POINT — ACCEPTED INDEX, NOT A TARGET:** **S1=A · S2=A · S3=A · S3*=A · S4=— · S5=—**.  
[Accepted assessment](https://github.com/opensiro/vsm-harness-index/blob/03b3cd41621b85cb4c2418eab574db030493512c/assessments/ga/gastown.md) (file blob `63864bc37d10e192d0ae8a96d1bfd6307bb03a09`), reviewed **2026-09-19** at original `649b832b7672bc7a2dbef26f5983aba6198b819b`, Profile **0.2.3**, Skills methodology **0.3.5**.

| VSM | Accepted | Original decision/closure | Roadmap consequence |
| --- | --- | --- | --- |
| S1 Operations | A | Polecats complete delegated coding work | Excluded from mandatory C work |
| S2 Coordination | A | Refinery serializes and resolves merge interference | Excluded from mandatory C work |
| S3 Current management | A | Mayor allocates current commitments/rigs and handles escalation | Excluded from mandatory C work |
| S3* Complementary audit | A | Separate Refinery verifies and may reject worker output | Excluded from mandatory C work |
| S4 Future adaptation | — | No first-party outside/future option-to-operation closure was established at review pin | **Conditional P0 hypothesis**, not a present defect finding |
| S5 Ultimate policy | — | No first-party ultimate-purpose/policy closure was established at review pin | Do not invent S5 or transfer Overseer authority |

**Pins and limits:** [original main at 94cc82289d2e](https://github.com/gastownhall/gastown/commit/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e), observed 2026-11-18; historical assessment is **60 days old** and a new Index review is recommended. Boundary is one first-party Gas Town workspace and its supported roles; external model providers, downstream repositories, optional extensions and maintainer governance are not counted as Gas Town-owned S4/S5. Matching [OpenSiro working fork](https://github.com/opensiro-contributions/gastown) uses **opensiro/meta** only for research records. Original source is MIT-licensed; [CONTRIBUTING](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/CONTRIBUTING.md) permits external feature-branch PRs and asks for an issue before large changes; this case authorizes no external publication. No CLA/AI-policy clearance is asserted.

**A, C and P describe ownership, not maturity.** Existing A functions are not required to turn into C. This draft does not regrade current main.

## 2. User capability and decision

**P0 — developer-composable S4 future runtime adaptation (conditional):** A developer wants to configure an autonomous first-party adaptation actor that handles a **credible upcoming** AI runtime/provider lifecycle change (deprecation, compatibility change or changing future capability). It must distinguish the future risk, offer supported choices such as **retain / migrate / hold**, select one within delegated authority, apply it to **later** legitimate sessions, and return actual success/failure to Mayor's S3 current management.

This is **not** a duplicate crash retry, rate-limit failover, model router or blanket periodic poller. **Native alternative:** an operator changes a [configured agent preset](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/docs/agent-provider-integration.md) or existing [role / cost-tier setting](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/cmd/config.go) and launches the subsequent sessions. If that already delivers the needed outcome at lower full cost, select **NO_USEFUL_CHANGE**.

## 3. Native shipped behavior vs proposed overlap

| Existing native path / proposal | Source status at 2026-11-18 | Residual question |
| --- | --- | --- |
| [Agent preset registry](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/config/agents.go), [provider guide](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/docs/agent-provider-integration.md) | SHIPPED | Are prospective adaptation choices already composable and independently closed? Not proven |
| [Merged cost-tier PR #1564](https://github.com/gastownhall/gastown/pull/1564) and [current config command](https://github.com/gastownhall/gastown/blob/94cc82289d2ead275a62e1db4ef1d4ada4a1f98e/internal/cmd/config.go) | MERGED / SHIPPED | Cost-tier selection alone is not outside-and-then S4 |
| [#232 profile switching](https://github.com/gastownhall/gastown/issues/232) | OPEN ISSUE | Reuse for reactive provider recovery; not equivalent to prospective S4 |
| [#4332 provider transition](https://github.com/gastownhall/gastown/issues/4332) | OPEN ISSUE | Possible concrete prospective-environment trigger; confirm active maintainer need |
| [#1143 learning loop](https://github.com/gastownhall/gastown/issues/1143); [PR #1729](https://github.com/gastownhall/gastown/pull/1729) | OPEN ISSUE; CLOSED_UNMERGED PR | Reuse source evidence, not a shipped cost-outcome-learning loop |
| [PR #4981 pricing](https://github.com/gastownhall/gastown/pull/4981) | OPEN PR | Do not duplicate live PR or claim updated prices already shipped |
| [#3147 agent pools](https://github.com/gastownhall/gastown/issues/3147) | CLOSED; maintainer cited Gas City transition | Verify product ownership before any new large Gas Town feature |

**Unverified gap:** whether a source-native, first-party autonomous developer-composed **future adaptation** decision/feedback loop is materially better than a small extension to existing config/formulas or simply belongs in Gas City. No missing grade alone proves user demand.

## 4. Priority and minimum sufficient outcome

| Priority | Purpose | Conditional complete path |
| --- | --- | --- |
| **P0 / S4** | Developer composes a lawful prospective adaptation choice | **Verified future signal → versioned available alternatives → developer-bound autonomous choice → authorized future config/session effect → actual session feedback to S3** |
| **P1 / dependencies** | Make P0 safe, reachable and testable | Reuse agent presets, config loader, formulas, role rights, sessions and Beads; only add missing first-party sensing/option state, guarded application, receipt and native tests |
| **P2 / NONE** | No justified secondary function | No automatic S3 or S5 constructor, no C(P)/A(P) ladder |

**C-sufficiency hypothesis, not certification:** the [separate technical companion](https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/constructor-sufficiency.md) maps every proposed S4 port to first-party source, decision actor, rights, closure and falsifiers. The full five-link path **could** qualify for future C review if actually shipped in a supported first-party mode; no current C is asserted.

## 5. Acceptance and stop gates

- **Positive:** a developer-installed autonomous adaptation actor selects one of two real supported future options; a later authorized Gas Town session uses the selected configuration and returns a verifiable result.
- **Counterfactual:** choosing `hold` or another lawful option changes the later outcome; without the installed decision actor, no invented autonomous decision occurs.
- **Authority:** unapproved provider/credentials, revoked rights, unsupported runtime and stale state must fail closed without changing existing sessions or the Overseer's reserved policy.
- **Compatibility:** working Polecats retain their assignments; application/restart failures return real failure, never fake successful adaptation.
- **Native alternative:** if ordinary configuration or an existing original proposal meets the identical task as cheaply, stop the new constructor.
- **Ownership:** if Gas City has superseded this feature boundary, link that existing issue/repository rather than opening duplicate Gas Town feature requests.

**Tests proposed, not run.** Neither this issue nor an unmerged PR can alter an Index grade.

## 6. Independent paths

**(a) Gas Town original-native integration:** prefer a small amendment to existing proposals and code; product implementation requires a separately authorized Upgrade. **(b) OpenSiro Profile/Skills feedback:** only if evidence reveals a semantic/methodology ambiguity. **(c) experimental domain fork:** a separately scoped, legal comparison of the same user task and first-party baseline. No maintainer adoption is presumed.

## 7. Cost hypothesis

For the **same planned provider migration**, compare manual native config/preset changes versus the proposed S4-composable decision: coding/integration/review/testing hours, repeated migrations, runtime failures, human interventions, maintenance and successful later-work return. **Cost status: NOT_MEASURED**.

## 8. Decision and handoff

**NEEDS_EVIDENCE** before engineering: establish an actually demanded prospective-runtime scenario, confirm actual current-main actor/decision/feedback gap, deduplicate the listed issues/PRs and clarify Gas Town versus Gas City ownership. A source-pinned Index reassessment is recommended (soft freshness advisory), not a roadmap blocker.

[AI/developer contract](https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/constructor-sufficiency.md) is the implementation-oriented evidence/acceptance handoff; [receipt](https://github.com/opensiro-contributions/gastown/blob/opensiro/meta/.opensiro/issues/capability-roadmap-runtime-adaptation-20261118/roadmap.md) records pins and limits. These are **one OpenSiro fork-local discussion case**, not two Issues. No Gas Town implementation, external original issue, original PR, grade change, testing result, autonomy grant or measured saving is claimed.

**AI disclosure:** Prepared with AI assistance. Source-native tests and independent human validation were not performed.
