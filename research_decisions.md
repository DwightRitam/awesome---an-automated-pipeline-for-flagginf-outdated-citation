# Research decision and evidence ledger
Date: 2026-11-17

- VERIFIED: The uploaded MDE09 review covers metadata matching, temporal graphs and NLI/agents (review pp. 3–7). Evidence: original uploaded review.
- VERIFIED: The assignment requires a second paper based on implementation and genuine controlled results, not review recycling (assignment pp. 1–2 and 9–10).
- VERIFIED: Review bibliography ref [3] assigns RefChecker to arXiv:2308.10002, but this ID resolves to an unrelated math article. Cross-check at https://arxiv.org/abs/2308.10002 . Actual RefChecker is https://arxiv.org/abs/2405.14486 . **Do not reproduce bibliography blindly**.
- VERIFIED: SciFact's original Wadden et al. paper is https://arxiv.org/abs/2004.14974 and provides evidence-labeled abstracts. Its original repository: https://github.com/allenai/scifact .
- INFERRED: Combining complementary lexical retrievers could improve coverage; not an established improvement in this project.
- UNKNOWN: Whether other frameworks and numerical performance/latency claims cited in the review are genuine and accurately characterized. Verify individually before reuse.
- DECISION: Study SciFact evidence retrieval using two transparent baselines (TF-IDF/BM25), then controlled RRF fusion. Reason: small compute, tractable, domain continuity.
- LIMITATION: This project does not test temporal outdatedness. A temporal annotation study is a future follow-up.
- NEXT: Download licensed official SciFact data; evaluate real dev split; add error cases and a correctly validated uncertainty estimate before manuscript claims.
