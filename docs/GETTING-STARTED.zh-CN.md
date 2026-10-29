# 从一场喜欢的 Set 开始

[← 返回主页](../README.zh-CN.md) · [English](GETTING-STARTED.md)

DJ Set Tracker 是用于 YouTube 和 Bilibili 的桌面浏览器插件。建议使用当前版本的 Chrome 或 Edge。

## 商店安装

前往 [Chrome 应用商店](https://chromewebstore.google.com/detail/set-tracker/jdpgcgcbigjpgfheaimikbkmgdpkaaod) 或 [Edge 扩展商店](https://microsoftedge.microsoft.com/addons/detail/set-tracker/dicipdfdgkemhcflmngpgojnhoialnoj)，完成安装，再刷新已经打开的视频页。商店版本获批后，由浏览器按其机制更新。

## ZIP 安装

1. 打开 [最新 Release](https://github.com/BlackiePiggy/DJ-Set-Tracker/releases/latest)，在 **Assets** 中下载 **DJ-Set-Tracker-Chrome-Edge.zip**。不要下载 “Source code (zip)”。
2. 把 ZIP 解压到一个固定文件夹，例如 `DJ-Set-Tracker`。安装后也要保留这个文件夹。
3. Chrome 打开 `chrome://extensions`，Edge 打开 `edge://extensions`，开启 **开发者模式**。
4. 点击 **加载已解压的扩展程序 / Load unpacked**，选择含有 `manifest.json` 的解压文件夹。本安装包的 manifest 位于 ZIP 根目录。
5. 打开或刷新 YouTube / Bilibili 视频，点击右侧的 **SET TRACKER** 悬浮入口。

同一份 ZIP 适用于两个浏览器。商店版与手动加载版属于不同安装，可能有独立的本地数据，请避免同时启用两份。

## 使用第一份曲目表

1. 打开 DJ Set 视频，展开 SET TRACKER 面板。
2. 从歌单选择器中选一个已有版本。如果没有，进入 **Import / Sources（导入 / 来源）**。
3. 可以粘贴 1001Tracklists 歌单链接、扫描已加载的简介和评论，或导入文本 / CSV 曲目表。预览确认后再应用。
4. 播放视频，当前曲目会跟随进度高亮；点击其他曲目可以跳到对应时间。

扫描简介与评论前，先展开简介、加载需要扫描的评论。如果来源网站要求验证，请在来源页面正常完成验证后重试。

## 校准时间

同一场演出的不同上传版本可能有不同片头或剪辑。用快捷时间设置调整整体偏移，点击 **清零 / Reset** 恢复为零。正数表示把曲目起点延后。请检查多个位置：如果视频中途被剪切，仅调整一次整体偏移不能修复所有时间点。

## 收藏与贡献

在插件内登录后，可收藏歌曲和整份歌单，再从 **My library（我的收藏）** 找回。音乐平台入口有直接链接时打开该链接，否则发起搜索；不同平台不一定提供同一个 mix 或版本。

编辑器支持添加曲目、跟随播放标记起点。导入或匹配的歌名、艺人和时间都应在发布前检查。粘贴歌曲链接后会显示资料预览，点击 **使用封面和信息 / Use cover and details** 才会采用。导入或保存编辑草稿本身不会自动公开投稿。

## 更新 ZIP 安装

1. 阅读 [新版本说明](https://github.com/BlackiePiggy/DJ-Set-Tracker/releases/latest)，下载 ZIP。
2. 先把新版解压到临时文件夹；结束编辑并确认当前内容已保存。
3. 用新版文件替换 **上次加载插件时使用的那个固定文件夹** 中的插件文件，保持原文件夹路径不变。
4. 在 `chrome://extensions` 或 `edge://extensions` 中，点击原插件卡片的 **重新加载 / Reload**。
5. 刷新视频页，并在插件管理页确认版本号。

不要为了更新直接卸载插件：卸载可能清除本地草稿和设置。不同浏览器配置和不同插件 ID 的存储相互独立。GitHub ZIP 安装需要手动更新，不会自动收到 GitHub 的新安装包。

想收到新版提醒，可在仓库右上角选择 **Watch → Custom → Releases**。

## 常见问题

**没有悬浮入口？** 检查插件是否启用，刷新视频页，并使用桌面版 `www.youtube.com` 或 `www.bilibili.com` 视频页面；手机 App 不支持。浏览器也可能需要允许插件访问该视频网站。

**找不到这场 Set 的歌单？** 覆盖取决于现有来源和社区贡献，可以导入对应来源或自己整理。插件不会在后台听音并自动识别所有歌曲。

**时间点不准确？** 先确认歌单对应同一个录像和剪辑版本。固定延迟可用整体偏移修正，中途剪切则需要分别修正曲目时间。

**ID 没识别出来，或者没有音乐链接？** 未发布歌曲和特殊 edit 很常见，保留未知信息比替换成另一首歌更准确。匹配与搜索结果只是候选，请确认具体版本。

**商店版本和 GitHub 版本不同？** 两个商店有独立审核和更新节奏，以浏览器实际显示的版本为准。GitHub 已发布不代表商店也已经审核通过。

**如何核验下载？** 每个 Release 提供 `SHA256SUMS.txt`。macOS / Linux 可执行 `shasum -a 256 DJ-Set-Tracker-Chrome-Edge.zip`；Windows PowerShell 可执行 `Get-FileHash .\DJ-Set-Tracker-Chrome-Edge.zip -Algorithm SHA256`，将结果与文件中的哈希对比。

**仍有问题？** [提交 Issue](https://github.com/BlackiePiggy/DJ-Set-Tracker/issues/new/choose)，说明浏览器、插件版本、公开视频链接和复现步骤。不要提交密码、令牌或私人账户资料。[官网支持](https://djsettracker.live/support) · [隐私政策](https://djsettracker.live/privacy)。
