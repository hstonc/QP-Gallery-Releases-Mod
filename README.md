# QuickPic Gallery Mod

[![Platform](https://img.shields.io/badge/android-platform?style=for-the-badge&label=platform&labelColor=21262d&color=6e7681)](https://www.android.com) [![API](https://img.shields.io/badge/23%2B-level?style=for-the-badge&logo=android&logoColor=3cd382&label=API&labelColor=21262d&color=ff663b)](https://developer.android.com/studio/releases/platforms) [![Release](https://img.shields.io/github/v/release/WSTxda/QP-Gallery-Releases?display_name=tag&style=for-the-badge&logo=github&labelColor=21262d&color=1f6feb)](https://github.com/hstonc/QP-Gallery-Releases-Mod/releases/latest) [![Downloads](https://img.shields.io/github/downloads/WSTxda/QP-Gallery-Releases/total?style=for-the-badge&labelColor=21262d&color=238636)](https://github.com/hstonc/QP-Gallery-Releases-Mod/releases)

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

## 新增與修改的功能

### 音量鍵翻頁

可以使用：

- 音量 +
- 音量 -

進行上一張 / 下一張圖片切換。

方便在單手操作、全螢幕閱讀漫畫或瀏覽大量圖片時使用。

---

### 快速切換上一個 / 下一個圖庫

當位於目前圖庫邊界時，可以直接切換到相鄰圖庫。

- 在**第一張圖片**繼續執行兩次「上一頁」操作 → 開啟上一個圖庫
- 在**最後一張圖片**繼續執行兩次「下一頁」操作 → 開啟下一個圖庫

支援的操作包括：

- 觸控滑動
- 鍵盤方向鍵
- 音量鍵

為避免誤觸，同一次滑動手勢只會計算一次，必須真正執行第二次操作才會切換圖庫。

切換至：

- 下一個圖庫時，從第一張開始
- 上一個圖庫時，從最後一張開始

---

### 閱讀進度記錄

增加 / 調整了圖庫閱讀進度記錄。

圖庫可以記錄上次閱讀到的位置。

再次點擊圖庫時：

- 沒有閱讀記錄 → 從第一張開始
- 有閱讀記錄 → 從上次閱讀位置繼續

切換去其他圖庫不會直接刪除目前圖庫的觀看記錄。

---

### 已看完狀態可以重新變回閱讀中

原本圖庫一旦被標記為「已看完」，之後重新閱讀時仍會一直保持完成狀態。

現在重新閱讀已完成的圖庫時：

- 剛重新打開時仍保持「已看完」
- 當重新閱讀到中間位置後，會自動恢復為「閱讀中 / 看一半」
- 同時重新保存目前閱讀位置

如果仍位於設定的完成區域，則繼續保持已看完狀態。

---

## 修復與改善

### 分享功能

修復圖片分享行為。

現在分享圖片時會正常調用 **Android 系統分享選單**，可以選擇其他應用程式進行分享。

---

### 移動 / 複製圖片到資料夾

增加將圖片：

- 移動到其他圖庫
- 複製到其他圖庫
- 移動到系統資料夾
- 複製到系統資料夾

的相關操作。

部分選單文字也進行了縮短，以減少介面佔用空間。

---

### 修復包含 / 排除資料夾路徑選擇

修復掃描設定中：

- 包含資料夾
- 排除資料夾

的目錄選擇與路徑處理問題。

改善本機儲存空間及 SD 卡目錄的掃描行為。

---

### 優化鍵盤操作

改善實體鍵盤 / 遙控器方向鍵操作圖片時的邏輯。

修復方向鍵切換圖片前，圖片本身會先取得焦點的問題。

同時處理 Android 預設 Focus Highlight，避免圖片上出現白色半透明焦點遮罩。

方向鍵現在會更直接地作為上一張 / 下一張操作使用。

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

## Added / Modified Features

### Volume Button Navigation

The volume buttons can now be used to navigate between images.

- Volume Up
- Volume Down

can be used as previous / next page controls.

This is especially useful for one-handed browsing, fullscreen reading and image-heavy galleries.

---

### Quick Previous / Next Gallery Navigation

When reaching the boundary of the current gallery:

- Perform **Previous Page twice** on the first image → open the previous gallery
- Perform **Next Page twice** on the last image → open the next gallery

Supported input methods include:

- Touch gestures
- Keyboard arrow keys
- Volume buttons

To prevent accidental activation, multiple callbacks generated by the same swipe gesture are counted as only one operation.

A real second gesture or button press is required before switching galleries.

When switching:

- The next gallery opens from its first image
- The previous gallery opens from its last image

---

### Reading Progress

Gallery reading progress is now stored.

When opening a gallery:

- No saved progress → open the first image
- Saved progress available → resume from the previous reading position

Opening another gallery no longer automatically removes the previous gallery's reading position.

---

### Completed Galleries Can Return to In-Progress State

Previously, once a gallery was marked as completed, it could remain permanently completed even after starting to read it again.

Now, when reopening a completed gallery:

- It initially remains marked as completed
- After reading back into the middle of the gallery, it automatically returns to an in-progress state
- The new reading position is saved again

If the current image is still within the configured completion range, the gallery remains completed.

---

## Fixes and Improvements

### System Share Sheet

Fixed image sharing behavior.

Sharing an image now correctly opens the **Android system share sheet**, allowing the image to be sent to other compatible apps.

---

### Move / Copy Images

Added or improved support for:

- Move to another gallery
- Copy to another gallery
- Move to a system folder
- Copy to a system folder

Some menu labels were also shortened to reduce UI clutter.

---

### Include / Exclude Folder Path Selection

Fixed folder selection and path handling for:

- Included folders
- Excluded folders

This also improves scanning behavior for internal storage and SD card directories.

---

### Keyboard Navigation Improvements

Improved navigation behavior when using a physical keyboard or directional controls.

Fixed an issue where the image view would receive focus before the arrow key navigation was processed.

Android's default focus highlight was also disabled for the image viewer, preventing the white translucent overlay from appearing during keyboard navigation.

Arrow keys now behave more directly as previous / next image controls.

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
