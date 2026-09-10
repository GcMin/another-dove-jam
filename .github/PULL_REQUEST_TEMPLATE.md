## 变更类型

- [ ] Main 共同约束/模板/协作规则
- [ ] 跨 proposal 决策
- [ ] 其他经过团队明确确认的 main 变更

## 为什么必须修改 Main？

说明为什么这不是某个单独 proposal 分支自己的事情。

## 影响范围

- 影响哪些 proposal：
- 是否需要现有 proposal 迁移：是 / 否
- 是否改变 main 的职责：是 / 否

## 检查

- [ ] 没有夹带某个具体游戏的玩法、剧情、角色、Boss、关卡或数值设计
- [ ] 没有提交具体游戏的 `project.godot`、场景、脚本或资源
- [ ] 规则变更已同步更新相关文档
- [ ] 如涉及跨 proposal 决策，已更新 `docs/DECISIONS.md`
- [ ] 没有把某个 proposal 的专属架构包装成全仓库强制标准

## 说明

如果这个 PR 的核心内容其实是一款具体游戏，它大概率提交错地方了。请把它留在 `proposal/<developer>/<game-slug>` 分支。