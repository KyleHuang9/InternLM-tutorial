# 书生·浦语大模型全链路开源开放体系

### 课程资料

第一次课程视频链接：[https://www.bilibili.com/video/BV1Rc411b7ns/](https://www.bilibili.com/video/BV1Rc411b7ns/)

## 为什么大模型？

大模型成为发展通用人工智能的重要途经，展现出更高阶智能的可能性。书生·浦语大模型系列在这方面发挥关键作用。

## 书生·浦语大模型系列
- 轻量级: InternLM-7B(已开源)
- 中量级: InternLM-20B(已开源)
- 重量级: InternLM-123B
- 领先于目前相近量级开源模型(包括Llama-33B, Llama2-13B)，其中 InternLM-20B 达到 Llama2-70B 的水平。

## 应用方向
可能的应用方向包括智能客服、个人助手、行业应用等。应用过程涉及书生·浦语开源工具，包括模型选型、应用数据(书生·万卷)、文本、图像、图像-文本、价值观对齐、全参数/部分参数微调(lora算法)(XTuner)、模型评测(OpenCompass)、模型部署(LMDeploy)以及智能体交互(Lagent, AgentLego)。

## 书生·万卷数据
- 文本数据：50亿数据，总数据量超1TB
- 图像-文本数据集：超2,200万个文件，数据量超140GB
- 视频数据：超1,000个文件，数据量超900GB
- 总数据量：2TB
- 发布日期：2023年7月14日
- 更多数据：[OpenDataLab](https://opendatalab.com)

## InternLM-Train (预训练)
- 高度可扩展：支持从8卡到千卡训练，千卡加速效率达92%
- 极致性能优化：Hybrid Zero独特技术 + 极致优化，加速50%
- 兼容主流：无缝衔接HuggingFace等技术生态，支持各类轻量化技术
- 开箱即用：支持多种规格语言模型，修改配置即可训练。

## XTuner (微调)
- 增量续训
  - 使用场景：让基座模型学习到一些新知识，如某个垂类领域知识；
  - 训练数据：文章、书籍、代码等。
- 有监督微调
  - 使用场景：让模型学会理解和遵循各类指令，或者注入少量领域知识；
  - 训练数据：高质量的对话、问答数据。
- 适配多种生态
  - 多种微调算法：多种微调策略与算法，覆盖各类SFT场景；
  - 适配多种开源生态：支持加载HuggingFace、ModelScope模型或数据集；
  - 自动优化加速：开发者无需关注复杂的显存优化与计算加速细节；
- 适配多种硬件
  - 训练方法覆盖NVIDIA 20系以上所有显卡；
  - 最低只需8GB显存即可微调7B模型。

## OpenCompass (评测)
全球领先的大模型开源评测体系：6大维度，80+评测集，40万+评测题目
- 丰富模型支持：开源模型、API模型一站式评测；
- 分布式高效评测：支持千亿参数模型在海量数据集上分布式评测；
- 便捷的数据集接口：支持社区用户根据自身需求快速添加自定义数据集；
- 敏捷的能力迭代：每周更新大模型能力榜单，每月提升评测工具能力。

## LMDeploy (部署)
- 高效推理引擎
  - 持续批处理技巧
  - 深度优化的低比特计算kernel
  - 模型并行
  - 高效的k/v缓存管理机制
- 完善易用的工具链
  - 量化、推理、服务全流程
  - 无缝衔接OpenCompass评测推理精度
  - 和OpenAI接口高度兼容的API server

## Lagent Agentlego (应用)
- LLM的局限性：
  - 最新信息和知识的获取
  - 回复的可靠性
  - 数学计算
  - 工具使用和交互
- Lagent：搭建智能体框架
  - 支持多种类型的智能体能力
  - 灵活支持多种大语言模型
  - 简单易拓展，支持丰富的工具
- AgentLego：多模态智能体工具箱
  - 丰富的工具集合，尤其是提供了大量视觉、多模态相关领域的前沿算法功能
  - 支持多个主流智能体系统，如LangChain, Transformers Agent, Lagent等
  - 灵活的多模态工具调用接口，可以轻松支持各类输入输出格式的工具函数
  - 一键式远程工具部署，轻松使用和调试大模型智能体
