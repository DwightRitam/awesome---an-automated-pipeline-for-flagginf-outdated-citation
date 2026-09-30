# Open-Source Implementations & Learning Resources

Selected open-source repositories and educational materials covering citation verification pipelines.

---

## GitHub Implementations

* **allenai/specter**
  * **Implemented Work:** SPECTER embeddings for scientific document representation.
  * **Description:** Citation-informed Transformer models that construct paper embeddings incorporating citation graphs for semantic retrieval.
  * **Link:** [allenai/specter Repository](https://github.com/allenai/specter)

* **dwadden/scifact**
  * **Implemented Work:** End-to-end scientific claim verification pipeline.
  * **Description:** Complete pipeline code for candidate passage retrieval, rationale sentence selection, and stance classification using SciBERT.
  * **Link:** [dwadden/scifact Repository](https://github.com/dwadden/scifact)

* **sebhaan/semanticcite**
  * **Implemented Work:** Claim-citation entailment verification framework.
  * **Description:** Tool for extracting claim-citation pairs and checking natural language inference against cited abstracts to detect misattributed references.
  * **Link:** [sebhaan/semanticcite Repository](https://github.com/sebhaan/semanticcite)

* **allenai/s2orc-doc2json**
  * **Implemented Work:** PDF and LaTeX parsing engine for scientific literature.
  * **Description:** Converts raw scientific papers into structured JSON format with linked inline citations and bibliographies.
  * **Link:** [allenai/s2orc-doc2json Repository](https://github.com/allenai/s2orc-doc2json)

* **CrossRef/rest-api-doc**
  * **Implemented Work:** API specifications and client tools for Crossref reference metadata.
  * **Description:** Official specifications and endpoints to check paper existence and verify retraction/update notices.
  * **Link:** [CrossRef REST API Repo](https://github.com/CrossRef/rest-api-doc)

---

## Tutorials & Learning Resources

* **Semantic Scholar Academic Graph API Developer Guide**
  * **Author/Provider:** Allen Institute for AI (AI2)
  * **Description:** Official guide on querying paper metadata, citation graphs, and embedding endpoints for automated reference resolution.
  * **Link:** [S2 API Documentation](https://api.semanticscholar.org/api-docs/)

* **Hugging Face Course: Fine-Tuning Models on Scientific NLP Tasks**
  * **Author/Provider:** Hugging Face
  * **Description:** Practical guide on adapting pre-trained Transformers (SciBERT, BioBERT) for scientific natural language inference.
  * **Link:** [Hugging Face NLP Course](https://huggingface.co/learn/nlp-course/)

* **Crossref Metadata Retrieval & Citation Integrity Guide**
  * **Author/Provider:** Crossref Technical Team
  * **Description:** Technical documentation detailing how to inspect citation metadata, query update status assertions, and process retractions.
  * **Link:** [Crossref API Guide](https://www.crossref.org/documentation/retrieve-metadata/rest-api/)

* **GROBID Service Setup & Deployment Guide**
  * **Author/Provider:** GROBID Open Source Community
  * **Description:** Instructions for deploying and configuring REST-based GROBID microservices to parse full-text research papers into machine-readable JSON/TEI XML.
  * **Link:** [GROBID Documentation](https://grobid.readthedocs.io/en/latest/)

* **Building RAG Systems for Academic Research (LlamaIndex Framework Guides)**
  * **Author/Provider:** LlamaIndex Team
  * **Description:** Developer tutorials covering semantic indexing, context chunking, and multi-stage verification pipelines over academic paper collections.
  * **Link:** [LlamaIndex Academic RAG Guide](https://docs.llamaindex.ai/en/stable/examples/usecases/academic_paper_rag/)
