# Tech-Spec-BTP

**Replicating Technical Specification Documents using RAG**

This repository contains the work for BTP-1 under the guidance of Prof. Senthilmurugan Subbiah, Department of Chemical Engineering.
The project focuses on building a Retrieval-Augmented Generation (RAG) pipeline to replicate technical specification documents, which are typically dense, multimodal, and domain-specific.

📌 **Problem Statement**

-> Technical specification documents contain acronyms, tables, figures, and structured sections that are difficult for LLMs to process reliably.

-> Vanilla RAG often fails for domain-specific contexts due to hallucinations and misinterpretations.

-> Existing research highlights sentence-level retrieval and structured term-definition handling, but no system focuses directly on replicating structured specification-style documents.

**🚀 Objectives**

Build a prototype pipeline that can:

- Parse document structures (headers, acronyms, tables).

- Retrieve relevant chunks using sentence-level retrieval (FAISS, SBERT).

- Regenerate clean specification-style sections via GPT API.

- Evaluate results using similarity and generation metrics.

**🛠️ Workflow**

_Parser →_ Extract headers, paragraphs, acronyms, and tables.

_Retriever →_ Perform sentence-level retrieval using FAISS + SBERT embeddings.

_Generator →_ Use GPT API to regenerate structured specification-style text.

_Evaluation →_ Metrics: cosine similarity, BLEU, ROUGE, Recall@k.

**📊 Proposed Evaluation Metrics**

_Retrieval Quality →_ Cosine Similarity, Recall@k

_Generation Quality →_ BLEU, ROUGE

**📈 Scope**

_BTP-1:_ Develop a working RAG prototype for replicating technical documents.

_BTP-2:_ Extend towards a multi-agent, multimodal RAG system with:

          - Multi-agent collaboration (Planner, Extractor, QA Writer).

          - Layout-aware parsing for tables and figures (Dolphin/MMST).

          - Expert-in-the-loop evaluation and semantic metrics.

📂 **References**

[Dolphin (Document Parsing)](https://github.com/bytedance/Dolphin)

[Multi-Agent RAG (Nguyen et al., 2025)](https://drive.google.com/file/d/1r2YWKU44-CIeL9mUJc6iqnrKnf-2ESsB/view?usp=sharing)

[RAG for Technical Docs (Soman & Roychowdhury, 2024)](https://drive.google.com/file/d/1ZK8EUJQhxh1Ee0oQ-ZaV3rJJt8_B5glU/view?usp=sharing)

**👩‍💻 Author**

Yoshita Banerjee
B.Tech Project, Department of Chemical Engineering
