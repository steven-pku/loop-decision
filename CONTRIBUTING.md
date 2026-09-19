# Contributing

Thanks for your interest. This skill is instruction-only — contributions are
markdown edits, which keeps the bar low and the review honest.

## Ground rules

1. **No fabricated sources.** Every rubric anchor and framework claim carries
   a citation with an evidence tier in `references/anchors-and-sources.md`
   (primary / consensus / rule of thumb). A PR that adds a claim without a
   tier-honest citation will be asked to fix it — including popular quotes
   that "everyone knows" (see the Kahneman misquote note in that file).
2. **No scripts.** Instruction-only is a design decision (auditability,
   portability, supply-chain safety), not a missing feature. PRs adding
   runtime code will be declined.
3. **Keep the gate honest.** The reversibility gate must keep protecting both
   directions — changes that make the skill process every small decision, or
   wave through irreversible ones, break its core.
4. **Chinese-first.** Templates and examples target Chinese decision briefs.
   An English mode would need its own examples and evals — open an issue
   first if you want to build one.

## Workflow

- Open an issue describing the failure mode you hit. Use synthetic or
  desensitized examples; never post a real offer, contract, medical record,
  financial position, or identifiable workplace material.
- For text changes: PR against `main`, one topic per PR.
- CI runs the agentskills spec validator and markdownlint; both must pass.

## Reporting problems

- Quality bugs (bad scoring, ritual passes, strawman tolerance): GitHub issue
  with the input that triggered it (desensitized).
- Security-relevant findings: see [SECURITY.md](SECURITY.md).
