# TickLite

TickLite 是一款**免费的 Windows 桌面时间助手**：轻量、单文件、免安装。原生 Win32 实现，资源占用极低。

> 本工具当前**不开放源代码**。发布于本仓库的仅为可执行的便携版压缩包，供免费下载使用。

## 功能

- **桌面悬浮时钟** —— 逐像素透明，只有文字显示在桌面上；每秒更新；可鼠标穿透（点击穿过时钟，不挡下层窗口）；可始终置顶
- **番茄钟** —— 专注 / 休息倒计时（默认 45 + 15 分钟，可在配置文件中调整），计时状态与时钟联动
- **备忘提醒** —— 本地备忘录，到期自动弹窗提醒，重启后自动恢复
- **本地音乐播放器** —— 支持 MP3 / WAV / FLAC；播放列表可导入文件 / 文件夹、多选批量移除；进度条点击精确跳转；歌名超宽自动滚动；隐藏窗口后音乐继续播放
- **外观自定义** —— 内置设置窗口：文字颜色、字号、透明度、鼠标穿透与置顶开关

## 下载

前往 [Releases](https://github.com/se7enseal/TickLite-Releases/releases) 页面下载最新版：

- `TickLite_v1.0.0_Windows_x64.zip`（约 10 MB）

发布包内含 `TickLite.exe` 与自带白噪音 `Music\WhiteNoise.wav`，请保持目录结构完整。

## 使用方法

1. 解压到任意**可写**目录（如桌面、D:\Tools；不要放在 Program Files）
2. 运行 `TickLite.exe`，桌面出现悬浮时钟，托盘区出现图标
3. 右键托盘图标可打开：设置窗口、备忘录、本地音乐播放器，或退出

## 音乐目录说明

- 播放器默认使用 EXE 同目录下的 `Music\` 文件夹，首次运行自动创建
- 把你的音乐文件放入该目录后，在播放器中点"刷新列表"即可
- 首次启动的默认播放列表自带一条白噪音（`Music\WhiteNoise.wav`）

## 系统要求

- Windows 10 / 11（x64）
- 全部依赖为系统组件，无需安装运行库
- **Windows N/KN 精简版**缺少媒体功能，需先安装微软官方 [Media Feature Pack](https://support.microsoft.com/zh-cn/topic/media-feature-pack-list-for-windows-n-editions-c1c6fffa-d052-8338-7a79-a4bb980a700a)，否则音乐播放不可用

## 数据与隐私

- 所有数据仅保存在你的电脑上：
  - `TickLite.ini`（EXE 同目录）—— 外观与交互设置
  - `%LOCALAPPDATA%\TickLite\memos.json` —— 备忘内容
  - `%LOCALAPPDATA%\TickLite\playlist.json` —— 播放列表（仅本地文件路径）
- **无网络通信、无遥测、无账号体系**，不上传任何个人数据
