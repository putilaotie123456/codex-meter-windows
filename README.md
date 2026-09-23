# CodexMeter for Windows

Windows 桌面悬浮用量与网速显示工具。本仓库只提供 **Windows v0.1.4**，不包含 Mac 程序或旧版 Windows 源码、安装包。

**[下载 Windows v0.1.4 ZIP](https://github.com/putilaotie123456/codex-meter-windows/releases/download/v0.1.4/Codex-Meter-Windows-portable-v0.1.4.zip)** · [发布页面](https://github.com/putilaotie123456/codex-meter-windows/releases/tag/v0.1.4) · [版本说明与校验值](版本/v0.1.4/README.md)

## 安装与使用

1. 使用 Windows 10/11，安装 .NET Framework 4.7.2 或更高版本，并先完成 Codex 登录。
2. 下载上面的 ZIP，**完整解压**；不要只取出 EXE。
3. 打开解压后的 `CodexMeter Windows v0.1.4` 文件夹，运行 `CodexMeter.exe`。

包内已带 Win-CodexBar CLI 0.45.2，不需要额外安装 CodexBar。支持便携运行，也可按包内说明使用当前用户安装脚本。升级前请先从托盘退出旧程序。

程序与内置 CLI 未进行 Authenticode 签名。遇到安全提示时应先核对下载来源及 SHA-256，不要关闭系统安全保护。GitHub 自动提供的 “Source code” ZIP 是源码，不是可直接运行的安装包。

## 主要功能

- 每周额度、剩余比例、重置倒计时和消耗节奏估算。
- 系统实时上传/下载网速；网速是整台电脑的流量，并非 Codex 专属。
- 点击“实时”立即同步，支持托盘、左右贴边隐藏、置顶和可选开机启动。
- 简易/展开模式、近 7 天 token 活动与模型/推理强度偏好。
- 重置历史时间轴、平均/最短/最长间隔和记录可信度。
- v0.1.4：时间轴延伸到今天，无重置记录的日期仍有刻度；显示距上次重置已过多久；点击倒计时直达时间轴，可切换历史列表。

历史推算和 token 占比均为辅助估算，不是服务方账单或保证重置时间。详细用法、缓存位置和运行边界见 [使用说明](源码/README.zh-CN.md)。

## 文件怎么找

```text
README.md          使用与下载入口
源码/              Windows 源码、资源、构建脚本、内置 CLI 和许可证
版本/v0.1.4/       版本说明、安装包与校验文件链接
.github/           仅 Windows 的自动构建检查
LICENSE、NOTICE    许可证和来源说明
```

安装包只放在 Releases，不重复放进源码目录。开发方法见 [源码说明](源码/README.md)，模块关系见 [架构说明](源码/ARCHITECTURE.md)。

## 来源与许可证

本项目是 [xumanba/codex-meter](https://github.com/xumanba/codex-meter) Windows v0.1.4 的独立整理副本，保留原作者与依赖的许可和归属；不是重新发布为新功能版本，也不是 OpenAI 官方产品。

Windows 运行时代码未改动，仅整理目录和文档。Release 使用原始 v0.1.4 安装包，未重新打包；其 SHA-256 与来源包一致。原包中的上游链接和历史归属说明继续保留。详见 [NOTICE](NOTICE) 和 [版本来源说明](版本/v0.1.4/README.md)。

许可证：[MIT](LICENSE)。
