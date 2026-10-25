# 大语言模型多轮对话智能体评测综述

[English](README.md) · [论文](https://arxiv.org/abs/2503.22458) · [PDF](https://arxiv.org/pdf/2503.22458)

本仓库是 **Evaluating LLM-based Agents for Multi-Turn Conversations: A Survey** 的配套资料仓库。

作者：Shengyue Guan、Jindong Wang、Jiang Bian、Bin Zhu、Jian-guang Lou、Haoyi Xiong。

## 从哪里开始

论文围绕两个问题组织多轮对话智能体评测：**评什么**与**怎么评**。

| 评测对象 | 主要关注点 |
| --- | --- |
| 端到端体验 | 任务完成、交互模式、用户体验与安全 |
| 动作与工具使用 | API 交互、多步骤工具选择、可靠性与幻觉 |
| 记忆 | 单轮、会话和持久记忆，以及记忆表示形式 |
| 规划 | 任务建模、任务分解、适应与控制、反思 |

评测方法涵盖对话数据生成与标注、依赖参考答案的指标、无标注评测，以及大模型裁判。

## 资料导航

- [分类导读](docs/taxonomy.md)：对应论文第二、三章的结构。
- [基准与资源表](docs/benchmarks.md)：整理论文第三章的研究、评测目标与指标。
- [完整参考文献](docs/references.md)：从 arXiv v2 HTML 提取的 267 条文献及可用外部链接。
- [参与贡献](CONTRIBUTING.md)：通过 Issue 或 Pull Request 提交勘误和资源建议。

初始资料版本对应 **2026 年 1 月 5 日发布的 arXiv v2**。引用格式见 [英文 README](README.md#citation)。文档及论文改编内容采用 [CC BY 4.0](LICENSE)；所链接资源遵循各自许可。
