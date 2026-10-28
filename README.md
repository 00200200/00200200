# Michał Furgała

I hold a BEng in Computer Engineering from Wrocław University of Science and Technology.

My research interests are counterfactual explanations, concept-based models, generative models, and LLM interpretability. I am a member of the ML team at Solvro, a student research club at Wrocław University of Science and Technology.

Here you'll find my ML experiments, developer tools, and contributions to Python, Go, Rust, and JavaScript projects.

[Original projects](https://github.com/00200200?tab=repositories&type=source) · [Merged contributions](https://github.com/pulls?q=is%3Apr+author%3A00200200+is%3Amerged+-user%3A00200200)

---

## Open-source contributions

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
| **set-cookie-parser** | JavaScript | Ignore invalid `Expires` attributes to retain valid expiry dates | [#91](https://github.com/nfriedly/set-cookie-parser/pull/91) |

My DuckDB fix for `overwrite=False` was submitted in [#642](https://github.com/duckdb/duckdb-python/pull/642) and incorporated by a maintainer in the merged [#668](https://github.com/duckdb/duckdb-python/pull/668).

---

## Projects

### Developer tools

- [UsageTrim](https://github.com/00200200/usagetrim): a local CLI and MCP tool that compacts test and build output, with cached text retrievable after recognized secrets are redacted.
- [Maintainer Skills Lab](https://github.com/00200200/maintainer-skills-lab): shared maintainer workflows and agent profiles for coding assistants.
- [Repro Lens](https://github.com/00200200/repro-lens): static reproducibility checks and experiment verification for ML pipelines.

### Computer vision

- [Video Waste Dumping Detection (IWDD)](https://github.com/00200200/Video-Waste-Dumping-Detection---IWDD): video classification with VideoMAE and X-CLIP for the IWDD competition.

- [Sudoku Solver](https://github.com/00200200/sudoku-solver-computer-vision-cnn): grid extraction with OpenCV, digit recognition with a PyTorch CNN, and a backtracking solver.

- [GAN Architectures from Scratch](https://github.com/00200200/gan-architectures-from-scratch-pytorch): Vanilla GAN, DCGAN, and conditional GAN implementations using PyTorch Lightning and Hydra.

---

### Machine learning and NLP

- [YouTube Comment Sentiment Analyzer](https://github.com/00200200/youtube-comment-sentiment-analyzer): a FastAPI and React app for analyzing comment sentiment with Hugging Face models.

- [Adaptive k for Dynamic Classifier Selection](https://github.com/00200200/complexity_adaptive_k_dynamic_classifier_selection): experiments on dataset complexity and neighborhood size in dynamic classifier selection.

- [Local RAG + Reranker](https://github.com/00200200/ollama-rag-reranker): a retrieval CLI using Ollama embeddings, HNSW indexing, and optional cross-encoder reranking.

- [T5 Text Summarizer](https://github.com/00200200/t5-text-summarization-cnn-dailymail): T5-small fine-tuning on CNN/DailyMail and XSum, with ROUGE evaluation and a Gradio interface.
