# Evaluation methods

Section 3.2 distinguishes annotation-based evaluation from annotation-free evaluation. The table below reproduces Table 1 in Markdown.

| Aspect | Annotation-based Evaluation | Annotation-free Evaluation |
| --- | --- | --- |
| Approach / Data | •<br>Relies on expert-annotated reference outputs<br>•<br>Uses fixed labels (e.g. annotated intents, entities) for exact matching. | •<br>Uses model-based metrics (e.g. LLM scoring of relevance, coherence).<br>•<br>Can perform direct, pairwise or listwise comparisons without gold labels. |
| Advantages | •<br>High Precision<br>: Ground-truth references ensure accurate scoring.<br>•<br>Interpretability<br>: Clear semantics of annotated labels guide evaluation. | •<br>Flexibility<br>: Adaptable to open-ended qualities without new data.<br>•<br>Automation<br>: Easily applies to new domains without annotation overhead. |
| Disadvantages | •<br>Costly & Slow<br>: Requires extensive human effort and time to produce ground truth label.<br>•<br>Bias<br>: Subject to annotator bias and low inter-annotator agreement. | •<br>Reliability & Bias Issues<br>: LLM evaluations can be inconsistent and biased.<br>•<br>Per-Query Cost<br>: API latency or usage costs for large LLM calls. |
| Flexibility & Coverage | •<br>Rigid<br>: Exact matching penalizes correct but unannotated responses.<br>•<br>Static<br>: Hard to cover new scenarios without fresh annotations. | •<br>Adaptive<br>: Can evaluate novel or broad cases via prompt design.<br>•<br>Broad Scope<br>: Judges subjective and multi-dimensional aspects dynamically. |

## Scoring and comparison

- **Point-wise:** assign a response a score under specified criteria, such as relevance, clarity, and coherence.
- **Pair-wise:** compare two responses directly, typically recording a win, loss, or tie.
- **List-wise:** rank several candidate responses together.
- **Agent-as-judge:** inspect intermediate execution information and retrieve evidence relevant to the evaluation criteria, extending evaluation beyond the final answer.

![Point-wise and pair-wise evaluation](../assets/figures/fig-09-pointwise-pairwise.png)

LLM judges offer scale and flexibility, but their reliability, bias, and per-query cost remain evaluation concerns. The paper emphasizes the value of intermediate milestones and dependencies when judging agent processes.

Source: [Section 3.2, arXiv v2](https://arxiv.org/html/2503.22458v2#S3.SS2). Adapted and reformatted under [CC BY 4.0](../LICENSE).
