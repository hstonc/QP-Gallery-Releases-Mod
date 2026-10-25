# QuickPic Gallery Mod

[![Platform](https://img.shields.io/badge/android-platform?style=for-the-badge&label=platform&labelColor=21262d&color=6e7681)](https://www.android.com) [![API](https://img.shields.io/badge/26%2B-level?style=for-the-badge&logo=android&logoColor=3cd382&label=API&labelColor=21262d&color=ff663b)](https://developer.android.com/studio/releases/platforms) [![Release](https://img.shields.io/github/v/release/hstonc/QP-Gallery-Releases-Mod?display_name=tag&style=for-the-badge&logo=github&labelColor=21262d&color=1f6feb)](https://github.com/hstonc/QP-Gallery-Releases-Mod/releases/latest)

![alt text](https://raw.githubusercontent.com/WSTxda/QP-Gallery-Releases/master/Images/Banner.svg)

基於 QP Gallery 的非官方修改版本，保留原有介面與輕量、快速、離線優先的使用體驗，並加入功能與修復。最低需求為 Android 8.0（API 26）；目前僅在 Android 15／16 兩台實際設備上進行基本測試。

An unofficial modification of QP Gallery, preserving its existing interface and lightweight, fast, offline-first experience while adding features and fixes. Requires Android 8.0 (API 26) or later; basic testing has only been performed on two physical devices running Android 15 and Android 16.

<details>
  <summary>Screenshots</summary>

![Screenshot](https://raw.githubusercontent.com/WSTxda/QP-Gallery-Releases/master/Images/Screenshots.png)

</details>

> QP Gallery 的非官方 AI 輔助修改版本 / Unofficial AI-assisted modification of QP Gallery

[中文](#中文) | [English](#english) | [Downloads](https://github.com/hstonc/QP-Gallery-Releases-Mod/releases)

---

## 中文

### 關於本專案

這是一個基於 **QP Gallery** 的非官方修改版本。

由於原倉庫目前已較長時間沒有更新，我根據自己的日常使用習慣，對現有 APK 進行了一些功能修改、補充與問題修復。

本專案中的修改主要在 AI 協助下完成，包括 APK 反編譯、Smali / 資源修改、功能分析與重新打包，因此不保證所有修改都符合原專案的設計方式，也不能保證不存在未知問題。

目前僅在：

- Android 15
- Android 16

兩台實際設備上進行了基本功能測試。

其他 Android 版本、不同 ROM、平板、折疊屏以及特殊設備上的兼容性尚未完整驗證。

> **這不是官方版本，與原作者沒有關聯，也未獲得原作者背書。**

### 上游專案

原始專案：

**WSTxda/QP-Gallery-Releases**

https://github.com/WSTxda/QP-Gallery-Releases

---

### 功能與設定入口

相簿、閱讀及掃描相關開關主要在 **設定 → 檢視**；播放行為與字幕等選項在 **設定 → 影片播放器**。圖片編輯器的「移除 EXIF」位於右上角選單。部分基礎修復沒有獨立開關。

---

### 功能

- [x] 音量鍵翻頁
- [x] 快速切換圖庫
- [x] 閱讀記錄與閱讀進度
- [x] 自動掃描開關、下拉刷新與掃描快取
- [x] 相簿內單檔列表顯示類型、大小、解析度、日期及影片長度，未知資訊略過
- [x] 列表日期固定為 `yyyy/MM/dd`（例如 `2026/12/31`）
- [x] 按檔案類型排序
- [x] 單擊選取數量全選，長按反選
- [x] 刪除相簿後保留列表位置；圖片瀏覽返回時定位到最後查看的圖片

### 影片播放器

- [x] 全新播放器介面與手勢操作
- [x] 「開啟應用播放器」預設開啟；關閉後由 Android 處理，遵循系統預設，亦可選回本 App
- [x] 關閉直接內建播放時隱藏相簿自動開啟／返回及批次播放入口，字幕、字體、畫中畫、背景、亮度與恢復設定仍可用
- [x] SMB／FTP／SFTP 影片透過唯讀、可定位介面交給外部播放器
- [x] 點選播放速度標示直達調速側邊欄；字幕／音軌彈窗依內容縮小，長清單可捲動
- [x] 播放記錄、自動建立播放列表與多種播放順序
- [x] 自動開啟影片及返回列表選項
- [x] 遠端 HTTP 代理播放
- [x] 畫中畫播放與背景純音訊播放
- [x] 外置／內置字幕、ASS 特效及 `.danmu.ass` 彈幕字幕
- [x] 字幕字體匯入與管理
- [x] 依影片方向自動旋轉與安全音量
- [x] 更多的编解码器加入
- [x] 更完整的影片資訊、章節與播放進度
- [x] 漸變側邊欄：播放列表、詳細資料、播放速度與睡眠計時器
- [x] 影片優先使用可用硬體解碼器，失敗時保留位置並回退
- [x] 音訊優先保留來源取樣率與聲道，使用浮點 PCM，設備不接受時降級；支援匹配的同名 MKA 外掛音軌

### 圖片編輯器

- [x] 透過 Android 系統分享選單分享編輯完成的副本
- [x] 可移除輸出副本的 EXIF，另存副本，原圖保留

### 收藏夾

- [x] 建立與管理收藏夾

### 伺服器

- [x] SMB2／SMB3、FTP、SFTP 的唯讀圖片與影片瀏覽

### 修復與改善

- [x] 分享使用 Android 系統選單；改善選圖返回的類型／授權／順序，以及伺服器影片分享的持續讀取
- [x] 改善複製／移動媒體與包含／排除資料夾的路徑顯示
- [x] 修正列表模式日期、平板每列數量及檔案瀏覽標題
- [x] 可見縮圖優先載入、慢速載入完成通知及網路快取整理優化
- [x] 修正實體／虛擬資料夾閱讀標記；子資料夾繼承隱藏父目錄及 `.nomedia` 狀態
- [x] 改善巢狀與虛擬資料夾刪除，加入刪除確認及快速刪除
- [x] Android 9+ 生物識別及收藏夾鎖定；密碼／手勢改用加鹽慢雜湊，加入錯誤次數限制
- [x] Material You 配色開關預設關閉；Android 12+ 可使用系統強調色

---

### 安裝注意事項

從相同套件、相同 Mod 簽章更新至 10.3.0，可直接覆蓋安裝並保留資料；不需要先解除安裝或清除資料。

此 Mod 使用與原始版本不同的簽章，兩者通常無法直接覆蓋安裝。

第一次切換前，請先備份需要保留的資料，並確認備份能還原；解除安裝可能刪除應用程式資料。不要將解除安裝或清除資料作為一般更新步驟。

之後使用相同套件名稱、相同 Mod 簽章且 versionCode 符合 Android 更新要求的版本，才可直接覆蓋更新。

---

### 已知限制

- 修改主要基於反編譯 APK，並非完整的 Android 原始碼專案。
- 大部分分析與實作由 AI 輔助完成。
- 目前僅在 Android 15 與 Android 16 上進行基本測試。
- 不保證所有 Android 版本、廠商 ROM 與儲存配置均相容。
- 預設播放器由 Android 管理。第三方播放器須支援交接的 URI／定位方式；需要認證的 HTTP 代理來源須支援 byte ranges，不能保證所有串流或 NAS 都相容。
- EXIF／GPS 可讀性取決於原檔、來源提供者與 Android 權限或遮蔽行為。
- 其他已知限制與本次驗證範圍見。
- 未來上游更新可能需要重新調整這些修改。

回報問題時，請提供：

- Android 版本
- 裝置型號
- App 版本
- 重現步驟
- 可提供時，附上截圖或螢幕錄影

---

### 免責聲明

這是非官方修改版本。

本專案供個人使用、實驗與學習用途；使用風險由使用者自行承擔。

原始應用程式、名稱與相關素材的權利均屬各自權利人所有。

---

## English

### About

This is an **unofficial modification of QP Gallery**.

Since the original repository has not received updates for some time, I have made feature changes, additions, and fixes to the existing APK based on my everyday use.

Most modifications were made with AI assistance, including APK decompilation, Smali/resource editing, feature analysis, and repackaging. They may not follow the original project's design, and unknown bugs may remain.

Basic testing has only been performed on two physical devices running:

- Android 15
- Android 16

Compatibility with other Android versions, ROMs, tablets, foldables, and specialized devices has not been fully verified.

> **This is an unofficial build, unaffiliated with and not endorsed by the original developer.**

### Upstream

Original project:

**WSTxda/QP-Gallery-Releases**

https://github.com/WSTxda/QP-Gallery-Releases

---

### Features and settings

Album, reading, and scan toggles are mainly under **Settings → View**. Playback behavior and subtitle options are under **Settings → Video player**. The image editor's “Remove EXIF” option is in the top-right overflow menu. Some basic fixes have no separate toggle.

---

### Features

- [x] Volume-button paging
- [x] Quick album switching
- [x] Reading history and progress
- [x] Automatic scan toggle, pull-to-refresh, and scan cache
- [x] Media list rows show type, size, resolution, date, and video duration; unavailable information is omitted
- [x] List dates use `yyyy/MM/dd` (for example, `2026/12/31`)
- [x] File-type sorting
- [x] Tap the selection count to select all; long-press it to invert the selection
- [x] Keep the list position after deleting albums and return to the last viewed image when leaving the viewer

### Video player

- [x] Redesigned player interface and gesture controls
- [x] “Enable app player” is enabled by default; disable it to let Android open videos using system defaults, while keeping this app available as a choice
- [x] Disabling direct built-in playback hides album auto-open/return and batch playback actions; subtitles, fonts, PiP, background playback, brightness, and resume settings remain available
- [x] Read-only, seekable handoff of SMB/FTP/SFTP videos to external players
- [x] Tap the speed indicator to open the speed drawer; subtitle/audio track dialogs fit their content and scroll for longer lists
- [x] Playback history, automatic playlists, and multiple playback modes
- [x] Auto-open videos with an optional return-to-list flow
- [x] Remote HTTP-proxy playback
- [x] Picture-in-Picture and background audio playback
- [x] External and embedded subtitles, ASS effects, and `.danmu.ass` overlays
- [x] Subtitle font import and management
- [x] Orientation-aware rotation and safe volume
- [x] Support for more codecs
- [x] More complete video details, chapters, and playback progress
- [x] Gradient sidebar for the playlist, details, playback speed, and sleep timer
- [x] Prefer available hardware video decoders, with position-preserving fallback on failure
- [x] Prefer the source sample rate and channel layout with float PCM, falling back when unsupported by the device; support matching MKA sidecar audio tracks

### Image editor

- [x] Share the edited output copy through the Android system share sheet
- [x] Optionally remove EXIF from the exported copy while preserving the original

### Collections

- [x] Create and manage collections

### Servers

- [x] Read-only image/video browsing over SMB2/SMB3, FTP, and SFTP

### Fixes and improvements

- [x] Android system share sheet integration; improved types, permissions, and ordering for picker results, plus continued reading of shared server videos
- [x] Improved media copy/move actions and include/exclude folder path display
- [x] Fixed list-mode dates, tablet items-per-row settings, and file-browser titles
- [x] Visible-thumbnail priority, slow-load completion handling, and network cache maintenance improvements
- [x] Fixed physical/virtual-folder reading markers; subfolders inherit hidden-parent and `.nomedia` status
- [x] Improved nested and virtual folder deletion, with confirmation and quick delete
- [x] Android 9+ biometrics and collection access locking; salted slow hashing for passwords/patterns and failed-attempt throttling
- [x] Optional Material You system accents on Android 12+, disabled by default

---

### Installation notes

Update to 10.3.0 with the same package name and Mod signing certificate to preserve data. Uninstalling or clearing data first is unnecessary.

This Mod uses a different signing certificate from the original version, so they usually cannot be installed over each other.

Before switching for the first time, back up any data you need and confirm that it can be restored; uninstalling may delete app data. Do not treat uninstalling or clearing data as a routine update step.

Subsequent in-place updates require the same package name, the same Mod signing certificate, and a versionCode that meets Android's update requirements.

---

### Known limitations

- The modifications are based primarily on a decompiled APK rather than a complete Android source project.
- Most analysis and implementation were AI-assisted.
- Only basic testing has been performed on Android 15 and Android 16.
- Compatibility with every Android version, OEM ROM, and storage configuration is not guaranteed.
- Android manages default players. Third-party players must support the supplied URI and seeking behavior. Authenticated HTTP-proxy sources require byte ranges; compatibility with every stream or NAS is not guaranteed.
- EXIF/GPS availability depends on the original file, provider, and Android permissions or metadata redaction.
- For other known limitations and validation details, see the release notes.
- Future upstream updates may require these modifications to be adapted again.

When reporting an issue, please include:

- Android version
- Device model
- App version
- Steps to reproduce
- Screenshots or screen recordings when available

---

### Disclaimer

This is an unofficial modification.

It is provided for personal use, experimentation, and learning. Use it at your own risk.

All rights to the original application, name, and related assets belong to their respective owners.
