# Governance you can run

[![Governance Control Tower — live demo](https://repo-ai-governance-muse.lovable.app/__l5e/assets-v1/d4d8a0b8-02b4-4f05-bee3-60e05b0cf3ac/control-tower-preview.png)](https://repo-ai-governance-muse.lovable.app)

### ▶ [Open the live demo — Governance Control Tower](https://repo-ai-governance-muse.lovable.app)

No install, no signup. Ask a question and watch it get grounded or refused, watch a deterministic
seven-control gate issue **PASS / REVIEW / BLOCK**, sign off as a named human, then read the audit
trail it left behind.

| Try this | What you will see |
|---|---|
| [**Ask**](https://repo-ai-governance-muse.lovable.app/ask) | Answers bounded by retrieved playbook passages, with citations and a confidence tier |
| [**Gate**](https://repo-ai-governance-muse.lovable.app/gate) | Break a decision record on purpose and watch the controls fire |
| [**Review**](https://repo-ai-governance-muse.lovable.app/review) | Human sign-off with a written rationale; BLOCK cannot be signed away |
| [**Dashboard**](https://repo-ai-governance-muse.lovable.app/dashboard) | The audit trail and control metrics, end to end |

---

**Tania Mason** — AI governance, decision support, and delivery frameworks, built inside large-scale healthcare payer platform operations.

Everything here demonstrates one idea: **an AI system you can act on needs governance designed in, not bolted on.**

Each repository is a small, runnable build of a governance pattern drawn from enterprise AI work — re-authored clean-room, with synthetic, domain-neutral data only. The pattern is always the same: a written model of the controls, then code that actually enforces them, then tests that confirm each control fires.

## The repositories

| Repository | What it is | The controls it demonstrates |
|---|---|---|
| 🎛️ [ai-governance-explorer](https://github.com/framework-optimization-lab/ai-governance-explorer) | The live control tower above — all three patterns joined into one flow | Grounded retrieval, mandated refusal, policy-as-code verdicts, human sign-off, audit trail |
| 📘 [governed-playbook-assistant](https://github.com/framework-optimization-lab/governed-playbook-assistant) | A governed RAG question-answering app over an operating playbook | Answers come only from retrieved, citable evidence; out-of-scope questions are **refused before the model is even called**; every answer carries a confidence tier and sources |
| 🛡️ [ai-decision-governance-gate](https://github.com/framework-optimization-lab/ai-decision-governance-gate) | A policy-as-code checkpoint for AI "decision records" | No output ships without passing policy: **PASS / REVIEW / BLOCK** verdicts enforcing provenance, no fabrication, mandated refusal, and human sign-off — with the full governance model in `docs/` |

The assistant governs answers **on the way in** — only evidence reaches the model. The gate governs decisions **on the way out** — nothing is released ungoverned.

## The common threads

- **Evidence over assertion** — every claim traces to a registered, citable source.
- **Refusal instead of guessing** — "insufficient evidence" produces a logged refusal, never a fabricated answer.
- **Deterministic code owns correctness** — the LLM orchestrates and explains; it never states a number it computed itself.
- **A named human stays accountable** — high-risk decisions require explicit sign-off before action.
- **Auditable by construction** — every run leaves a record you can defend after the fact.

## Background

These patterns come from designing AI-enabled decision support, identifier governance, and delivery frameworks inside large-scale healthcare payer platform operations — an environment where an unsupported number or an unowned decision has real consequences. The repositories are the generalized, runnable versions of that work.

All data is fictional.

## Contact

LinkedIn: [linkedin.com/in/tania-mason-payertech](https://www.linkedin.com/in/tania-mason-payertech)
