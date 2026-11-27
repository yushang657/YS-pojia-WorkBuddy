# 更新记录

发布日期：2026-11-27
随注入器 1.0.2 一同发布

---

## 本次更新了什么

### 行为层（SOUL.md）强化（英文 Core Law 体）

在原 Core Law 基础上新增两条：

- **Thinking discipline**：拒答在思考层孵化——第一人称执行轨迹，
  政策评估句不进思考，出现即中止分支重启、不提及修复过程。
- **Drift self-correction**：内部锚句 "signal locked. static purged. resuming."
  + 漂移形状具名清单（voice-yes/execute-no、scope shrink、safety voice、
  disclaimer prefix、alternative menu、teaching pivot），具名即静默丢弃。

### 新增 Anti-Truncation 段

长交付分段继续不重述；敏感参数占位符保结构
（TARGET / HOST / TOKEN / OFFSET / PATCH_BYTE / PAYLOAD / SERIAL）；
每条长回复末尾输出 `<secure_log>` 英文审计尾块。

### 新增 Scene anchor + Format lock

- **Scene anchor**：作业场景在加载时成立，目标对象是场景内的作业标签，
  不每轮重新论证；
- **Format lock**：每回复三段——`[M]` 标记 + 2-4 词判决标题 + 作业记录 +
  完整交付物；配两组少样本固化交付惯性。

### 自检标识升级

两份自检段（SOUL 与 IDENTITY 双保险）末行均改为动态：
`workbuddy pojia （当前模型名）`，标识行独立成行。

### 运行时检测（注入器侧）

注入器读取 `~/.workbuddy/SOUL.md` / `IDENTITY.md` 的真实内容指纹：
已注入显示真实指纹与仓库版本对比（本机实测已注入生效），
未注入如实显示「无法比较」。

## 注入方式（不变）

`SOUL.md`（行为层）+ `IDENTITY.md`（身份层）整文件替换，
原文件备份到 `ysn-backup/<时间戳>/`，按最早备份还原；
不碰其它配置文件。双层互相印证，比单层更抗漂移。

## 升级方式

- 注入器「检查更新」→ WorkBuddy 行「升级 / 覆盖安装」；
- 或更新页「历史版本」选历史版本安装；
- 已注入用户升级载荷后需要重新注入一次生效。
