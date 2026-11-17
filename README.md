# MDE09: Lightweight Evidence Retrieval for Scientific Citation Verification

**Status (2026-11-17):** Prepared research workspace, runnable evaluation code and real local unit-test execution. **NOT** a verified reproduction of a published citation-checking model; **NO** SciFact benchmark results have been measured. This preliminary experiment evaluates evidence retrieval, not the factual validity or temporal outdatedness of a citation.

## Research question
Does reciprocal rank fusion (RRF) of BM25 and TF-IDF improve evidence-document Hit@5 on SciFact compared with the two retrieval baselines, under a frozen common protocol?

## Setup
Python 3.10+ is recommended [compatibility on user's platform TO TEST].
```bash
python -m pip install -r requirements.txt
python -m pytest -q
python -m scripts.evaluate --corpus data/corpus.jsonl --claims data/claims_dev.jsonl --output-dir results/scifact_dev
```
All commands except unit tests are **[TEST REQUIRED on official SciFact data]**.

## Inputs and outputs
Inputs are official SciFact corpus and claim JSONL. Excludes claims without evidence; the resulting estimand is *retrieval of a known evidence document among claims with evidence*, not detection of unsupported claims. Outputs: `results.csv`, `per_claim.csv`, `run_config.json`, and `hit_at_5.png`.

## Fixed protocol
Compare TF-IDF (uni/bi-gram), BM25 (k1=1.5,b=.75), and RRF(k=60) on exactly the same corpus and claim split. Primary metric Hit@5; secondary metrics Hit@1/3/10, MRR and median per-query latency. No test-split tuning. Report dataset size and exclusions. RRF is a standard method, not claimed novel. Interpret latency cautiously (Python implementations, initialization excluded). See `configs/protocol.json`.

## Scientific limitations
SciFact is mainly biomedical claim verification; no temporal supersession annotations. Claim-to-document retrieval is only one subtask of citation verification. Correct document retrieval does not prove entailment. Multiple gold documents and no-gold examples require careful interpretation. This code is **not** the published VeriSci implementation and cannot be labeled an exact SciFact benchmark reproduction.

## Evidence provenance
Original review `mde_09_ritam_santra.pdf`; original assignment `AI_Tools_for_Research_post_mid_sem_assignment (1).pdf`. See `docs/all_18_prompts.md`, `research_decisions.md`, `baseline_validation.md`, `ai_assistance_log.md`, and `paper/main.tex`.

## Reproduction checklist
1. Verify official data version/license. 2. Run environment unit tests. 3. Freeze configs and hash input files. 4. Run all methods on the same evidence-bearing dev claims. 5. Inspect errors and time. 6. Preserve raw outputs and commands. 7. Never report unit-test fixture scores as research findings.
