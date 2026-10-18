# QuickPic Gallery Mod

[![Platform](https://img.shields.io/badge/android-platform?style=for-the-badge&label=platform&labelColor=21262d&color=6e7681)](https://www.android.com) [![API](https://img.shields.io/badge/26%2B-level?style=for-the-badge&logo=android&logoColor=3cd382&label=API&labelColor=21262d&color=ff663b)](https://developer.android.com/studio/releases/platforms) [![Release](https://img.shields.io/github/v/release/hstonc/QP-Gallery-Releases-Mod?display_name=tag&style=for-the-badge&logo=github&labelColor=21262d&color=1f6feb)](https://github.com/hstonc/QP-Gallery-Releases-Mod/releases/latest)

![alt text](https://raw.githubusercontent.com/WSTxda/QP-Gallery-Releases/master/Images/Banner.svg)

基於 QP Gallery 的非官方修改版本，保留原有介面與輕量、快速、離線優先的使用體驗，並加入功能與修復。最低需求為 Android 8.0（API 26）；目前僅在 Android 15／16 兩台實際設備上進行基本測試。

An unofficial modification of QP Gallery, preserving its existing interface and lightweight, fast, offline-first experience while adding features and fixes. Requires Android 8.0 (API 26) or later; basic testing has only been performed on two physical devices running Android 15 and Android 16.

<details>
  <summary>Screenshots</summary>

![Screenshot](https://raw.githubusercontent.com/WSTxda/QP-Gallery-Releases/master/Images/Screenshots.png)

</details>

# QP Gallery Mod

> Unofficial AI-assisted modification of QP Gallery  
> QP Gallery 的非官方 AI 輔助修改版本

[中文](#中文) | [English](#english)

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

## Mod 功能開關

本 Mod 增加或調整的主要功能可以在：

**設定 → 檢視（Settings → View）**

中開啟或關閉。部分修復屬於基礎行為修正，可能不提供獨立開關。

---

## 功能

- [x] 音量鍵翻頁
- [x] 快速切換圖庫
- [x] 閱讀記錄與閱讀進度
- [x] 自動掃描開關、下拉刷新與掃描快取

## 影片播放器

- [x] 全新播放器介面與手勢操作
- [x] 播放記錄、自動建立播放列表與多種播放順序
- [x] 自動開啟影片及返回列表選項
- [x] 遠端 HTTP 代理播放
- [x] 畫中畫播放與背景純音訊播放
- [x] 外置／內置字幕、ASS 特效及 `.danmu.ass` 彈幕字幕
- [x] 字幕字體匯入與管理
- [x] 依影片方向自動旋轉與安全音量
- [x] MPEG-4 SP／ASP 等相容解碼
- [x] 更完整的影片資訊、章節與播放進度
- [x] 漸變側邊欄：播放列表、詳細資料、播放速度與睡眠計時器
- [x] 影片優先使用可用硬體解碼器，失敗時保留位置並回退
- [x] 音訊優先保留來源取樣率與聲道，使用浮點 PCM，設備不接受時降級；支援匹配的同名 MKA 外掛音軌

## 收藏夾

- [x] 新增收藏夾功能

## 伺服器

- [x] SMB2／SMB3、FTP、SFTP 的唯讀圖片與影片瀏覽

## 修復與改善

- [x] 分享功能使用 Android 系統分享選單
- [x] 改善複製／移動媒體與包含／排除資料夾的路徑顯示
- [x] 修正列表模式日期、平板每列數量及檔案瀏覽標題
- [x] 改善資料夾及子資料夾縮圖載入
- [x] 修正實體／虛擬資料夾閱讀標記與 `.nomedia` 顯示
- [x] 改善巢狀與虛擬資料夾刪除，加入刪除確認及快速刪除
- [x] Android 9+ 生物識別及收藏夾鎖定；密碼／手勢改用加鹽慢雜湊，加入錯誤次數限制
- [x] Material You 配色開關預設關閉；Android 12+ 可使用系統強調色

---

## 安裝注意事項

此 Mod 使用與原始版本不同的簽章，兩者通常無法直接覆蓋安裝。

第一次切換前，請先備份需要保留的資料，並確認備份能還原；解除安裝可能刪除應用程式資料。不要將解除安裝或清除資料作為一般更新步驟。

之後使用相同套件名稱、相同 Mod 簽章且 versionCode 符合 Android 更新要求的版本，才可直接覆蓋更新。

---

## 已知限制

- 修改主要基於反編譯 APK，並非完整的 Android 原始碼專案。
- 大部分分析與實作由 AI 輔助完成。
- 目前僅在 Android 15 與 Android 16 上進行基本測試。
- 不保證所有 Android 版本、廠商 ROM 與儲存配置均相容。
- 外部預設播放器的「一律開啟」支援仍暫緩，不列為已完成功能。
- 未來上游更新可能需要重新調整這些修改。

回報問題時，請提供：

- Android 版本
- 裝置型號
- App 版本
- 重現步驟
- 可提供時，附上截圖或螢幕錄影

---

## 免責聲明

這是非官方修改版本。

本專案供個人使用、實驗與學習用途；使用風險由使用者自行承擔。

原始應用程式、名稱與相關素材的權利均屬各自權利人所有。

---

## English

## About

This is an **unofficial modification of QP Gallery**.

Since the original repository has not received updates for some time, I made several changes and fixes based on my own daily usage preferences.

Most modifications in this project were completed with the assistance of AI, including APK analysis, decompilation, Smali/resource editing, feature implementation and repackaging.

Because of this, the modifications may not follow the architecture or implementation style intended by the original developer, and unknown bugs may still exist.

The current build has only received basic testing on two physical devices running:

- Android 15
- Android 16

Compatibility with other Android versions, custom ROMs, tablets, foldables and other devices has not been fully tested.

> **This is not an official build and is not affiliated with or endorsed by the original developer.**

### Upstream

Original project:

**WSTxda/QP-Gallery-Releases**

https://github.com/WSTxda/QP-Gallery-Releases

---

## Mod Feature Toggles

Most features added or changed by this Mod can be enabled or disabled under:

**Settings → View**

Some fixes are basic behavior corrections and may not have a separate toggle.

---

## Features

- [x] Volume-button paging
- [x] Quick album switching
- [x] Reading history and progress
- [x] Automatic scan toggle, pull-to-refresh, and scan cache

## Video player

- [x] Redesigned controls and gesture navigation
- [x] Playback history, automatic playlists, and playback modes
- [x] Auto-open videos with an optional return-to-list flow
- [x] Remote HTTP-proxy playback
- [x] Picture-in-Picture and background audio playback
- [x] External and embedded subtitles, ASS styling, and `.danmu.ass` overlays
- [x] Subtitle font import and management
- [x] Orientation-aware rotation and safe volume
- [x] Compatibility decoding including MPEG-4 SP/ASP
- [x] Richer video details, chapters, and playback progress
- [x] Gradient drawer for the playlist, details, playback speed and sleep timer
- [x] Prefer available hardware video decoding with position-preserving fallback
- [x] Prefer source-rate/channel float PCM with device-compatible fallbacks, and select matching MKA sidecar tracks

## Collections

- [x] Added Favorites feature

## Servers

- [x] Read-only image/video browsing over SMB2/SMB3, FTP and SFTP

## Fixes and improvements

- [x] Android system share sheet integration
- [x] Improved media copy/move actions and include/exclude path display
- [x] Fixed list-mode dates, tablet items-per-row settings, and file-browser titles
- [x] Improved folder and subfolder thumbnail loading
- [x] Fixed reading markers for physical/virtual folders and `.nomedia`
- [x] Improved nested and virtual folder deletion with confirmation and quick delete
- [x] Android 9+ biometrics and collection access locking; salted slow hashing for passwords/patterns and failed-attempt throttling
- [x] Optional Material You accents, off by default, on Android 12+

---

## Installation Notes

This Mod uses a different signing certificate from the original version, so the two usually cannot be installed over each other.

Before switching for the first time, back up any data you need and confirm that it can be restored; uninstalling may delete app data. Do not treat uninstalling or clearing data as a routine update step.

Subsequent in-place updates require the same package name, the same Mod signing certificate, and a versionCode that meets Android's update requirements.

---

## Known Limitations

- The modifications are primarily based on a decompiled APK rather than a complete Android source project.
- A significant portion of the analysis and implementation was AI-assisted.
- Only basic testing has been performed on Android 15 and Android 16.
- Compatibility with every Android version, OEM ROM and storage configuration is not guaranteed.
- External default-player “Always open” support remains deferred and is not listed as a completed feature.
- Future upstream releases may require these modifications to be adapted again.

When reporting an issue, please include:

- Android version
- Device model
- App version
- Steps to reproduce
- Screenshots or screen recordings when possible

---

## Disclaimer

This is an unofficial modification.

It is provided for personal use, experimentation and learning purposes. Use it at your own risk.

All rights to the original application, name and related assets belong to their respective owners.
