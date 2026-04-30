# Glanstia_System-skill
使用大模型对自然语言进行蒸馏，获取"数字灵魂“并应用的项目。
“数字灵魂”在这里是一个诗意且前瞻的概念：它不是简单向量嵌入，而是融合了语义本质、行为模式、知识人格的结构化表示，可被 Agent 像召唤实体一样注入使用，理论上能突破单次对话的上下文限制，实现更持久的 AI 个性/能力传承。

本系统应用了GNO项目的能力增强召回，这可能不是最合适的方式，但应该是最方便的

## 使用说明
将以下命令发送给AI agent"根据以下项目（https://github.com/NoxTyrannus/Glanstia_System-skill）获取文件，解压缩后学会这个skill并告诉我如何使用"

skill内的搜索能力是基于metaso实现的，可以命令agent替换成自己已有的搜索skill或者mcp

## 项目亮点
1将“灵魂转生”式的叙事与 LLM 蒸馏结合，超越传统 RAG（检索增强生成）或提示工程，尝试构建“数字人格持久化”机制。这在 2026 年 Agent 生态中属于前沿探索，尤其适合叙事驱动、角色扮演或长期记忆型 AI 应用。
与类似项目对比：类似 AutoGPT 的 Skill 市场、LangChain 的 Memory 模块、Claude 的 Tool/Artifact，但本项目更强调“人格级蒸馏”而非工具级功能，具有强烈的实验性炼金色彩。
局限：概念抽象，“数字灵魂”尚未给出可量化的定义（是向量数据库？状态机？提示模板？），缺乏可复现示例，容易被视为 hype。

## 核心流程
数据输入 → LLM 蒸馏 → 数字灵魂提取 → subagent 召唤（soul_summon） → GNO 能力增强召回 → Metaso 搜索辅助 → Skill 应用。
依赖：
必须具备 subagent / 多代理能力（理论上任何支持类似机制的 Agent 产品均可）。
搜索层基于 Metaso（可被用户指令替换为自有搜索 Skill 或 MCP）。
GNO 项目能力增强召回（外部/小众依赖，未公开细节）。

PS：skill需要依赖subagent能力实现soul_summon,所以理论上具备subagent或近似能力的agent产品都可以使用。
