# Michał Furgała

Software engineer and machine learning practitioner.  
Focused on computer vision, applied ML, developer tooling, and open-source systems across Python, PyTorch, Go, and Rust.

[Original projects](https://github.com/00200200?tab=repositories&type=source) · [Merged contributions](https://github.com/pulls?q=is%3Apr+author%3A00200200+is%3Amerged+-user%3A00200200)

---

## Merged Open Source Contributions

A selection of my pull requests merged upstream:

| Project | Ecosystem | Summary | Pull Request |
| :--- | :--- | :--- | :--- |
| **PyCQA / isort** | Python | Respect extension filters for explicit files with `--filter-files` | [#2720](https://github.com/PyCQA/isort/pull/2720) |
| **urllib3** | Python | Ensure Memray plugin availability before configuring pytest options | [#5307](https://github.com/urllib3/urllib3/pull/5307) |
| **serde_json** | Rust | Report invalid UTF-8 at the first bad byte rather than string end | [#1345](https://github.com/serde-rs/json/pull/1345) |
| **AnyIO** | Python | Skip empty object-stream messages when receiving buffered bytes | [#1409](https://github.com/agronholm/anyio/pull/1409) |
| **redis-py** | Python | Preserve zero-valued `GEOSEARCH` arguments instead of dropping them | [#4356](https://github.com/redis/redis-py/pull/4356) |
| **Fiber** | Go | Let empty optional route parameters yield to later required segments | [#4722](https://github.com/gofiber/fiber/pull/4722) |
| **narwhals** | Python | Avoid trailing separators in `concat_str` when ignoring nulls | [#3967](https://github.com/narwhals-dev/narwhals/pull/3967) |
| **pytest-httpserver** | Python | Add an opt-in case-insensitive header value matcher | [#524](https://github.com/csernazs/pytest-httpserver/pull/524) |
| **chardet** | Python | Respect encoding filters when applying preferred supersets | [#393](https://github.com/chardet/chardet/pull/393) |
| **set-cookie-parser** | JavaScript | Ignore invalid `Expires` attributes to retain valid expiry dates (v3.1.4) | [#91](https://github.com/nfriedly/set-cookie-parser/pull/91) |

My DuckDB fix for `overwrite=False` was submitted in [#642](https://github.com/duckdb/duckdb-python/pull/642) and incorporated by a maintainer in the merged [#668](https://github.com/duckdb/duckdb-python/pull/668).

---

## Selected Projects

### Computer Vision & Deep Learning

- **[Video Waste Dumping Detection (IWDD)](https://github.com/00200200/Video-Waste-Dumping-Detection---IWDD)**  
  Video classification pipeline developed for the international IWDD competition. Evaluates VideoMAE and X-CLIP architectures for automated surveillance and environmental monitoring.  
  `PyTorch` `PyTorch Lightning` `OpenCV` `VideoMAE`

- **[Sudoku Solver CV Pipeline](https://github.com/00200200/sudoku-solver-computer-vision-cnn)**  
  End-to-end vision pipeline that extracts Sudoku grids from arbitrary camera images using OpenCV perspective transforms, classifies handwritten/printed digits with a PyTorch CNN, and solves the board via constraint satisfaction.  
  `PyTorch` `OpenCV` `CNN` `Python`

- **[GAN Architectures from Scratch](https://github.com/00200200/gan-architectures-from-scratch-pytorch)**  
  Clean implementations of Vanilla GAN, Deep Convolutional GAN (DCGAN), and Conditional GAN (cGAN) on MNIST, CIFAR-10, and Fashion-MNIST with PyTorch Lightning and Hydra configuration.  
  `PyTorch Lightning` `Hydra` `Computer Vision`

---

### Machine Learning & NLP Applications

- **[Emotube — Sentiment Analysis Platform](https://github.com/00200200/youtube-comment-sentiment-analyzer)**  
  Full-stack web application for real-time sentiment analysis and opinion mining across YouTube comment threads. Features interactive charting, automated categorization, and sentiment aggregation.  
  `FastAPI` `React` `PostgreSQL` `Hugging Face Transformers`

- **[Adaptive k for Dynamic Classifier Selection](https://github.com/00200200/complexity_adaptive_k_dynamic_classifier_selection)**  
  Empirical research studying the relationship between dataset complexity metrics and neighborhood size ($k$) in dynamic ensemble selection.  
  `scikit-learn` `DESlib` `Data Science`

- **[Local RAG + Reranker](https://github.com/00200200/ollama-rag-reranker)**  
  Lightweight retrieval-augmented generation CLI running fully locally. Uses Ollama embeddings with HNSW indexing and optional FlagEmbedding cross-encoder reranking.  
  `Python` `Ollama` `HNSW` `Vector Search`

- **[T5 Text Summarizer](https://github.com/00200200/t5-text-summarization-cnn-dailymail)**  
  Abstractive text summarization fine-tuning T5-small on CNN/DailyMail and XSum datasets with ROUGE metrics evaluation and Gradio interface.  
  `Transformers` `PyTorch` `Gradio`

---

### Developer Tooling & Systems

- **[Repro Lens](https://github.com/00200200/repro-lens)**  
  Static reproducibility checks and experiment verification for ML pipelines. Detects unseeded random generators, device non-determinism, and output drift across refactors without requiring heavy ML runtimes.  
  `Python` `AST` `Static Analysis` `pre-commit`

- **[UsageTrim](https://github.com/00200200/usagetrim)**  
  Local CLI and MCP tool for compacting verbose test and build output, with full output recoverable by reference.<br>
  `Python` `CLI` `MCP`

- **[Maintainer Skills Lab](https://github.com/00200200/maintainer-skills-lab)**  
  Maintainer workflows and agent profiles, shared from one source across Codex, Claude Code, Cursor, and other coding clients.<br>
  `Python` `Markdown` `Developer Tooling`
