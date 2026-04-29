# Index

本文件是知识库的总目录。上半部分由 LLM 手工维护（wiki 内容），下半部分由 Dataview 自动生成（raw 资料清单）。

---

## Wiki（手工维护）

### 主题（MOC 入口）
_暂无_

### 概念（单点知识）
_暂无_

### 实体（人 / 公司 / 产品 / 模型）
_暂无_

### 摘要（资料提炼）
_暂无_

### 对比（跨源比较分析）
_暂无_

### 问答（探索沉淀）
_暂无_

---

## Raw 资料清单（Dataview 自动生成）

```dataview
TABLE medium AS "载体", topics AS "主题", status AS "状态", ingested AS "吸收日期"
FROM "raw"
WHERE type = "source"
SORT ingested DESC
```

### 按主题聚合

```dataview
TABLE rows.file.link AS "资料"
FROM "raw"
WHERE type = "source"
FLATTEN topics AS topic
GROUP BY topic
```
