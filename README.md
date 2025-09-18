# NLP and Text Analytics — Assignments and Final Exam Project

This repository collects the work of me and my peers for the course “Natural Language Processing and Text Analytics (CDSCO1002U.LA_F25)” at Copenhagen Business School. It contains two course assignments and the code and notes supporting the final exam project on clause retrieval for legal contract drafting.

## Repository structure

| Path | Type | Description |
| --- | --- | --- |
| `assignment_1.ipynb` | Jupyter Notebook | Preprocessing and classical NLP models used in coursework. |
| `assignment_2.ipynb` | Jupyter Notebook | Topic modeling, vectorization, and baseline retrieval experiments. |
| `final/NLP_TA_final_exam_ItaMark.ipynb` | Jupyter Notebook | End-to-end pipeline used for the exam project. |
| `final/NLP_exam_Written_Product.pdf` | PDF | Exam write-up describing the dataset, pipeline, and evaluation. |
| `README.md` | Markdown | This file. |


## Final project overview

The final project evaluates clause retrieval pipelines for commercial contract drafting on a graded-relevance benchmark. It compares lexical retrieval (TF-IDF, BM25), dense bi-encoders (MiniLM, SBERT, Legal-BERT), and second-stage cross-encoder rerankers (MS MARCO MiniLM and GPT-4.1-nano). Evaluation uses NDCG@k and star-precision@k on a clause corpus annotated by legal experts. The study finds that dense retrieval improves over lexical baselines and that lightweight cross-encoder reranking yields the largest gains on graded relevance, while still requiring expert review for “paste-ready” clauses.


