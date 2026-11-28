# iClip — macOS 剪切板 / 剪贴板历史管理工具（兼容 Windows 10/11）

> **纯原生 Swift（macOS）与 Rust Win32（Windows）打造的液态玻璃剪切板与灵感待办工作台**｜安装包仅 **1.2–4.7 MB**、待机 **0.00% CPU**、完全离线加密、全部核心功能免费无订阅。
>
> **[官方网站与在线交互体验](https://app.webfooo.com/iClip)** · **[6 款 macOS 剪切板对比指南](https://app.webfooo.com/iClip/macos-clipboard)** · **[v3.5.1 实机使用教程](https://app.webfooo.com/iClip/guide)** · **[Releases 最新下载](https://github.com/fanaruto/iClip/releases/latest)**

按下 **`⌥V`**（macOS）或 **`Alt+V`**（Windows），系统级液态玻璃剪切板面板在你的**鼠标光标旁 0ms 零失焦滑落**——原输入框与微信/飞书搜索框全程不关闭；选中回车或按 **`⌘1–9`** 直接落字，随时按 **`⌘E` / `Ctrl+E`** 一键切回极简纯净模式。

<p align="center">
  <img src="assets/demo.gif" alt="iClip macOS 剪切板与剪贴板历史实机演示：鼠标旁零失焦唤醒、原生液态玻璃材质、3 列截图相册悬停放大与双击直贴" width="760" />
</p>

---

## 快速安装（3 秒直装，免安全拦截弹窗）

- **macOS 14+（原生通用支持 Apple Silicon M1/M2/M3/M4 与 Intel Mac）**：
  ```zsh
  curl -fsSL https://app.webfooo.com/iClip/install.sh | zsh
  ```
  或通过 **Homebrew Cask** 安装：
  ```zsh
  brew install --cask fanaruto/tap/iclip
  ```
  自动从国内高速源下载并装入「应用程序」，绕过浏览器下载隔离标记，免除「无法验证开发者」弹窗。
- **Windows 10 / 11（64 位纯 Rust Win32 原生版，约 1.2 MB）**：
  ```powershell
  irm https://app.webfooo.com/iClip/install.ps1 | iex
  ```
- **手动下载安装包**：前往 [iClip 官网高速下载页](https://app.webfooo.com/iClip) 或本仓库 [GitHub Releases](https://github.com/fanaruto/iClip/releases/latest) 获取 `.dmg` / `.zip` 安装包。

---

## 为什么选择 iClip 作为你的 macOS 剪切板工具？

1. **0ms 零失焦直贴，聊天搜索框不再塌掉**
   无激活原生悬浮架构，按下 `⌥V` 呼出时不抢占当前窗口焦点，微信、飞书搜索框与浏览器下拉输入全程保持激活；内置微信/飞书复制图片直显自愈，告别粘贴变空白或文件路径。
2. **3 列截图相册 + HeroZoom 实况识字 OCR 与原位批注**
   连续截图自动聚合成 3 列圆角相册并智能避让放大预览；按 `Space` 触发 120Hz GPU 大屏预览，按 `T` 离线调用系统级 VisionKit 实况划字，按 `E` 原位液态玻璃标注箭头与红框。
3. **全库本地静态加密、投屏自动隐身与双向 AI 隐私替身**
   历史记录与截图 100% 本地离线存储（AES-256-GCM 硬件静态加密），无账号、无云端上传、无统计埋点；腾讯会议 / Zoom 共享屏幕自动隐身；发往大模型前按 `⇧↵` 自动替换为安全隐私替身，复制回复后一键无损还原真值。
4. **双端 1:1 纯原生体验 + 独立待办 AI MCP 闭环**
   macOS 纯 Swift + Windows 纯 Rust 双端一致体验，待机 0.00% CPU；内置 `⌥X` 独立原生待办（离线自然语言解析 + 9 大标准 MCP 工具一键对接本机 AI 客户端）与 `⌥A` 窗口磁吸截图，按 `⌘E` 可随时一键回归最安静的纯剪贴板。

---

## 与主流 macOS 剪贴板工具横向对比

> 完整 6 款工具深度横评（含 EcoPaste、Clipy）与人群选型建议见：[macOS 剪切板工具对比与使用指南](https://app.webfooo.com/iClip/macos-clipboard)。

| 对比维度 | **iClip** | Paste | Raycast | Maccy | EcoPaste |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **原生架构与体积** | Swift / Rust 纯原生（1.2–4.7 MB） | 原生（体量较大） | 综合启动器（占用偏高） | Swift 轻量原生 | Tauri / WebView |
| **唤起是否抢焦点** | **0ms 零失焦直贴** | 抢占焦点 | 抢占焦点 | 抢占焦点 | 抢占焦点 |
| **截图相册与实况 OCR** | **3 列避让相册 + 聊天图直显 + 实况 OCR/批注** | 底部横向卡片 | 单列小预览 | 无相册与 OCR | 支持卡片与插件 OCR |
| **隐私与安全能力** | **AES-256-GCM 加密 + 投屏隐身 + AI 隐私替身** | 侧重 iCloud 同步 | 基础忽略名单 | 基础忽略名单 | 本地存储 |
| **平台支持** | **macOS 14+ & Windows 10/11** | 仅 Apple 生态 | macOS 为主 | 仅 macOS | macOS / Win / Linux |
| **费用与历史迁移** | **免费无订阅 · 三步无损导入旧工具历史** | 年费订阅制 | 高级历史需订阅 | GitHub 免费 / 商店买断 | 开源免费 |

---

## 高频快捷键速查

| macOS | Windows | 功能说明 |
| :--- | :--- | :--- |
| **`⌥ V`** | **`Alt + V`** | 光标旁 0ms 零失焦呼出 / 收起剪切板主面板（支持改为双击 `⌘` / `Ctrl`） |
| **`⌘ 1` ~ `⌘ 9`** | **`Ctrl + 1` ~ `9`** | 顺位盲按直接粘贴前 9 条记录 |
| **`Tab`** | **`Tab`** | 120Hz 液态玻璃放大镜切换分类（全部 / 收藏 / 文本 / 链接 / 图片 / 文件） |
| **`Space`** | **`Space`** | HeroZoom 大屏预览（图片按 `T` 实况识字、`E` 批注；链接按 `→` 网页速览） |
| **`⌥ X`** | **`Alt + X`** | 呼出独立原生待办面板（离线自然语言解析 & AI MCP 协同） |
| **`⌥ A`** | **`Alt + A`** | 启动原生窗口磁吸截图与 AI 一键打码 |
| **`⌘ B`** | **`Ctrl + B`** | 粘贴即焚（落字 5 秒后自动清空敏感记录） |
| **`⌘ E`** | **`Ctrl + E`** | 一键切换极简纯净模式 |

完整 5 段 1080p60 实机教学视频、NLP 语法与 MCP 配置请查看 **[iClip 官方实机教程](https://app.webfooo.com/iClip/guide)**。

---

## 常见问题（FAQ）

- **macOS 系统有自带剪切板历史吗？**
  macOS 原生仅保存最近 1 条复制记录。安装 iClip 后按下 `⌥V` 即可随时回溯、检索并粘贴历史文本、截图、链接与文件。
- **从 Paste、Maccy、Raycast 或 Alfred 切换过来会丢历史吗？**
  不会。打开 iClip 设置（`⌘,`）→「数据迁移」，即可按分类三步将原剪贴板历史与常用语无损迁入本地加密库。
- **自动更新与数据隐私如何保障？**
  客户端内置基于 SHA-256 校验的一键 OTA 自动更新；剪贴内容与待办数据全程加密保存在本机，无账号体系、无云端上传、无统计埋点，联网仅用于检查与下载新版本。

---

## English Overview

**iClip** is a fast, native, offline-first **macOS & Windows clipboard manager** built with pure **Swift (macOS Liquid Glass)** and **Rust Win32 (Windows 10/11)** — zero Electron overhead, 1.2–4.7 MB binary size, and 0.00% idle CPU usage.

- **Zero-Focus-Loss Pasting (`⌥V` / `Alt+V`)**: Pops up right beside your cursor without stealing focus from search bars or popovers.
- **Visual Screenshot Grid & Offline Live Text OCR**: 3-column smart-avoidance image gallery, GPU HeroZoom preview (`Space`), native VisionKit OCR (`T`), and inline annotation (`E`).
- **Zero-Trust Privacy**: Full local AES-256-GCM encryption, automatic screen-sharing stealth mode, AI prompt secret redaction, and 5-second burn-after-paste (`⌘B`).
- **Free Alternative to Paste, Maccy & Raycast Clipboard**: Includes built-in 3-step local history migration from Paste, Maccy, Raycast, and Alfred.

Website: **https://app.webfooo.com/iClip**

---

## 仓库说明与问题反馈

- 本仓库为 **iClip 官方版本发布、自动更新分发与问题反馈仓库**（源码自 v3.5 起迁入私有仓库持续迭代，本仓库持续同步发布双端正式安装包）。
- 使用中遇到问题或有功能建议，欢迎在 [Issues](https://github.com/fanaruto/iClip/issues) 提交反馈，或直接在 [官网反馈入口](https://app.webfooo.com/iClip#community) 留言。
