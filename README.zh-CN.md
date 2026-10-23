[English](README.md) | 简体中文

# codex-claude-muse-boot

**给 AI 编程工具的开机 / 启动动画 —— Codex、Claude、Muse 三版角色闪屏，一个零依赖的 HTML 文件全搞定。**

[![Stars](https://img.shields.io/github/stars/chenyi6758-source/codex-claude-muse-boot?style=flat)](https://github.com/chenyi6758-source/codex-claude-muse-boot/stargazers)
[![Forks](https://img.shields.io/github/forks/chenyi6758-source/codex-claude-muse-boot?style=flat)](https://github.com/chenyi6758-source/codex-claude-muse-boot/network/members)
[![Last commit](https://img.shields.io/github/last-commit/chenyi6758-source/codex-claude-muse-boot?style=flat)](https://github.com/chenyi6758-source/codex-claude-muse-boot/commits/main)
[![License](https://img.shields.io/github/license/chenyi6758-source/codex-claude-muse-boot?style=flat)](LICENSE)
[![在线演示](https://img.shields.io/badge/在线演示-demo.cyruscy.me-brightgreen)](https://demo.cyruscy.me/)

**▶ 先看动图，再打开玩：[demo.cyruscy.me](https://demo.cyruscy.me/) · 或从 [Releases](https://github.com/chenyi6758-source/codex-claude-muse-boot/releases) 下载单文件带走**

![演示——Codex、Claude、Muse 三版角色闪屏](assets/demo.gif)

一套给 AI 工具的“操作系统开机”仪式，做成**角色闪屏**风：角色立绘缓缓淡入、花体签名与一句标语浮现、标志描边成形、金属大字逐字显现、终端风 loading 日志滚动、最后聊天框升起定版。三个版本、一个文件、全部效果由代码生成。

所有标志均为手绘同风格图形，未使用任何官方素材。

## 演示

**▶ 在线演示：https://demo.cyruscy.me/**

或用任意现代浏览器打开 `index.html`。无需构建、无依赖、无需服务器。三个舞台并排自动播放，可单独或同步重播、暂停、变速（0.5× / 1× / 2×）。单版时长约 6.8 秒；整页是一个约 91 KB 的 HTML 文件加三张角色立绘（1920 × 1280）。

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
  - **开机图生成**：选一版角色，填上你自己的签名和标语，一键在本机生成 1920×1080 的专属开机图 PNG——当壁纸、锁屏或启动器封面都行

## 在 Windows 与 macOS 上

本页本身与平台无关——任意现代浏览器、两个系统都能直接打开，零安装。真要给桌面应用配上启动动画，两边的可行路线不同：

- **Windows** —— 可以走深度集成：启动器类工具全屏播完片头再把应用交接出来；支持自定义视频的开机动画插件可以直接放本页舞台录制/导出的片段；Wallpaper Engine 壁纸可用上方内置导入转成开机背景。
- **macOS** —— 覆盖路线：启动器用自己的窗口播放、淡出交接，不改动应用本身；未签名应用首次启动需右键 → 打开（Gatekeeper）。Mac 上零安装路线就是上面的在线演示。

## 为什么做这个

AI 工具的开机动画是个很散的 niche：一个平台有一簇插件，Codex 有零星一两个启动器，Claude 几乎空白，Muse 一个都没有。这个仓库把三家的概念收拢到一处，并保持它可魔改：单文件、代码可读、一切效果由代码生成。

## 路线图

- [ ] 给 README 顶部配上三版舞台的演示 GIF
- [ ] 把合成好的舞台导出为 MP4 / WebM / GIF（可直接用作 DSH 插件片头）
- [ ] 可下载素材包：角色 PNG + 舞台录制
- [ ] 分时段片头与片库轮换模式
- [ ] Codex / Claude 桌面版（Windows）独立启动器：全屏片头播完无缝交接给应用
- [ ] 更多品牌舞台与社区主题

## 授权

代码 MIT。`assets/` 中的角色立绘为本项目 AI 生成。通过 Wikimedia Commons / Openverse 获取的图片遵循其各自的单图授权，再利用前请查看每张图旁标注的授权信息。
