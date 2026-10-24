# 影片音檔合併工具

這是公開安裝包下載專案，不需登入 GitHub。開發用的原始碼專案維持私有。

## 下載

請前往 [最新版本](https://github.com/chuehheng/video-media-toolkit-releases/releases/latest)。

| 系統 | 安裝包檔名結尾 |
| --- | --- |
| Windows x64 | `windows_x86_64.zip` |
| Apple Silicon Mac | `macOS_arm64.zip` |
| Intel Mac | `macOS_x86_64.zip` |

Windows 請完整解壓縮，保留所有資料夾，執行「影片音檔合併工具.exe」。不要單獨移出 EXE。
Mac 請完整解壓縮並將 App 移到可寫入的位置；支援 macOS 15 或更新版本。目前 App 使用 ad-hoc 簽署，未經 Apple Developer ID 公證。

從 `v2026.10.24.2` 起，程式內更新使用本公開專案，不需要 GitHub 權杖。
更舊版本仍指向私有下載來源，請先手動安裝新版一次。
每個安裝包附 SHA-256 校驗碼；影片簽章的私鑰不包含在安裝包內。

## 功能

- 替代影片音訊、抽出 Opus 音訊。
- 不重新編碼連接或切割影片。
- 影片 metadata 編輯、來源簽章及驗證。

FPS 相同不等於聲畫內容完全同步。外部音檔需自行確認與影片內容對齊。
公開提供安裝包不代表已授予開放原始碼授權；FFmpeg 等依賴套件另依上游授權條款。
