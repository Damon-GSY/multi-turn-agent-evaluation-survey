# Evaluating LLM-based Agents for Multi-Turn Conversations: A Survey

[![arXiv](https://img.shields.io/badge/arXiv-2503.22458-b31b1b.svg)](https://arxiv.org/abs/2503.22458)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**The companion resource repository for our survey on evaluating LLM-based multi-turn conversational agents.**

Shengyue Guan, Jindong Wang, Jiang Bian, Bin Zhu, Jian-guang Lou, Haoyi Xiong

[Paper](https://arxiv.org/abs/2503.22458) · [PDF](https://arxiv.org/pdf/2503.22458) · [中文说明](README.zh-CN.md) · [Taxonomy](docs/taxonomy.md) · [Benchmarks](docs/benchmarks.md) · [References](docs/references.md)

## Overview

A useful conversational agent must carry information, decisions, and actions across turns. This survey organizes evaluation around two connected questions: **what to evaluate** and **how to evaluate**.

| What to evaluate | Focus |
| --- | --- |
| End-to-end experience | Task completion, interaction patterns, user experience, and safety |
| Action and tool use | API interaction, multi-step tool selection, and reliability |
| Memory | Turn, conversation, and permanent memory; memory representations |
| Planning | Task modeling, decomposition, adaptation, control, and reflection |

Evaluation methods cover data generation and annotation, reference-based metrics, annotation-free evaluation, and LLM-based judges. See the [taxonomy guide](docs/taxonomy.md) for the paper's section structure.

## Explore the resources

- [Benchmark tables](docs/benchmarks.md): the studies, evaluation targets, and metrics listed in Section 3.3.
- [Complete reference index](docs/references.md): all 267 bibliography entries extracted from the arXiv v2 HTML, with available external links.
- [Contributing](CONTRIBUTING.md): suggest corrections and relevant resources through issues or pull requests.

## Version

The repository's initial resource snapshot follows **arXiv v2, January 5, 2026**. The benchmark tables and reference index preserve that snapshot; additions should identify their source and distinguish later work.

## Citation

```bibtex
@misc{guan2026evaluatingllmbasedagentsmultiturn,
  title={Evaluating LLM-based Agents for Multi-Turn Conversations: A Survey},
  author={Shengyue Guan and Jindong Wang and Jiang Bian and Bin Zhu and Jian-guang Lou and Haoyi Xiong},
  year={2026},
  eprint={2503.22458},
  archivePrefix={arXiv},
  primaryClass={cs.CL},
  url={https://arxiv.org/abs/2503.22458}
}
```

## License

Documentation and material adapted from the paper are available under [CC BY 4.0](LICENSE). Linked papers, datasets, and software retain their respective licenses.
