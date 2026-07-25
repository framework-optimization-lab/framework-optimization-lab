# Governance you can run

**Tania Mason** — AI governance, decision support, and delivery frameworks, built inside large-scale healthcare payer platform operations.

Everything here demonstrates one idea: **an AI system you can act on needs governance designed in, not bolted on.**

Each repository is a small, runnable build of a governance pattern drawn from enterprise AI work — re-authored clean-room, with synthetic, domain-neutral data only. The pattern is always the same: a written model of the controls, then code that actually enforces them, then tests that prove each control fires.

## The repositories

| Repository | What it is | What it proves |
|---|---|---|
| 📘 [governed-playbook-assistant](https://github.com/framework-optimization-lab/governed-playbook-assistant) | A governed RAG question-answering app over an operating playbook | Answers come only from retrieved, citable evidence; out-of-scope questions are **refused before the model is even called**; every answer carries a confidence tier and sources |
| 🛡️ [ai-decision-governance-gate](https://github.com/framework-optimization-lab/ai-decision-governance-gate) | A policy-as-code checkpoint for AI "decision records" | No output ships without passing policy: **PASS / REVIEW / BLOCK** verdicts enforcing provenance, no fabrication, mandated refusal, and human sign-off — with the full governance model in `docs/` |

The two are companions. The assistant governs answers **on the way in** — only evidence reaches the model. The gate governs decisions **on the way out** — nothing is released ungoverned.

## The common threads

- **Evidence over assertion** — every claim traces to a registered, citable source.
- **Refusal instead of guessing** — "insufficient evidence" produces a logged refusal, never a fabricated answer.
- **Deterministic code owns correctness** — the LLM orchestrates and explains; it never states a number it computed itself.
- **A named human stays accountable** — high-risk decisions require explicit sign-off before action.
- **Auditable by construction** — every run leaves a record you can defend after the fact.

## Background

These patterns come from designing AI-enabled decision support, identifier governance, and delivery frameworks inside large-scale healthcare payer platform operations — an environment where an unsupported number or an unowned decision has real consequences. The repositories are the generalized, runnable versions of that work.

All code is dependency-light Python with passing test suites. All data is fictional.

## Contact

LinkedIn: [linkedin.com/in/tania-mason-payertech](https://www.linkedin.com/in/tania-mason-payertech)
