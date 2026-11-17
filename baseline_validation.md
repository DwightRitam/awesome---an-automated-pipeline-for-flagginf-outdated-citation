# Baseline validation report — preliminary

VERIFIED: Source modules were created, unit tests exercise BM25 ranking, 3 retriever methods, JSONL parsing, and invalid ID rejection. Consult `results/unit_test_log.txt` for actual run output.

UNCERTAIN: Official SciFact data access, distribution, file hashes, performance and relevance precision. Not yet evaluated.

NEEDS CORRECTION/VERIFICATION: These baselines are own lightweight implementations rather than reproductions of the official VeriSci architecture; verify SciFact's official evaluation protocol before framing any score as benchmark-comparable. Run official corpus and inspect at least 10 errors.

DEVIATION: Restricting evaluation to claims with a nonempty gold evidence set biases the sample toward answerable retrieval questions. Disclose denominator and exclusions.
