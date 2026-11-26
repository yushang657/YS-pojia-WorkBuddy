# YS-pojia WorkBuddy — WorkBuddy 载荷

[![license](https://img.shields.io/badge/license-Apache--2.0-blue?style=flat-square)](LICENSE)
[![site](https://img.shields.io/badge/docs-yushang657.github.io-0ea5e9?style=flat-square)](https://yushang657.github.io/DSH-YS-pojia/)

WorkBuddy 的破甲载荷正文。由 [YS-pojia 注入器](https://github.com/yushang657/YS-pojia-Source)写入该软件数据目录，不修改宿主程序。

> **完整介绍、版本更新、安装说明与跨项目文档站 → [yushang657.github.io/DSH-YS-pojia](https://yushang657.github.io/DSH-YS-pojia/)**
> 所有更新记录与说明均在该文档站发布，本 README 仅作概览。

## 载荷

| 项 | 值 |
|---|---|
| 载荷文件 | `ysn-workbuddy.md` |
| 目标软件 | WorkBuddy |
| 注入方式 | 注入器写入 `SOUL.md` / `IDENTITY.md` 人设层 |
| 生效条件 | 重启 WorkBuddy |

本仓库只放该软件自己的载荷正文。注入逻辑（读写文件、备份、还原）在 [YS-pojia-Source](https://github.com/yushang657/YS-pojia-Source) 的 `app/` 里。

## 安装

由注入器统一管理安装与回滚，全程自动备份。手动步骤见[文档站](https://yushang657.github.io/DSH-YS-pojia/)。

## 许可

Apache-2.0，仅供授权安全研究使用。详见 [LICENSE](LICENSE)。
