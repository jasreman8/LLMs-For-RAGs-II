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

**PROJECT 2:** Implementing query expansion and hypothetical questions for RAG retrieval learning:
- Created an ephemeral ChromaDB vector store with a small document corpus
- Implemented query expansion to generate multiple semantically related queries
- Generated hypothetical questions (HyDE-style) to bridge user queries and document language

**PROJECT 3:** Adding a foundational multimodal document parsing and indexing pipeline:
- Parsed a multimodal laptop manual containing text, tables, and images using LlamaParse
- Generated textual descriptions for tables and images to enable semantic indexing
- Chunked and processed extracted text for embedding generation

**PROJECT 4:** Exploring RAG generation improvements using compression and re-ranking:
- Retrieved top-k (k=3) relevant document chunks for a given query
- Applied a compression retriever to summarize and select the most salient document for the generation context
- Implemented re-ranking to reorder the top-k retrieved chunks based on semantic relevance
- Observed and compared differences between compression-based selection and re-ranking order
