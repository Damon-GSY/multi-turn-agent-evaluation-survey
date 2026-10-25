<p align="right"><strong>English</strong> · <a href="README.zh-CN.md">简体中文</a></p>

# Evaluating LLM-based Agents for Multi-Turn Conversations

### A Survey · ACM TIST 2026

**A map of what to evaluate—and how to evaluate it—when agents converse, remember, plan, and use tools across turns.**

Shengyue Guan · Jindong Wang · Jiang Bian · Bin Zhu · Jian-Guang Lou · Haoyi Xiong

[![ACM TIST](https://img.shields.io/badge/ACM_TIST-17%284%29_%C2%B7_2026-315C84?style=flat-square)](https://doi.org/10.1145/3793671)
[![arXiv](https://img.shields.io/badge/arXiv-2503.22458-B31B1B?style=flat-square)](https://arxiv.org/abs/2503.22458)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-65727E?style=flat-square)](LICENSE)

[**Read the paper ↗**](https://doi.org/10.1145/3793671) · [Core ideas](docs/key-insights.md) · [Benchmarks](docs/benchmarks.md) · [References](docs/references.md) · [Cite](#citation)

<p align="center">
  <img src="assets/readme/evaluation-map.svg" width="100%" alt="Multi-turn agent evaluation: follow the conversation across turns and assess experience, tool use, memory, and planning through data, metrics, and benchmarks.">
</p>

## Start here

This is the companion resource repository for **Evaluating LLM-based Agents for Multi-turn Conversations: A Survey**, published in *ACM Transactions on Intelligent Systems and Technology*, 17(4), 2026.

- **Understand the framework:** read the [core ideas and findings](docs/key-insights.md).
- **Find an evaluation resource:** browse the [benchmark tables](docs/benchmarks.md) and [method comparison](docs/evaluation-methods.md).
- **Explore the literature:** open the [267-entry reference index](docs/references.md), with linked paper titles.
- **Read the original material:** view [all 10 figures](docs/figures.md) or the [arXiv v2 PDF](paper/2503.22458v2.pdf).

## What to evaluate

A successful conversation depends on more than its last answer. The survey connects dialogue-level outcomes to three agent components: tools, memory, and planning.

| Evaluation target | Central question |
| --- | --- |
| **End-to-end experience** | Does the agent complete tasks while sustaining coherent, useful, and safe interaction? |
| **Action and tool use** | Does it select, chain, and interpret tools correctly across turns? |
| **Memory** | Does it retain and use information within turns, across a conversation, and between sessions? |
| **Planning** | Can it model goals, decompose tasks, adapt plans, and reflect on decisions? |

<details>
<summary><strong>View the full taxonomy from the paper · Figure 3</strong></summary>

![Original taxonomy of evaluation goals and methodologies](assets/figures/fig-03-evaluation-taxonomy.png)

[Open full-size figure](assets/figures/fig-03-evaluation-taxonomy.png) · [Section-by-section taxonomy](docs/taxonomy.md)

</details>

## How to evaluate

The second taxonomy connects **evaluation data** to **evaluation metrics**:

1. **Build the data.** Generate and annotate responses, tool calls, rewritten queries, retrieved information, and factual claims.
2. **Choose the method.** Use annotated references or exact targets, point-wise scoring, pair-wise/list-wise comparisons, and LLM or agent judges.
3. **Inspect the process.** Consider intermediate actions, memory use, and plan changes alongside final outcomes.

[Compare the methods →](docs/evaluation-methods.md) · [Explore benchmarks →](docs/benchmarks.md)

## Inside a multi-turn agent

![Paper Figure 1: a conversation coordinated through planning, tools, and memory](assets/figures/fig-01-agent-example.png)

The example illustrates how planning, tool execution, and memory support a conversation as the user's request develops. [Original caption and source](docs/figures.md#figure-1-agent-example).

## Research directions

The survey highlights adaptive evaluation across turns, long-term memory benchmarks, test-time self-assessment, error correction, cumulative tool use, scalable evaluation, privacy, and ethical accountability.

<details>
<summary><strong>View the evolution of conversation systems and evaluation · Figure 10</strong></summary>

![Roadmap of conversational systems and their evaluation methods](assets/figures/fig-10-roadmap.png)

[Full roadmap and caption](docs/figures.md#figure-10-roadmap)

</details>

[Read the challenges and future directions →](docs/key-insights.md#open-challenges-and-future-directions)

## Citation

Please cite the published ACM TIST article. [DOI](https://doi.org/10.1145/3793671) · [BibTeX file](citation.bib)

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

## Version, contributions, and license

The resource collection follows **arXiv v2 (January 5, 2026)**; the citation points to the published ACM article. The PDF and extracted figures retain the arXiv v2 content. The [reference index notes](docs/references.md#link-notes) explain the two historical sources linked through a book page or author bibliography.

Suggestions and corrections are welcome through issues and pull requests. See [Contributing](CONTRIBUTING.md).

Documentation and adapted arXiv material use [CC BY 4.0](LICENSE). The opening map is a simplified repository illustration of the survey taxonomy; numbered figures are reproduced from the paper. Linked resources retain their own licenses.
