# Hi, I'm Michał

I build developer tools for AI agents, context optimization, and machine learning reproducibility.
My work spans AI token optimization, agent harnesses, local RAG, computer vision, and NLP.

[All repositories](https://github.com/00200200?tab=repositories)

## Selected merged contributions

Alongside my own projects, I contribute fixes to upstream open-source libraries.
These pull requests have been merged:

| Project | Change | Pull request |
| --- | --- | --- |
| AnyIO | Skip empty object-stream messages when receiving buffered bytes. | [#1409](https://github.com/agronholm/anyio/pull/1409) |
| serde_json | Report invalid UTF-8 at the first bad byte rather than the end of the string. | [#1345](https://github.com/serde-rs/json/pull/1345) |
| redis-py | Preserve zero-valued GEOSEARCH arguments instead of silently dropping them. | [#4356](https://github.com/redis/redis-py/pull/4356) |
| Fiber | Let empty optional route parameters yield to later required segments. | [#4722](https://github.com/gofiber/fiber/pull/4722) |

---

## Featured projects

### [UsageTrim](https://github.com/00200200/usagetrim)

<a href="https://github.com/00200200/usagetrim">
  <picture>
    <source media="(prefers-reduced-motion: reduce)" srcset="https://raw.githubusercontent.com/00200200/usagetrim/main/assets/readme-hero.png">
    <img src="https://raw.githubusercontent.com/00200200/usagetrim/main/assets/readme-hero.gif" width="100%" alt="UsageTrim: keep the signal, cut the noise. Authored fixtures cut docker 18,360→107, cargo 3,795→185, pytest 1,562→174.">
  </picture>
</a>

**Keep the signal. Cut the noise.** Local CLI + MCP that folds verbose tool output for Claude Code, Codex, Cursor, and Claude Desktop — recoverable by reference.

- Losslessly compacts other MCP servers' output (JSON rows → TSV, unescaped wrappers): −18.3% on 11,058 real results.
- Folds passing tests, build progress, runner setup, and bulky JSON while keeping failures, assertions, and stack traces verbatim.
- Every cut is recoverable: the original stays in a local cache behind a `usagetrim retrieve <ref>` id. No model calls, nothing leaves the machine.
- Specialized filters for pytest, cargo, go, vitest, eslint, tsc, mypy, Docker, kubectl, terraform, `gh` JSON, and GitHub Actions logs.
- Lean MCP profiles (9–11 tools, 36–38% smaller schemas), targeted symbol reads, session dedup, and a `gain` report of local estimates.
- Optional native macOS pet showing remaining Codex/Claude allowance.

```sh
# inside Claude Code
/plugin marketplace add 00200200/usagetrim
/plugin install usagetrim@usagetrim
```

`Python` `Swift` `MCP` `Claude Code` `Codex` `Cursor` `Claude Desktop` `Context Engineering`

[Website](https://00200200.github.io/usagetrim/) · [Repository](https://github.com/00200200/usagetrim) · [Install](https://github.com/00200200/usagetrim#install) · [Demo](https://github.com/00200200/usagetrim#see-it-cut) · [Connect your agent](https://github.com/00200200/usagetrim#connect-your-agent) · [Guide](https://github.com/00200200/usagetrim/blob/main/docs/guide.md)

### [Repro Lens](https://github.com/00200200/repro-lens)

**Check whether a refactor or a coding agent's edit changed your experiment outputs.**

- Screen selected reproducibility risks in scikit-learn, XGBoost, LightGBM, PyTorch, TensorFlow and Lightning, plus Python and NumPy RNGs. Static checks need no ML dependencies.
- Replay an experiment twice, then compare saved reports before and after an edit. Retain metrics, artifact hashes, commands and logs.
- Use the CLI, pre-commit hook, or reproducibility skill for coding agents.

`Python` `ML reproducibility` `AST` `pre-commit`

[Quick demo — no ML dependencies](https://github.com/00200200/repro-lens/tree/main/examples/agent_review) · [XGBoost training example — CPU](https://github.com/00200200/repro-lens/tree/main/examples/xgboost_review) · [Quickstart](https://github.com/00200200/repro-lens/blob/main/docs/quickstart.md)

The XGBoost example trains on a small synthetic dataset, accepts a refactor that preserves outputs, and reports changed outputs after reducing tree depth.

### [Ollama RAG + Reranker](https://github.com/00200200/ollama-rag-reranker)

Local retrieval-augmented generation with Ollama embeddings, HNSW vector search, and optional FlagEmbedding reranking.
The interactive CLI lets you compare answers with and without reranking.

`Python` `Ollama` `HNSW` `FlagEmbedding` `uv`

### [Maintainer Skills Lab](https://github.com/00200200/maintainer-skills-lab)

Shared skills, agent profiles and opt-in Git hooks for writing, debugging, PR review and releases.
Generated versions support Codex, Claude Code, Cursor and OpenCode; Grok Bot uses manual setup.
Start with Humanizer to edit a draft, or Skill Watch to track documentation changes and identify instructions needing review.

`Python` `Markdown` `Skills` `Git hooks`

[Humanizer skill](https://github.com/00200200/maintainer-skills-lab/blob/main/skills/mkl-humanize/SKILL.md) · [Browse the workflows](https://github.com/00200200/maintainer-skills-lab/blob/main/providers/README.md) · [Skill Watch demo](https://github.com/00200200/maintainer-skills-lab/tree/main/examples/skill-watch)

## More ML projects

- **[Video Waste Dumping Detection](https://github.com/00200200/Video-Waste-Dumping-Detection---IWDD)** — Video classification for the IWDD contest, with VideoMAE and X-CLIP training configurations. `PyTorch` `Lightning`

- **[Sudoku Solver](https://github.com/00200200/sudoku-solver-computer-vision-cnn)** — Grid extraction, digit recognition, and backtracking to solve Sudoku from images. `PyTorch` `OpenCV`

- **[Adaptive k for Classifier Selection](https://github.com/00200200/complexity_adaptive_k_dynamic_classifier_selection)** — How dataset complexity relates to neighborhood size in dynamic classifier selection. `scikit-learn` `DESlib`

- **[GANs from Scratch](https://github.com/00200200/gan-architectures-from-scratch-pytorch)** — Vanilla GAN, DCGAN, and Conditional GAN on MNIST, CIFAR-10, and Fashion-MNIST. `PyTorch Lightning` `Hydra`

- **[T5 Text Summarizer](https://github.com/00200200/t5-text-summarization-cnn-dailymail)** — T5-small fine-tuning on CNN/DailyMail and XSum, with ROUGE evaluation and a demo UI. `Transformers` `Gradio`

- **[Emotube](https://github.com/00200200/youtube-comment-sentiment-analyzer)** — YouTube comment sentiment analysis with filtering and interactive charts. `FastAPI` `React` `PostgreSQL`

<details>
<summary>Project screenshots and sample outputs</summary>

#### Ollama RAG: interactive CLI

<img src="https://raw.githubusercontent.com/00200200/ollama-rag-reranker/master/assets/cli.png" alt="Ollama RAG terminal menu with question, retrieval, and reranking options" width="342" />

#### Sudoku: solved puzzle

<img src="https://raw.githubusercontent.com/00200200/sudoku-solver-computer-vision-cnn/main/results/pipeline_outputs/20250605_113638_solved.jpg" alt="Detected Sudoku grid with the computed solution overlaid" width="640" />

#### DCGAN: generated CIFAR-10 samples

<img src="https://raw.githubusercontent.com/00200200/gan-architectures-from-scratch-pytorch/main/results/dcgan/epoch_90.png" alt="Grid of CIFAR-10 samples generated by DCGAN at epoch 90" width="274" />

#### T5: summarization interface

<img src="https://raw.githubusercontent.com/00200200/t5-text-summarization-cnn-dailymail/main/docs/app_gui.png" alt="Gradio interface for comparing T5 text summaries" width="640" />

#### Emotube: application home page

<img src="https://raw.githubusercontent.com/00200200/youtube-comment-sentiment-analyzer/main/readme_photos/ui_home.png" alt="Emotube home page for starting YouTube comment analysis" width="640" />

</details>

<details>
<summary>GitHub activity</summary>

[![Profile views](https://komarev.com/ghpvc/?username=00200200&label=Profile%20Views&color=6366F1&style=flat)](https://github.com/00200200)
[![GitHub followers](https://img.shields.io/github/followers/00200200?label=Followers&style=flat&color=6366F1)](https://github.com/00200200?tab=followers)
[![GitHub stars](https://img.shields.io/github/stars/00200200?label=Stars&style=flat&color=6366F1)](https://github.com/00200200?tab=repositories)

<img src="https://streak-stats.demolab.com?user=00200200&amp;theme=tokyonight&amp;hide_border=true&amp;border_radius=10&amp;background=0D1117&amp;stroke=6366F1&amp;ring=6366F1&amp;fire=FF6B6B&amp;currStreakLabel=6366F1" alt="GitHub contribution streak statistics for 00200200" width="495" />

<img src="https://raw.githubusercontent.com/00200200/00200200/output/snake.svg" alt="Snake animation of the GitHub contribution graph" width="880" />

</details>
