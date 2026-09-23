# Windows v0.1.4

[返回首页](../../README.md) · [开发源码](../../源码/README.md)

本仓库仅提供这一个 Windows 版本，不包含 Mac 或旧版 Windows 程序。

## 安装包下载

- [Windows 便携 ZIP](https://github.com/putilaotie123456/codex-meter-windows/releases/download/v0.1.4/Codex-Meter-Windows-portable-v0.1.4.zip)
- [SHA-256 校验文件](https://github.com/putilaotie123456/codex-meter-windows/releases/download/v0.1.4/Codex-Meter-Windows-portable-v0.1.4.zip.sha256)
- [Release 页面](https://github.com/putilaotie123456/codex-meter-windows/releases/tag/v0.1.4)

ZIP 大小：6,280,654 字节。SHA-256：

```text
007fb74196abbbe6de7f801a54b1e5b99c77516f1779eb40633c3be96e893df0
```

Windows 10/11、.NET Framework 4.7.2 或更高版本。需已登录 Codex。完整解压后运行 `CodexMeter.exe`，保持内置 `codexbar-cli.exe` 和许可证等文件在同一目录；不需要另装 Win-CodexBar。软件未进行 Authenticode 签名，请核对来源和校验值。

## 这一版的功能

包含每周额度、系统网速、托盘、自启动、贴边、近 7 天用量、模型偏好及重置历史。

v0.1.4 的重置历史时间轴会延伸至今天，连续无记录的日期也保留每日刻度；显示距上次重置已过多久。点击倒计时先打开时间轴，再通过底部按钮切换可滚轮浏览的历史记录列表。

## 源码与来源

- [本仓库 v0.1.4 源码 ZIP](https://github.com/putilaotie123456/codex-meter-windows/archive/refs/tags/v0.1.4.zip)：源码在 `源码/`，不是运行安装包。
- [原始 Windows v0.1.4 发布来源](https://github.com/xumanba/codex-meter/releases/tag/v0.1.4)。
- 源码取自已整理的 Windows 工程 `8f9ea39b00060bdba6e7fb50b380d1154a58f91a`，该整理已合并到原仓库 `ff69332cfaad41743cb20e14573b31d490ae1d71`。

本仓库仅调整目录和文档，没有修改 C# 程序、安装/卸载行为或内置 CLI。Release 上传的是原始 ZIP，不是本次重新编译生成的包；原包保留其原有项目链接和归属说明。MIT 及依赖许可证全部保留。

独立目录已完成本地构建、211 项自测、10 文件打包检查、文档本地链接检查及简易卡片/历史时间轴测试数据预览。32 个 C# 文件与来源工程逐文件 SHA-256 一致。重建验证包仅保存在本地，不替代上面的原始 Release ZIP。

本次发布不重新安装或替换用户电脑上的程序，也不更改代理、自启动或用户数据。目录分离后的构建与自测以本仓库 Windows CI 为准；不宣称完成了新的账号在线同步或全新系统安装测试。
