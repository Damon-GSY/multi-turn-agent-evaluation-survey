# Core ideas and findings

This guide summarizes Sections 1–5 of [the survey (arXiv v2)](https://arxiv.org/html/2503.22458v2). It is a reading companion to the paper.

## Why multi-turn evaluation needs its own framework

A conversational agent combines an LLM with tool use, memory, and planning. Its actions and responses depend on earlier exchanges, while user goals and the environment can change. A correct individual response does not establish that a whole conversation succeeded: errors can propagate, constraints can be forgotten, and a useful plan can become outdated.

![Multi-turn conversational agent example](../assets/figures/fig-01-agent-example.png)

## Two connected taxonomies

The survey connects **what to evaluate** with **how to evaluate**. The first organizes evaluation targets; the second organizes data construction, annotations, and evaluation methods.

![Overall evaluation taxonomy](../assets/figures/fig-03-evaluation-taxonomy.png)

### End-to-end experience

Evaluate whether the agent completes the user's tasks while maintaining coherent interaction and a satisfactory experience. The paper discusses task completion, multitask capabilities, recollection, expansion, refinement, follow-up, and safety across turns. Dialogue-level outcomes and the process of achieving them both matter.

### Action and tool use

The paper separates three concerns: mapping user intent to API calls, selecting and chaining tools through multiple steps, and ensuring reliability. Correct tool selection alone is insufficient if parameters are wrong, tool outputs are misinterpreted, or subsequent actions ignore earlier results. Evaluation should capture execution accuracy, efficiency, error recovery, and multi-turn coherence.

### Memory

Memory is organized along two axes:

| Axis | Categories | Main evaluation concerns |
| --- | --- | --- |
| Span | Turn, conversation, permanent | Accurate updates, recall, temporal continuity, and cross-session consistency |
| Textual form | Complete, recent, retrieved, external interactions | Coverage, context completeness, retrieval precision and recall, efficiency, and integration correctness |
| Parametric form | Fine-tuning, memory editing | Adaptability, update control, and generalization |

![Memory evaluation taxonomy](../assets/figures/fig-04-memory-taxonomy.png)

[Figure 5](figures.md#figure-5-memory-forms) illustrates the four interaction forms. Full-history retention, a recent context window, selective retrieval, and external information each create different evaluation trade-offs.

### Planning

Planning is treated as a continuing control loop. The four dimensions are:

1. **Task modeling:** represent goals, actions, constraints, and relevant context.
2. **Task decomposition:** split complex goals into executable steps with appropriate granularity and dependencies.
3. **Adaptation and control:** revise plans as the environment and user intentions change.
4. **Reflection:** verify feasibility and select plans during or after generation.

![Planner evaluation taxonomy](../assets/figures/fig-06-planner-taxonomy.png)

## How to evaluate

### Evaluation data

The data taxonomy separates **generation** from **annotation**. Both cover next-turn responses, tool use, query rewriting/retrieved information, and factual verification. These targets connect evaluation data to the actual decisions an agent makes across a conversation.

![Evaluation data taxonomy](../assets/figures/fig-07-evaluation-data.png)

### Evaluation metrics and judges

Annotation-based evaluation uses curated references or exact targets. Annotation-free evaluation includes scoring individual responses and comparing candidate responses. The survey also discusses agent-as-judge evaluation, which uses evidence from intermediate execution steps.

![Evaluation metrics taxonomy](../assets/figures/fig-08-evaluation-metrics.png)

Reference-based measures provide concrete targets but depend on annotation coverage. Annotation-free judges handle open-ended outputs more flexibly, while introducing reliability, bias, and cost concerns. See the [method comparison and scoring examples](evaluation-methods.md).

## Research evolution

The roadmap follows the development from rule-based conversational systems, through neural dialogue models, to LLM-based agents. Evaluation develops alongside those systems: from qualitative user assessments toward contextual metrics, human preferences, tool-use benchmarks, and automated judges.

![Roadmap of multi-turn conversational evaluation](../assets/figures/fig-10-roadmap.png)

## Open challenges and future directions

Section 4.2 identifies the following research directions. Related ethical discussion is consolidated here.

| Direction | Main issue |
| --- | --- |
| Unified and adaptive evaluation | Combine turn-level and conversation-level assessments while tracking changing context |
| Memory and context retention | Distinguish temporary recall from persistent integration over long interactions |
| Test-time self-assessment | Evaluate coherence, factual accuracy, and context alignment during response generation |
| Self-correction and error propagation | Detect and repair early errors before they compound across turns |
| Tool use and action planning | Assess cumulative tool execution and plan revision under changing inputs |
| Scalability and real-world applicability | Reduce annotation and computation costs while retaining realistic evaluation |
| Privacy preservation | Evaluate conversations while protecting sensitive interaction data |
| Philosophical and ethical dimensions | Address transparency, consent, accountability, and human-centered deployment |

## Main takeaway

Evaluate the whole conversation and the components that sustain it. Pair outcome measures with evidence about tool execution, memory, planning, and intermediate progress. The survey's contribution is the taxonomy and synthesis that connect these evaluation targets to data, metrics, and open research questions.

## Reading map

- [All 10 figures with original captions](figures.md)
- [Section-by-section taxonomy](taxonomy.md)
- [Evaluation method comparison (Table 1)](evaluation-methods.md)
- [Benchmark resource tables (Tables 2–3)](benchmarks.md)
- [Complete reference index](references.md)
- [Full paper PDF](../paper/2503.22458v2.pdf)

---
Adapted from Shengyue Guan, Jindong Wang, Jiang Bian, Bin Zhu, Jian-guang Lou, and Haoyi Xiong, *Evaluating LLM-based Agents for Multi-Turn Conversations: A Survey*, arXiv:2503.22458v2. Summaries and organization are adapted for this repository under [CC BY 4.0](../LICENSE).
