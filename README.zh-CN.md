[English](README.md) | 简体中文

# codex-claude-muse-boot

**给 AI 编程工具的开机 / 启动动画 —— Codex、Claude、Muse 三版角色闪屏，一个零依赖的 HTML 文件全搞定。**

[![Stars](https://img.shields.io/github/stars/chenyi6758-source/codex-claude-muse-boot?style=flat)](https://github.com/chenyi6758-source/codex-claude-muse-boot/stargazers)
[![Forks](https://img.shields.io/github/forks/chenyi6758-source/codex-claude-muse-boot?style=flat)](https://github.com/chenyi6758-source/codex-claude-muse-boot/network/members)
[![Last commit](https://img.shields.io/github/last-commit/chenyi6758-source/codex-claude-muse-boot?style=flat)](https://github.com/chenyi6758-source/codex-claude-muse-boot/commits/main)
[![License](https://img.shields.io/github/license/chenyi6758-source/codex-claude-muse-boot?style=flat)](LICENSE)
[![在线演示](https://img.shields.io/badge/在线演示-demo.cyruscy.me-brightgreen)](https://demo.cyruscy.me/)

灵感来自 DeepSeek Harness（DSH）上爆火的开机动画插件和 dragon-codex-boot 启动器。这个项目把那套“操作系统开机”仪式带给没有开放插件系统的 AI 工具，并做成**角色闪屏**风：角色立绘缓缓淡入、花体签名与一句标语浮现、标志描边成形、金属大字逐字显现、终端风 loading 日志滚动、最后聊天框升起定版。

> **非官方粉丝概念作品。** 与 OpenAI、Anthropic、Meta 无关。所有标志均为手绘同风格图形，未使用任何官方素材。Codex、Claude、Muse 都没有开放开机动画插件接口——这是一个可直接播放的概念演示，也是后续做启动器 / 桌面端集成的起点。

## 演示

**▶ 在线演示：https://demo.cyruscy.me/**

或用任意现代浏览器打开 `index.html`。无需构建、无依赖、无需服务器。三个舞台并排自动播放，可单独或同步重播、暂停、变速（0.5× / 1× / 2×）。单版时长约 6.8 秒；整页是一个约 86 KB 的 HTML 文件加三张角色立绘（1920 × 1280）。

| Muse ——「Cyrus」 | Codex | Claude |
|---|---|---|
| ![Muse 角色](assets/char-muse.webp) | ![Codex 角色](assets/char-gpt.webp) | ![Claude 角色](assets/char-claude.webp) |

纯标志动画的原版保留在 [`index-v1-original.html`](index-v1-original.html)（在线版：https://demo.cyruscy.me/index-v1-original.html）。

## 功能

- **三个角色闪屏舞台** —— Muse（星火标、宝蓝、常驻角色 Cyrus）、Codex（六角结扣标、经典绿、“构建模式”）、Claude（陶土橙放射星芒、“深度思考模式”），各自有能力栏、终端启动日志和标语
- **黑客帝国矩阵雨模式** —— 全局开关，三块屏幕同时下起片假名/数字雨，启动日志逐字打字输出
- **舞台特效** —— 故障 Glitch、粒子星尘汇聚、霓虹网格、光轨扫描、溶解收尾等
- **素材工作台**
  - 11 个代码生成主题（深海极光、霓虹雨夜、矩阵代码雨……），零素材也能玩
  - 在线搜图直连 **Wikimedia Commons**（默认）和 **Openverse**（备用），均免费、免 API key，点一张即套为开机背景
  - **上传动效化**：拖入自己的图片或视频，选 10 种动效预设和时长，你的素材立刻变成开机动画；全程在本机内存处理，不经过任何服务器
  - **Steam Wallpaper Engine 导入**：粘贴工坊链接自动解析物品 ID，给出本地路径（`steamapps/workshop/content/431960/<ID>`）和 `steam://` 深链一键在 Steam 客户端打开，下载后把壁纸文件拖进上传区即可使用

## 在 Windows 与 macOS 上

本页本身与平台无关——任意现代浏览器、两个系统都能直接打开，零安装。真要给官方应用配上启动动画，两边的路线不同（下面的原生项目也是这么分的）：

- **Windows** —— 深度集成路线。[dragon-codex-boot](https://github.com/yushua0808-cpu/dragon-codex-boot) 是原生 Codex 启动器，替换应用快捷方式（带可还原备份）并把真实窗口嵌进动画；DSH 系列开机插件支持换成自己的视频，把本页舞台录制/导出的片段放进去即可；Wallpaper Engine 壁纸可用上方内置导入转成开机背景。
- **macOS** —— 保守覆盖路线。原生启动器（dragon-codex-boot 另有独立的 Swift 版）用自己的窗口播放、淡出交接，不改官方应用、不动 Dock、不申请录屏/辅助功能权限；未签名应用首次启动需右键 → 打开（Gatekeeper）。Mac 上零安装路线就是上面的在线演示。

## 同类项目

- [NativeDog1/dsh-boot-animation](https://github.com/NativeDog1/dsh-boot-animation) —— DSH 开机插件原版（324★），支持换自己的视频
- [lxj5820/dsh-boot-animation](https://github.com/lxj5820/dsh-boot-animation) —— 带片尾溶解进应用的 DSH 插件（254★）
- [yushua0808-cpu/dragon-codex-boot](https://github.com/yushua0808-cpu/dragon-codex-boot) —— Codex 原生启动器（Windows & macOS），龙女角色闪屏（263★）
- [yannicksong0106/dsh-550c-boot](https://github.com/yannicksong0106/dsh-550c-boot) —— 产品化程度最高的 DSH 开机动画，带主题与开机音乐（180★）

## 为什么做这个

在 GitHub 上，开机动画插件只在平台开放可安装时才爆起来：DeepSeek Harness 有一整个集群（原版 324★），Codex 有 dragon-codex-boot（263★）和几个 0–2 星的尝试，Claude 只有三个小项目，Muse 一个都没有。这个仓库把三家的概念收拢到一处，并保持它可魔改：单文件、代码可读、一切效果由代码生成。

## 路线图

- [ ] 给 README 顶部配上三版舞台的演示 GIF
- [ ] 把合成好的舞台导出为 MP4 / WebM / GIF（可直接用作 DSH 插件片头）
- [ ] 可下载素材包：角色 PNG + 舞台录制
- [ ] 分时段片头与片库轮换模式
- [ ] Codex / Claude 桌面版（Windows）独立启动器：全屏片头播完无缝交接给应用
- [ ] 更多品牌舞台与社区主题

## 授权

代码 MIT。`assets/` 中的角色立绘为本项目 AI 生成。通过 Wikimedia Commons / Openverse 获取的图片遵循其各自的单图授权，再利用前请查看每张图旁标注的授权信息。
