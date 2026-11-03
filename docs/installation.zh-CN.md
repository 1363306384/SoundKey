# 安装 SoundKey

[English](installation.md) · **简体中文** · [返回首页](../README.zh-CN.md)

从 [1.0.2 发布页](https://github.com/1363306384/SoundKey/releases/tag/v1.0.2)下载安装包。发布附件提供 SHA-256 校验文件，可用于核对下载完整性。

| 平台 | 安装包 | 系统要求 |
| --- | --- | --- |
| Mac | `SoundKey-1.0.2-Mac-arm64.dmg` | Apple Silicon，macOS 13 或更高版本 |
| Windows | `SoundKey-1.0.2-windows-x64-Setup.exe` | Windows 10 或 11，x64 |

## Mac

当前 Mac 应用使用 Apple Development 开发签名；Installer 安装包未签名，发行包**尚未经过 Apple 公证**。macOS 可能要求手动确认。这不是 App Store 或已通过 Developer ID 签名、公证的发行版本。

1. 退出正在运行的 SoundKey。
2. 打开下载的 DMG。
3. 运行包内 **Install SoundKey.command**，阅读提示后，输入 **INSTALL** 确认继续。
4. 在 Apple 系统安装器中完成安装，应用会安装到「应用程序」。
5. 从「应用程序」打开 **SoundKey**。

这个 command 文件是当前版本的安装入口。它会先校验旁边的 `SoundKey.pkg`，再准备临时安装副本。隔离标记修复仅限校验通过的临时安装包与 SoundKey 应用，不会关闭系统全局 Gatekeeper。请保留配套文件，不要替换成其他版本的安装包。

如果 Finder 无法运行 command 文件，打开「终端」，输入 `/bin/bash` 和一个空格，再把已挂载 DMG 中的 **.command** 文件拖进终端，按回车。阅读提示，确认要安装本次下载后再输入 **INSTALL**。如果校验失败，请重新下载配套版本，不要绕过检查。

### 在其他软件中使用快捷键

后台快捷键可以稍后设置，导入后即可先用鼠标播放音乐。

1. 打开 SoundKey「设置 → 后台快捷键 → 打开输入监控」。
2. 在「系统设置 → 隐私与安全性 → 输入监控」中，添加或开启「应用程序」中的 SoundKey。SoundKey 会提供方便添加应用的拖拽条。
3. 如果系统提示，选择「退出并重新打开」。若应用没有自动重新打开，从「应用程序」手动打开即可。
4. 回到 SoundKey 设置，点击「重新检查」。确保「音乐快捷键总开关」开启，关闭设置后再切换到其他软件测试绑定键。

系统开关已开启时，当前进程仍可能尚未获得有效授权。如果 SoundKey 继续提示输入监控尚未生效，请完全退出应用，重新打开「应用程序」中的版本，再检查一次。避免同时运行下载目录或其他磁盘映像里的旧副本。

另一台 macOS 15.2 电脑首次授权时的「退出并重新打开」完整流程尚未验证。本次更新范围见[版本说明](releases/1.0.2.zh-CN.md)。

## Windows

1. 如果 SoundKey 正在运行，先退出。
2. 运行 **SoundKey-1.0.2-windows-x64-Setup.exe**。
3. 按安装器提示完成安装，再从桌面或开始菜单快捷方式打开 SoundKey。

安装与卸载向导的按钮、提示和快捷方式名称统一使用英文。安装后的应用仍可在设置中切换英文和中文。安装包内置所需 .NET 运行时和导入工具，按当前用户安装。升级时会把已知旧版中文快捷方式替换为英文 **SoundKey** 与 **Uninstall SoundKey** 入口，保留音乐、分组、绑定和设置。

应用和安装器仍未使用 Authenticode 发行签名，Windows 可能显示未知发布者或 SmartScreen 提示。请先核对下载来源与校验值，再决定是否继续。自动回归覆盖本次更新的播放、导入和转换流程；本次候选包的 Windows 原生安装和界面检查仍未验证，自动检查没有运行 WPF 界面或操作系统的全局键盘钩子。详见[版本验证范围](releases/1.0.2.zh-CN.md#验证范围)。

### Windows 可以签名吗？

可以。Windows 发行使用受信任证书机构提供的 Authenticode 代码签名身份，或符合资格并通过身份核验的 **Microsoft Artifact Signing** 账户。后者需要付费 Azure 订阅，并有国家／地区及个人／组织资格限制。Apple 开发证书不能用于 Windows；SoundKey 1.0.2 目前尚未配置 Windows 发行签名身份。详见 [Microsoft 签名前提](https://learn.microsoft.com/en-us/azure/artifact-signing/quickstart)和[订阅要求](https://learn.microsoft.com/en-us/azure/artifact-signing/faq)。

受信任签名可以标识经过核验的发行人，并验证文件完整性，但不保证新版本立即免除 SmartScreen 提示；EV 签名也可能需要积累信誉。自签名不会让应用自动获得公众信任。详见 [Microsoft SmartScreen 说明](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/smartscreen-reputation)。

## 更新、备份与卸载

更新前，建议从「曲库 → 曲库备份与恢复」导出备份。退出 SoundKey 后，将新版安装到原应用位置；确认新版工作正常后再处理旧备份。

Windows 卸载器移除应用及快捷方式，保留本地曲库。Mac 删除应用也会保留单独存放的曲库。卸载应用不等于清空全部数据。

分组、快捷键和备份的日常用法见[用户指南](user-guide.zh-CN.md)。
