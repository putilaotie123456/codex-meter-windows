# Windows v1.0.0

[返回首页](../../README.md) · [开发源码](../../源码/README.md)

本仓库只维护 Windows，不包含 Mac 程序或源码。

## 安装包下载

- [Windows 便携 ZIP](https://github.com/putilaotie123456/codex-meter-windows/releases/download/v1.0.0/Codex-Meter-Windows-portable-v1.0.0.zip)
- [SHA-256 校验文件](https://github.com/putilaotie123456/codex-meter-windows/releases/download/v1.0.0/Codex-Meter-Windows-portable-v1.0.0.zip.sha256)
- [Release 页面](https://github.com/putilaotie123456/codex-meter-windows/releases/tag/v1.0.0)

ZIP 大小：6,281,042 字节。SHA-256：

```text
cf1708d5aba9cf1893ec3101815ab7b5a936711923d0dce3c4274722aceb9494
```

需要 Windows 10/11、.NET Framework 4.7.2 或更高版本，并已登录 Codex。完整解压后进入 `CodexMeter Windows v1.0.0`，运行 `CodexMeter.exe`。包内已带 Win-CodexBar CLI 0.45.2，不需要另装 CodexBar；软件未进行 Authenticode 签名，请核对来源和校验值。

## 相比 v0.1.4

- 统一版本号为 v1.0.0，程序文件版本为 1.0.0.0。
- 更新构建、打包、云端检查配置及下载说明，重新编译生成独立 ZIP 和校验文件。
- 功能、界面和业务逻辑不变，保留每周额度、系统网速、托盘、自启动、贴边、近 7 天用量、模型偏好和重置历史。
- 内置 CLI、安装路径和用户数据格式不变；升级无需清空设置或重置历史。

升级前先从托盘退出旧程序，再完整解压运行新版，或按包内说明运行新版 `install.ps1`。发布新版不会自动替换本机已经安装或正在运行的程序。

## 源码与来源

- [v1.0.0 源码 ZIP](https://github.com/putilaotie123456/codex-meter-windows/archive/refs/tags/v1.0.0.zip)：源码位于 `源码/`，不是可直接运行的安装包。
- 基于本仓库 v0.1.4（`4f874393eaca5021bb7973e4c0ccc90c401a2d63`），上游归属与许可证见 [NOTICE](../../NOTICE)。
- 本仓库将原 v0.1.4 发布替换为 v1.0.0，仅保留当前版本的标签、安装包和版本目录；Git 提交历史保留。Mac 和上游原仓库不受本次更新影响。

## 验证范围

已完成本地编译、211 项自测及 10 文件打包检查，EXE 文件版本核对为 1.0.0.0，包内 CLI 的固定 SHA-256 校验通过。本次不进行新的账号在线同步、全新系统安装或本机安装替换；云端构建以本仓库 Windows CI 结果为准。
