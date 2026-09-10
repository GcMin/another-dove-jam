# Cross-Proposal Decisions

这里只记录影响多个 proposal 或仓库整体协作方式的决定。

单一游戏方案自己的玩法/技术决策，应记录在该 proposal 分支的 `docs/DECISIONS.md`。

---

## D-0001 — 使用 Main 约束 + 独立 Proposal 分支

- 日期：2026-09-10
- 状态：Accepted
- 影响范围：整个仓库

### 决策

仓库采用以下协作模型：

```text
main
├─ 共同约束
├─ 协作规范
├─ 模板
└─ 跨 proposal 决策

proposal/<developer>/<game-slug>
├─ 独立游戏设计
├─ Godot 项目
├─ 原型与实现
├─ 资产
└─ 本方案自己的决策记录
```

每位开发者在独立 proposal 分支探索一套独立游戏方案。探索阶段不要求多个方案共享游戏代码，也不把任何一个方案默认视为正式主线。

### 原因

- 避免多人在尚未确定游戏方向时争夺同一代码结构。
- 允许不同开发者完整验证不同玩法，而不是过早妥协成一个谁都不满意的混合物。
- 让 main 成为稳定协作契约，降低跨方案冲突。
- 后续选型依据可玩原型和评审，而不是谁先把代码合进 main。

### 迁移要求

新 proposal 必须从 main 创建，并遵守 `docs/COLLABORATION_RULES.md`。

---

## 决策模板

```markdown
## D-XXXX — 标题

- 日期：YYYY-MM-DD
- 状态：Proposed / Accepted / Superseded
- 影响范围：

### 决策

### 原因

### 迁移要求

### 替代/被替代
```
