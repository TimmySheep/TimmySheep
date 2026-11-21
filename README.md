# Tim Huang · 黄天维

影像创作者，也写一些日常用的小软件。
Filmmaker and image-maker — I also build the small tools I want to use myself.

做纪录片与影像创作，也做本地优先的原生客户端：数据尽量留在设备上，不依赖账号与云同步。
I work on documentary and moving-image projects, and build local-first native clients — data stays on your device, with no account and no cloud sync.

**[timhuang.net](https://timhuang.net/)** · **[apps.timhuang.net](https://apps.timhuang.net/)** · **[words.timhuang.net](https://words.timhuang.net/)** · **[works.timhuang.net](https://works.timhuang.net/)**

---

## 主要项目 / Featured

### OpenTranslate · Safari 全页翻译
Safari 自带翻译覆盖的语言有限（例如芬兰语就不支持），这个扩展补上这块：约 32 个翻译提供方、页内双语对照渲染、设置全部保存在本机。
Safari's built-in translation covers few languages (Finnish, for one, is unsupported). This extension fills the gap: ~32 translation providers, in-page bilingual rendering, and settings stored entirely on-device.

`Swift` · `TypeScript` · 基于 [read-frog](https://github.com/mengxi-ream/read-frog)（GPL-3.0）· [介绍页](https://apps.timhuang.net/opentranslate/)

### Smart Shot · 只在画面变化时截图
录课、看直播、跟演示时，画面大部分时间是静止的。Smart Shot 用两级检测判断"这一帧有没有新内容"，只在真有变化时落盘，而不是按固定频率堆一堆重复图片。
While recording a lecture or following a demo the screen is mostly static. Smart Shot decides whether a frame actually carries new content and writes a file only when it does — instead of piling up duplicates on a timer.

`Swift` · `SwiftUI` · `ScreenCaptureKit` · MIT · [下载](https://github.com/TimmySheep/Smart-Shot/releases/latest)

### ulanzidial-native · Ulanzi D100H 原生客户端
给 Ulanzi D100H 旋钮控制器写的原生 macOS 客户端，约 1 MB 包体，没有 Electron、没有 Chromium。
A native macOS client for the Ulanzi D100H dial controller — around 1 MB, no Electron, no Chromium.

`Swift` · MIT

### Local Transcribe · 本地语音转写
把录音转成文字，全程留在本机，不上传音频。
Turns recordings into text without the audio ever leaving the machine.

[产品页](https://apps.timhuang.net/transcribe/zh/)

## 其他项目 / Others

| 项目 | 说明 | 语言 |
|---|---|---|
| [webspeak-ios](https://github.com/TimmySheep/webspeak-ios) · [webspeak-android](https://github.com/TimmySheep/webspeak-android) | WebSpeak（自托管 TeamSpeak 网页客户端）的原生 iPhone/iPad 与 Android 客户端 | Swift / Kotlin |
| [r6-lobby](https://github.com/TimmySheep/r6-lobby) | 小队集结看板：把参加意向与到场时间放在一起 | JavaScript |
| [R6ConfigBridge](https://github.com/TimmySheep/R6ConfigBridge) | 彩虹六号配置迁移工具，国际服与国服双向对照 | C# |
| [GainShark](https://github.com/TimmySheep/GainShark) · [sharkord-mic-gain](https://github.com/TimmySheep/sharkord-mic-gain) | Sharkord 的音频类插件 | TypeScript |
| [codexbar-ntfy](https://github.com/TimmySheep/codexbar-ntfy) | 把 CodexBar 的配额状况推到 ntfy | Python |
| [sharkord-next](https://github.com/TimmySheep/sharkord-next) | 兼容 Sharkord 的原生客户端（Android / iOS / watchOS） | TypeScript |

## 取向 / How I build

- **本地优先**：能留在设备上的数据，就不放到云上。
- **原生优先**：能在系统框架里做完的事，不为此引入一整个浏览器内核。
- **说清楚边界**：工具应该让人更清楚发生了什么，而不是用一个漂亮的界面盖住不确定性。

## 关于 fork / On forks

下面几个是上游项目的 fork，我在其上做适配与维护，作者与许可证以上游为准：

| 本仓库 | 上游 |
|---|---|
| [OpenTranslate](https://github.com/TimmySheep/OpenTranslate) | [mekedron/OpenTranslate](https://github.com/mekedron/OpenTranslate) |
| [FreeReps](https://github.com/TimmySheep/FreeReps) | [meltforce/FreeReps](https://github.com/meltforce/FreeReps) |
| [MicYou](https://github.com/TimmySheep/MicYou) | [MicYou-Dev/MicYou](https://github.com/MicYou-Dev/MicYou) |

---

<details>
<summary><b>English (full)</b></summary>

### What I do

Documentary and moving-image work, plus small local-first software. Most of the tools here are native clients for macOS, iOS and Android, built so that your data stays on your device.

### Featured projects

- **OpenTranslate** — a Safari web extension for full-page translation. Built on [read-frog](https://github.com/mengxi-ream/read-frog) (GPL-3.0). Supports roughly 32 translation providers, renders translations inline next to the original text, and stores settings locally.
- **Smart Shot** — a native macOS screenshot tool that saves a frame only when the picture actually changes, using a two-stage detector. MIT licensed.
- **ulanzidial-native** — a ~1 MB native macOS client for the Ulanzi D100H dial controller.
- **Local Transcribe** — on-device speech-to-text; audio never leaves the machine.

### Principles

Local-first by default; native frameworks before bundling a browser engine; and honest boundaries — a tool should make it clearer what happened, not hide uncertainty behind a polished UI.

</details>
