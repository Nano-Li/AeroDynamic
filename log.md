# Log

知识库的时间线，仅记录三类事件：`ingest`（吸收新资料）、`query`（产出新分析或问答）、`lint`（健康检查）。

条目格式：`## [YYYY-MM-DD] <type> | <short title>`，便于 `grep "^## \[" log.md` 解析。

---

## [2026-04-28] init | 知识库初始化
- 基于 [[llm-wiki.md]] 的方法论，搭建三层架构（raw / wiki / schema）
- 创建文件夹结构：`raw/{书籍, 论文, 媒体, 网页, assets}`、`wiki/{主题, 概念, 实体, 摘要, 对比, 问答}`
- 写入 [[CLAUDE.md]] 维护手册，覆盖 YAML 规范、简记纪律、命名规则、三类工作流、输出语言策略
- 写入 [[index.md]]（wiki 手工 + raw Dataview 自动）和 [[log.md]]
