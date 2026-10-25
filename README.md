# Evaluating LLM-based Agents for Multi-Turn Conversations: A Survey

[![DOI](https://img.shields.io/badge/DOI-10.1145%2F3793671-blue)](https://doi.org/10.1145/3793671)
[![arXiv](https://img.shields.io/badge/arXiv-2503.22458-b31b1b.svg)](https://arxiv.org/abs/2503.22458)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**The companion resource repository for our survey on evaluating LLM-based multi-turn conversational agents.**

Shengyue Guan, Jindong Wang, Jiang Bian, Bin Zhu, Jian-guang Lou, Haoyi Xiong

[ACM paper](https://doi.org/10.1145/3793671) · [arXiv](https://arxiv.org/abs/2503.22458) · [PDF](https://arxiv.org/pdf/2503.22458) · [中文说明](README.zh-CN.md) · [Taxonomy](docs/taxonomy.md) · [Benchmarks](docs/benchmarks.md) · [References](docs/references.md)

## Overview

A useful conversational agent must carry information, decisions, and actions across turns. This survey organizes evaluation around two connected questions: **what to evaluate** and **how to evaluate**.

| What to evaluate | Focus |
| --- | --- |
| End-to-end experience | Task completion, interaction patterns, user experience, and safety |
| Action and tool use | API interaction, multi-step tool selection, and reliability |
| Memory | Turn, conversation, and permanent memory; memory representations |
| Planning | Task modeling, decomposition, adaptation, control, and reflection |

Evaluation methods cover data generation and annotation, reference-based metrics, annotation-free evaluation, and LLM-based judges. See the [taxonomy guide](docs/taxonomy.md) for the paper's section structure.

## The framework at a glance

![Taxonomy of evaluation approaches for multi-turn conversational agents](assets/figures/fig-03-evaluation-taxonomy.png)

The taxonomy links agent capabilities to evaluation data and metrics. Read the [core ideas and findings](docs/key-insights.md) for a guided explanation of tool use, memory, planning, evaluation methods, and future directions.

## Agent example

![An example of a multi-turn conversational agent](assets/figures/fig-01-agent-example.png)

## Evaluation roadmap

![Roadmap of multi-turn conversational evaluation](assets/figures/fig-10-roadmap.png)

Figures are reproduced from the paper under [CC BY 4.0](LICENSE). See [all 10 figures and their original captions](docs/figures.md).

## Explore the resources

- [Core ideas and findings](docs/key-insights.md): the paper's main contributions, evaluation dimensions, and open challenges.
- [Figure gallery](docs/figures.md): all 10 figures, including memory, planning, data, and metrics taxonomies.
- [Evaluation methods](docs/evaluation-methods.md): Table 1 and point-wise/pair-wise evaluation.
- [Full paper PDF](paper/2503.22458v2.pdf): a local copy of arXiv v2.


- [Benchmark tables](docs/benchmarks.md): the studies, evaluation targets, and metrics listed in Section 3.3.
- [Complete reference index](docs/references.md): all 267 bibliography entries extracted from the arXiv v2 HTML, with linked titles and direct paper URLs (publisher/author records for the two historical reprints or legacy sources).
- [Contributing](CONTRIBUTING.md): suggest corrections and relevant resources through issues or pull requests.

## Version

The published journal article is available at [ACM, DOI: 10.1145/3793671](https://doi.org/10.1145/3793671).

The repository's initial resource snapshot follows **arXiv v2, January 5, 2026**. The benchmark tables and reference index preserve that snapshot; additions should identify their source and distinguish later work.

## Citation

Published in **ACM Transactions on Intelligent Systems and Technology (TIST), 17(4), 2026**. Please cite the published journal article below. [ACM / DOI](https://doi.org/10.1145/3793671) · [Download BibTeX](citation.bib)


```bibtex
@article{guan2026evaluating,
  title = {Evaluating {LLM}-based Agents for Multi-turn Conversations: A Survey},
  author = {Guan, Shengyue and Wang, Jindong and Bian, Jiang and Zhu, Bin and Lou, Jian-Guang and Xiong, Haoyi},
  journal = {ACM Transactions on Intelligent Systems and Technology},
  volume = {17},
  number = {4},
  pages = {1--40},
  year = {2026},
  month = apr,
  publisher = {Association for Computing Machinery},
  doi = {10.1145/3793671},
  url = {https://doi.org/10.1145/3793671}
}
```

## License

Documentation and material adapted from the paper are available under [CC BY 4.0](LICENSE). Linked papers, datasets, and software retain their respective licenses.
