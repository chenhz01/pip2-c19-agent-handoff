# Learning Cards

Four layers per card: **L0** a twelve-year-old can follow → **L1** the mechanism → **L2** how to use it → **limit** when it fails. Gap evidence follows each cluster.

---

## c19 代理间交接（3 件）— 证据：`agent handoff protocol` 236 仓半满（协议层 vs v1 L33 内容层，正交）

- **L72 交接协议完整性**：L0 一个伙伴把活交给另一个时，交接单必须写全：干到哪、卡在哪、下一步谁干。缺项的交接单不许收。L1 校验交接包必填字段（状态/阻塞/下一步/权限边界），缺项拒收并列缺失。L2 断言=①缺「阻塞项」拒收、②齐全签收。
- **L73 注意力分诊**：L0 多个伙伴同时干活时，它回答一个问题：现在谁在等我？谁的事最急？L1 汇总各协作者状态（working/waiting/done），按等待时长+阻塞链长度排优先级。L2 断言=①被阻塞链最长的排最前、②done 的不占队列。
- **L74 并发写冲突闸**：L0 两个人同时改同一份文件，后写的会盖掉先写的——它把这单查出来，让你决定谁先。L1 检测多 agent 对同一资源的写意图重叠（资源路径+时间窗），重叠 → 冲突报告。L2 断言=①同资源双写意图报冲突、②不同资源放行。
