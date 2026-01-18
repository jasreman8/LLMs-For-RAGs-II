# LLMs-For-RAGs-II
This repository contains additional projects on developing RAGs using LLMs and exploring RAG Triads, RAGAS, Query Expansion, Hypothetical Questions, Information Compression, and Reranking.

**PROJECT 1:** Adding multimodal RAG pipeline for complex PDFs with evaluation and query expansion:
- Implemented multimodal document ingestion for PDFs containing text, tables, charts, and diagrams
- Integrated LlamaParse to extract text, tables, and images from PDF datasets
- Generated table and image descriptions to enable cross-modal retrieval and grounding
- Unified extracted text + generated descriptions into a single retrieval corpus for RAG Q&A
- Added RAG evaluation using RAG Triad (answer relevancy, faithfulness, contextual relevancy)
- Added RAGAS evaluation (answer relevancy, faithfulness, contextual precision, contextual recall)
- Explored retrieval improvements via query expansion and hypothetical question (HyDE-style) prompting

