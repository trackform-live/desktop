<p align="center">
  <img src=".github/assets/icon.png" width="96" height="96" alt="Trackform Live">
</p>

<h1 align="center">Trackform Live 桌面端</h1>

<p align="center">
  面向教育培训的直播学习平台客户端：看直播、看回放、课程资料、互动答疑，讲师一键推流。
</p>

<p align="center">
  <a href="https://github.com/trackform-live/desktop/releases/latest"><img alt="最新版本" src="https://img.shields.io/github/v/release/trackform-live/desktop?label=%E6%9C%80%E6%96%B0%E7%89%88%E6%9C%AC"></a>
  <a href="https://github.com/trackform-live/desktop/issues"><img alt="问题反馈" src="https://img.shields.io/github/issues/trackform-live/desktop?label=%E9%97%AE%E9%A2%98%E5%8F%8D%E9%A6%88"></a>
</p>

> 本仓库只用于发布安装包和收集反馈，不包含源代码。

## 下载

| 系统 | 安装包 | 国内加速下载 | GitHub 直连 |
| --- | --- | --- | --- |
| Windows 10 / 11（64 位） | `trackform-live-setup.exe` | [下载](https://gh-proxy.com/https://github.com/trackform-live/desktop/releases/latest/download/trackform-live-setup.exe) | [下载](https://github.com/trackform-live/desktop/releases/latest/download/trackform-live-setup.exe) |
| macOS 12 及以上（Apple 芯片 M1 / M2 / M3 / M4） | `trackform-live-arm64.dmg` | [下载](https://gh-proxy.com/https://github.com/trackform-live/desktop/releases/latest/download/trackform-live-arm64.dmg) | [下载](https://github.com/trackform-live/desktop/releases/latest/download/trackform-live-arm64.dmg) |
| macOS 12 及以上（Intel 芯片） | `trackform-live-x64.dmg` | [下载](https://gh-proxy.com/https://github.com/trackform-live/desktop/releases/latest/download/trackform-live-x64.dmg) | [下载](https://github.com/trackform-live/desktop/releases/latest/download/trackform-live-x64.dmg) |
| Linux（64 位） | `trackform-live.AppImage` | [下载](https://gh-proxy.com/https://github.com/trackform-live/desktop/releases/latest/download/trackform-live.AppImage) | [下载](https://github.com/trackform-live/desktop/releases/latest/download/trackform-live.AppImage) |

历史版本与更新说明见 [Releases](https://github.com/trackform-live/desktop/releases)。客户端会自动检查更新，一般无需手动下载新版。

> 不确定 Mac 是哪种芯片？点击屏幕左上角  →「关于本机」，「芯片」一栏显示 Apple M 系列即为 Apple 芯片，显示 Intel 即为 Intel 芯片。

## 安装说明

**Windows**：运行安装程序。若出现「Windows 已保护你的电脑」，点击「更多信息」→「仍要运行」。

**macOS**：打开 dmg，把 Trackform Live 拖进「应用程序」。首次打开如提示「无法验证开发者」：

1. 打开「系统设置」→「隐私与安全性」，在页面下方点击「仍要打开」；
2. 若提示「已损坏，无法打开」，在「终端」中执行下面的命令后再打开：
   ```bash
   xattr -cr "/Applications/Trackform Live.app"
   ```

**Linux**：下载后赋予执行权限再运行：

```bash
chmod +x trackform-live.AppImage
./trackform-live.AppImage
```

## 校验安装包

每个版本的发布说明中列出了各安装包的 SHA-256，可用下面的命令核对（与发布说明一致即为官方原版）：

```bash
# Windows（PowerShell）
Get-FileHash .\trackform-live-setup.exe -Algorithm SHA256
# macOS / Linux
shasum -a 256 trackform-live-arm64.dmg
```

客户端自动更新时也会校验 SHA-256，不一致的安装包会被丢弃。

## 问题反馈

- **使用中遇到问题**：[提交问题](https://github.com/trackform-live/desktop/issues/new/choose)，请写明客户端版本（「个人中心 → 关于」）、操作系统和复现步骤。
- **功能建议、使用交流**：[讨论区](https://github.com/trackform-live/desktop/discussions)。
- **安全问题**：请通过 [私密漏洞报告](https://github.com/trackform-live/desktop/security/advisories/new) 提交，不要公开发布。

> 请勿在 Issue 或讨论中填写手机号、身份证号、账号密码、课程激活码等个人信息。

## 移动端

Android / iOS 客户端见 [trackform-live/app](https://github.com/trackform-live/app)。

---

© Trackform. 保留所有权利。
