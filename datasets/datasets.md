# Curated Datasets for Citation Verification & Retraction Detection

Primary datasets and academic knowledge bases used for training models and auditing citation validity.

---

## 1. SciFact & SciFact-Open
* **Source:** Allen Institute for AI (AI2)
* **Description:** Expert-annotated dataset of scientific claims derived from research abstracts paired with evidence rationales and stance labels (`SUPPORT` / `CONTRADICT`).
* **Primary Application:** Scientific claim verification, citation entailment, and rationale sentence extraction.
* **Link:** [SciFact GitHub Repository](https://github.com/dwadden/scifact)

---

## 2. Crossref Retraction Watch Database
* **Source:** Center for Scientific Integrity / Crossref
* **Description:** Public database containing 40,000+ retracted research articles across scientific fields with reason codes, retraction dates, and DOI metadata.
* **Primary Application:** Outdated/retracted paper detection and automated academic integrity auditing.
* **Link:** [Retraction Watch User Portal](https://retractionwatch.com/retraction-watch-database-user-guide/)

---

## 3. Semantic Scholar Academic Graph (S2AG)
* **Source:** Allen Institute for AI
* **Description:** Open academic knowledge graph containing 200M+ publications, metadata, resolved DOIs, and inline citation locations.
* **Primary Application:** Citation context parsing, reference resolution, and co-citation graph traversal.
* **Link:** [S2 API & Data Access](https://api.semanticscholar.org/)

---

## 4. FEVER (Fact Extraction and VERification)
* **Source:** University of Cambridge
* **Description:** Benchmark dataset containing 185,000+ verified claims paired with Wikipedia evidence passages for stance classification.
* **Primary Application:** Pre-training NLI evidence retrieval models prior to domain adaptation on scientific text.
* **Link:** [FEVER Project Site](https://fever.ai/)
