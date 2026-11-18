# Gas Town roadmap — follow-up evidence adjudication (2026-11-18)

**Scope:** Existing source-pinned roadmap for `gastownhall/gastown` in OpenSiro's [fork-local Issue #1](https://github.com/opensiro-contributions/gastown/issues/1). Original Issue body, `issue.md`, technical constructor contract, and initial receipt are **historical snapshots and were not edited**.

**Verdict: `NO_USEFUL_CHANGE` for implementing a NEW S4 future-runtime-adaptation constructor in the retired Gas Town product.**

This is a **decision on the proposed engineering target**, not a claim that S4 is already shipped in Gas Town, a normative Index reassessment, a proof that S4 cannot be useful, or a conclusion about Gas City's VSM classification. The research route remains PLAN_ONLY. Cost impact: `NOT_MEASURED`; native runtime acceptance tests: `NOT_RUN`.

## New decisive first-party evidence

1. **Product lifecycle:** Steve Yegge's [Gas Town project page](https://yegge.ai/gastown) identifies Gas Town as retired and explicitly identifies Gas City as its successor. This is an author-origin publication, not a source-code test.
2. **Maintainer routing decision:** on [Gas Town issue #3147, comment 4151252437](https://github.com/gastownhall/gastown/issues/3147#issuecomment-4151252437), Steve Yegge closed a feature proposal on **2026-03-29** saying the system was transitioning to Gas City and that relevant ideas should be filed against the new project.
3. **Owning product's native migration semantics:** [Gas City's first-party migration guide](https://github.com/gastownhall/gascity/blob/11a3589ab9e5df40150028b9461a98c605ad3965/docs/getting-started/coming-from-gastown.md) states that hardcoded Gas Town roles become configurable pack agents, schedulers/plugins become orders, and formulas and state are driven by the Gas City orchestrator. It explicitly says platform features lift configured Gas Town implementations too.
4. **Current supported extension primitives:** [Gas City code: runtime registry](https://github.com/gastownhall/gascity/blob/11a3589ab9e5df40150028b9461a98c605ad3965/cmd/gc/runtime_registry.go) plus [pack runtime declarations](https://github.com/gastownhall/gascity/blob/11a3589ab9e5df40150028b9461a98c605ad3965/internal/config/pack_runtimes.go) already provide first-party extensibility. [Gas City product architecture](https://github.com/gastownhall/gascity/blob/11a3589ab9e5df40150028b9461a98c605ad3965/docs/getting-started/how-gas-city-works.md) exposes agents, packs, orders, formulas, events and durable beads.
5. **Active Gas City proposal overlap:** [#2075](https://github.com/gastownhall/gascity/issues/2075) (pack-based provider/runtime decomposition), [#19](https://github.com/gastownhall/gascity/issues/19) (account/quota rotation), [#9006](https://github.com/gastownhall/gascity/issues/9006) (remaining runtime protocol capabilities) remain OPEN as observed 2026-11-18. These are **proposals and partial substrate**, not proof of a complete S4 controller.
6. **Original Gas Town roadmap overlap:** [#4332](https://github.com/gastownhall/gastown/issues/4332) (future CLI transition), [#232](https://github.com/gastownhall/gastown/issues/232) (rate-limit failover), and [#1143](https://github.com/gastownhall/gastown/issues/1143) (execution cost and outcome learning) remained OPEN as observed 2026-11-18. None is an accepted Gas Town S4=C witness; rate-limit recovery alone is a present-operation mechanism.

**Pinned HEAD readback:** original `gastownhall/gastown/main` was `94cc82289d2ead275a62e1db4ef1d4ada4a1f98e`; successor `gastownhall/gascity/main` was `11a3589ab9e5df40150028b9461a98c605ad3965`, observed 2026-11-18.

## Decision rule and native alternative

The old P0 requested source-native, developer-composable **future** runtime adaptation that chooses `retain/migrate/hold` and returns an actual later-session outcome to the present S3 owner.

**The decisive changed fact is engineering ownership, not an implementation test.** Adding a major Gas Town-specific S4 constructor would duplicate a legacy organizational surface whose roles and provider integration are already represented by Gas City's configurable platform. The more economical native alternative **to investigate**, without asserting measured savings, is a bounded *Gas City* pack/order/formula enhancement, reusing its current runtime registry/config/evidence flow. A simpler manual preset/config change is still the benchmark for any actual end-user future-provider migration.

We did **not** establish that Gas City currently has the full five-link S4 future-disturbance → autonomous legal option → protected apply → later session feedback closure. Therefore this is **NOT** `NO_USEFUL_CHANGE` for all future S4 work.

## Result and next permitted decision

- **Gas Town new S4 implementation:** `NO_USEFUL_CHANGE` (stop new architecture in this retired original; do not open a corresponding external original Issue/PR).
- **Original fork-local Issue #1:** leave OPEN as a public historical research/discussion index; its approved body remains byte-identical to pinned `issue.md`. No public Issue comment/edit/closure was made.
- **Gas City future S4 hypothesis:** `NEEDS_EVIDENCE` as a separate potential target. Assess against *Gas City's own* accepted Index record (if any), current source, overlaps, legal/publication rules and first-party native operation, not Gas Town's historical six-function vector.
- **Decision readiness:** enough evidence to decide **not to build the proposed controller in Gas Town**, not enough evidence to issue an implementation-ready S4 constructor for Gas City.
- **No original repo communication:** no external issue, PR or comment is authorized by this verification; any new public fork-local or original Issue needs independent exact approval.

**Evidence type:** first-party documentation, live GitHub Issue/PR state and source-code reading; **no code changes**, native end-to-end runs or cost benchmarks.
