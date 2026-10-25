# Benchmark datasets and resources

Tables transcribed from Section 3.3 of the paper. Study labels link to their bibliography entries in the source. Descriptions and metrics retain the paper’s wording.


## Multitask Capabilities

| Study | Focus | Metrics |
| --- | --- | --- |
| [Hendrycks et al. (2020)](https://arxiv.org/html/2503.22458v2#bib.bib8) | Domain-Specific Multitasking | Accuracy in domain-specific question answering and problem-solving |
| [Li et al. (2017)](https://arxiv.org/html/2503.22458v2#bib.bib131) | Manually Annotated Multi-Turn Data (DailyDialog) | Annotation quality, response coherence |
| [Gopalakrishnan et al. (2019)](https://arxiv.org/html/2503.22458v2#bib.bib132) | Topic-Based Dialogue Dataset (Topical Chat) | Knowledge grounding, conversational diversity |

## Interaction Patterns in Multi-Turn Conversations

| Study | Focus | Metrics |
| --- | --- | --- |
| [Zheng et al. (2023)](https://arxiv.org/html/2503.22458v2#bib.bib9) | Multi-Turn Benchmark (MT-Bench) | Precision, quality of generated responses |
| [Kwan et al. (2024)](https://arxiv.org/html/2503.22458v2#bib.bib12) | Human-LLM Interaction Patterns | Recognition of multi-turn patterns, task success rates |

## Temporal Dimensions in Multi-Turn Conversations

| Study | Focus | Metrics |
| --- | --- | --- |
| [Xu et al. (2022b)](https://arxiv.org/html/2503.22458v2#bib.bib14) | Long-Term Conversations Dataset | Retention of shared context over sessions |
| [Maharana et al. (2024)](https://arxiv.org/html/2503.22458v2#bib.bib16) | Months-Long Conversations Dataset | Context retention in multi-month interactions |

## Safety in Multi-Turn Conversations

| Study | Focus | Metrics |
| --- | --- | --- |
| [Yu et al. (2024)](https://arxiv.org/html/2503.22458v2#bib.bib19) | Safety: Coreference-Based Attacks | Vulnerability to coreference-based attacks |

## Tool-Use Benchmarks

| Study | Focus | Metrics |
| --- | --- | --- |
| [Mialon et al. (2024)](https://arxiv.org/html/2503.22458v2#bib.bib258) | real word question that is easy for human but hard for AI (GAIA benchmark) | Performance is gauged by the percentage of exact-match. |
| [Huang et al. (2024d)](https://arxiv.org/html/2503.22458v2#bib.bib212) | Tool Awareness & Decision-Making | Correct tool selection rate, effective usage in single-/multi-tool tasks |
| [Wang et al. (2024f)](https://arxiv.org/html/2503.22458v2#bib.bib29) | Multi-Turn Tool-Use in Python | Successful integration & execution of Python-based tools |
| [Xu et al. (2023)](https://arxiv.org/html/2503.22458v2#bib.bib24) | API Call Execution (ToolBench) | Function call success rate |
| [Shim et al. (2025)](https://arxiv.org/html/2503.22458v2#bib.bib128) | ToolDial benchmark | Annotation efficiency, action prediction |
| [Shen et al. (2023)](https://arxiv.org/html/2503.22458v2#bib.bib25) | Orchestrated Tool-Use (HuggingGPT) | Task execution accuracy |
| [Li et al. (2023c)](https://arxiv.org/html/2503.22458v2#bib.bib201) | API Benchmarking | Context retention, API success rate |
| [Wang et al. (2024e)](https://arxiv.org/html/2503.22458v2#bib.bib27) | Multi-Granularity Tool-Use (MTU-Bench) | Tool selection, parameter accuracy |

## Reliability and Hallucination Mitigation in Tool-Use

| Study | Focus | Metrics |
| --- | --- | --- |
| [Zhang et al. (2024f)](https://arxiv.org/html/2503.22458v2#bib.bib31) | Multi-Level Hallucination Diagnosis | Hallucination detection accuracy, depth and breadth analysis |

## Next-Turn Response

| Study | Focus | Metrics |
| --- | --- | --- |
| [Moniri et al. (2024)](https://arxiv.org/html/2503.22458v2#bib.bib127) | Multi-Round Structured Debates | Clarity, factual accuracy, consistency |
| [Abercrombie and Batista-Navarro (2020a)](https://arxiv.org/html/2503.22458v2#bib.bib125) | Parliamentary Debate Analysis | Logical flow, structured reasoning |

## Query Rewritten and Retrieved Items

| Study | Focus | Metrics |
| --- | --- | --- |
| [Aliannejadi et al. (2020)](https://arxiv.org/html/2503.22458v2#bib.bib117) | Relevant Utterance Dataset | Precision, Recall and F1-score |

## Conversation Memory

| Study | Focus | Metrics |
| --- | --- | --- |
| [Chen et al. (2024a)](https://arxiv.org/html/2503.22458v2#bib.bib204) | Conversational Memory Benchmark | Keyword recall, memory retention over multiple turns |

## Complete Interaction

| Study | Focus | Metrics |
| --- | --- | --- |
| [Li et al. (2023a)](https://arxiv.org/html/2503.22458v2#bib.bib45) | Long-Range Context Retrieval | Long-context recall, retrieval accuracy |
| [Maharana et al. (2024)](https://arxiv.org/html/2503.22458v2#bib.bib16) | Long-Term Multi-Agent Conversations | Memory retention, coherence in extended dialogues |

## Task Representation

| Study | Focus | Metrics |
| --- | --- | --- |
| [Zhang et al. (2024d)](https://arxiv.org/html/2503.22458v2#bib.bib76) | Language Model-Driven PDDL Planning | Planning efficiency, generalization across tasks |

## Context Modeling

| Study | Focus | Metrics |
| --- | --- | --- |
| [Xiao et al. (2024)](https://arxiv.org/html/2503.22458v2#bib.bib211) | Reducing Context Hallucinations | Hallucination reduction, response precision |

## Task Decomposition

| Study | Focus | Metrics |
| --- | --- | --- |
| [Wang et al. (2024h)](https://arxiv.org/html/2503.22458v2#bib.bib82) | Multi-Agent Task Decomposition | Adaptability, task efficiency |
| [Wu et al. (2024b)](https://arxiv.org/html/2503.22458v2#bib.bib91) | Multi-Level Task Planning | Task decomposition accuracy |

## Post-Generation Plan Selection

| Study | Focus | Metrics |
| --- | --- | --- |
| [Kargupta et al. (2024)](https://arxiv.org/html/2503.22458v2#bib.bib200) | Structured Questioning | Plan consistency, dialogue coherence |


---
Source: [Guan et al., arXiv:2503.22458v2](https://arxiv.org/html/2503.22458v2), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). This page reorganizes material from the paper.
