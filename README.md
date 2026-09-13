# QuickPic Gallery Mod

[![Platform](https://img.shields.io/badge/android-platform?style=for-the-badge&label=platform&labelColor=21262d&color=6e7681)](https://www.android.com) [![API](https://img.shields.io/badge/23%2B-level?style=for-the-badge&logo=android&logoColor=3cd382&label=API&labelColor=21262d&color=ff663b)](https://developer.android.com/studio/releases/platforms) [![Release](https://img.shields.io/github/v/release/hstonc/QP-Gallery-Releases-Mod?display_name=tag&style=for-the-badge&logo=github&labelColor=21262d&color=1f6feb)](https://github.com/hstonc/QP-Gallery-Releases-Mod/releases/latest) 

![alt text](https://raw.githubusercontent.com/WSTxda/QP-Gallery-Releases/master/Images/Banner.svg)

A modernized version of the classic QuickPic Gallery, focused on speed, stability, and simplicity.
It includes multiple bug fixes, improved compatibility with recent Android versions, and a refreshed Material 3 design — while preserving the lightweight, fast, and offline-first experience of the original app.

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

### Upstream

Original project / 原始專案：

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
- [x] 排除過小圖片
- [x] 自動掃描開關、下拉刷新與掃描快取

## 影片播放器

- [x] 全新播放器介面與手勢操作
- [x] 播放記錄、自動建立播放列表與多種播放順序
- [x] 自動開啟影片及返回列表選項
- [x] 固定預設播放器與遠端 HTTP 代理播放
- [x] 畫中畫播放與背景純音訊播放
- [x] 外置／內置字幕、ASS 特效及 `.danmu.ass` 彈幕字幕
- [x] 字幕字體匯入與管理
- [x] 依影片方向自動旋轉與安全音量
- [x] MPEG-4 SP／ASP 等相容解碼
- [x] 更完整的影片資訊、章節與播放進度

## 修復與改善

- [x] 分享功能使用 Android 系統分享選單
- [x] 改善複製／移動媒體與包含／排除資料夾的路徑顯示
- [x] 修正列表模式日期、平板每列數量及檔案瀏覽標題
- [x] 改善資料夾及子資料夾縮圖載入
- [x] 修正實體／虛擬資料夾閱讀標記與 `.nomedia` 顯示
- [x] 改善巢狀與虛擬資料夾刪除，加入刪除確認及快速刪除

 ---

## 安裝注意事項

此 Mod 使用與原始版本不同的簽名。

因此第一次從官方 / 原始版本切換到本 Mod 時，可能需要先卸載原版本後再安裝。

之後如果一直使用同一個 Mod 簽名，則可以直接覆蓋更新。

> 請在卸載前確認需要保留的資料是否已備份。

---

## Disclaimer

This is an unofficial modification.

The project is provided for personal use, experimentation and learning purposes. Use it at your own risk.

All rights to the original application, name and related assets belong to their respective owners.

---

# English

## About

This is an **unofficial modification of QP Gallery**.

Since the original repository has not received updates for some time, I made several changes and fixes based on my own daily usage preferences.

Most modifications in this project were completed with the assistance of AI, including APK analysis, decompilation, Smali/resource editing, feature implementation and repackaging.

Because of this, the modifications may not follow the architecture or implementation style intended by the original developer, and unknown bugs may still exist.

The current build has only received basic testing on two physical devices running:

- Android 15
- Android 16

Compatibility with older Android versions, custom ROMs, tablets, foldables and other devices has not been fully tested.

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
- [x] Tiny-image exclusion
- [x] Automatic scan toggle, pull-to-refresh, and scan cache

## Video player

- [x] Redesigned controls and gesture navigation
- [x] Playback history, automatic playlists, and playback modes
- [x] Auto-open videos with an optional return-to-list flow
- [x] Default video associations and remote HTTP-proxy playback
- [x] Picture-in-Picture and background audio playback
- [x] External and embedded subtitles, ASS styling, and `.danmu.ass` overlays
- [x] Subtitle font import and management
- [x] Orientation-aware rotation and safe volume
- [x] Compatibility decoding including MPEG-4 SP/ASP
- [x] Richer video details, chapters, and playback progress

## Fixes and improvements

- [x] Android system share sheet integration
- [x] Improved media copy/move actions and include/exclude path display
- [x] Fixed list dates, tablet one-folder-per-row layout, and file-browser titles
- [x] Improved nested-folder thumbnail loading
- [x] Fixed reading markers for physical/virtual folders and `.nomedia`
- [x] Improved nested and virtual folder deletion with confirmation and quick delete

---

## Known Limitations

- The modifications are primarily based on a decompiled APK rather than a complete Android source project.
- A significant portion of the analysis and implementation was AI-assisted.
- Only basic testing has been performed on Android 15 and Android 16.
- Compatibility with every Android version, OEM ROM and storage configuration is not guaranteed.
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
