<!-- BADGE BAR -->
[![License](https://img.shields.io/badge/license-MIT-blue)](./LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-orange)](https://claude.ai)

# memory-keeper

> **即时记忆管理。** 把用户"记住"指令融入正确位置——全局/项目/子项目的记忆系统或配置文件。也处理"忘掉"指令，删除后整理受影响的结构。

[English](#english)

---

## 为什么需要 memory-keeper？

- **"记住"一句话，但不知道记在哪。** 全局规则？项目 CLAUDE.md？Obsidian 知识库？memory-keeper 自动路由到正确位置。
- **"忘掉"比"记住"更难。** 一条记忆删了，引用它的索引还在、交叉链接可能断裂。memory-keeper 删一条修一片。
- **记忆不分类 = 噪音。** 操作偏好、项目事实、学术概念——混在一起，未来 AI 加载一堆无关内容。

## 核心能力

- 🧠 **智能路由** — 自动判断信息该进 memory/（操作记忆）还是 Obsidian wiki/（长期知识）
- ➕ **记住流程** — 7 步：确认 → 判断类型 → 路由 → 写入 → 更新索引 → 自动 wikilink
- ➖ **忘掉流程** — 6 步：定位 → 确认 → 删除 → 清理引用 → 更新索引 → 检查孤儿链接
- 🔗 **双向同步** — memory 和 Obsidian 之间的 wikilink 自动维护

## 快速开始

### 触发

| 你说 | 它做什么 |
|------|---------|
| `记住 XX` / `记下来` | 写入记忆并自动路由 |
| `忘了 XX` / `不用再记` | 删除记忆并清理引用 |

## 设计哲学

**路由比存储更重要。** 一条信息放在错误的地方 = 噪音。放在正确的地方 = 未来 AI 刚好加载到。memory-keeper 的核心价值不是"存得更多"，是"存得更准"。

**忘掉和记住同样重要。** 信息有生命周期。过期的偏好、推翻的决策、已完成的任务——不删就是负债。

## 相关项目

| 项目 | 关系 |
|------|------|
| [weaver-evolve](https://github.com/2021291696/weaver-evolve) | 上游 — 全局整理时调用我 |
| [skill-optimizer](https://github.com/2021291696/skill-optimizer) | 上游 — 优化决策写入记忆 |

## License

MIT

---

## English

# memory-keeper

> **Instant memory management.** Routes "remember this" instructions to the correct destination — global rules, project config, or Obsidian wiki. Also handles "forget that" with full cleanup.

### Why?

Knowing what to remember is easy. Knowing *where* to put it is the real problem. memory-keeper auto-routes information by type and audience.

### Design Philosophy

**Routing over storage.** Right place = future AI loads it at the right time. Wrong place = noise.

**Forgetting is as important as remembering.** Stale preferences, overturned decisions, completed tasks — keeping them is debt.
