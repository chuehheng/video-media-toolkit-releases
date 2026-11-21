# CFI VR Player

這是公開安裝包下載專案，不需登入 GitHub。開發用的原始碼專案維持私有。

## 下載

請前往 [最新版本](https://github.com/chuehheng/video-media-toolkit-releases/releases/latest)。

| 系統 | 安裝包檔名結尾 |
| --- | --- |
| Windows x64 | `Windows-x64.zip` |
| Apple Silicon Mac | `macOS-arm64.zip` |
| Intel Mac | `macOS-x64.zip` |

Windows 請完整解壓縮，保留所有資料夾，執行「CFI VR Player.exe」。不要單獨移出 EXE。
Mac 請完整解壓縮並將 App 移到可寫入的位置；支援 macOS 15 或更新版本。目前 App 使用 ad-hoc 簽署，未經 Apple Developer ID 公證。

Player 使用獨立的 `major.minor.patch` 版號與 `CFI-VR-Player-<版本>-<平台>-<架構>.zip` 檔名。舊日期版號、Viewer 或影片音檔合併工具首次轉換需手動安裝一次。
正式可攜式版本可在啟動時自動查詢，點擊右上版號查看版本／建置號及手動安裝。自動查詢不會自動下載或關閉工具，安裝前需明確確認；影音工作及播放中禁止安裝。
每個安裝包附 SHA-256 校驗碼；影片簽章的私鑰不包含在安裝包內。

## 功能

- GPU 解碼：NVIDIA NVDEC、AMD D3D11VA、Intel QSV、macOS VideoToolbox，自動回退 CPU。AMD／macOS 尚待實機驗證。

- 360／180、Cubemap／EAC、一般平面及魚眼來源切換，支援單眼／SBS／TB 與左右眼選取。
- 透視／小行星／魚眼／全景展開，拖曳方向、滾輪縮放與全螢幕。
- 16K 圖片來源、2K／4K／8K 預覽快取，匯出原圖視角 PNG／JPG 或固定視角 MP4。
- Windows 以 mpv 硬體解碼及 GPU 投影同步播放音訊；Cubemap／EAC 與 FFmpeg 相容路徑維持 CPU 投影及靜音預覽。尚無球面標記轉存與原始雙魚眼拼接。
- 影片時間軸、毫秒時間碼、前後逐格；FOV／Super 35 等效焦段、CPU／GPU／FPS 資訊。
- F1／「？」查看快捷鍵說明，I／資訊圖示顯示或隱藏資訊，主畫面與全畫面同步。
- 替代影片音訊、抽出 Opus 音訊。
- 不重新編碼連接或切割影片。
- 影片 metadata 編輯、來源簽章及驗證。

FPS 相同不等於聲畫內容完全同步。外部音檔需自行確認與影片內容對齊。
公開提供安裝包不代表已授予開放原始碼授權；FFmpeg 等依賴套件另依上游授權條款。
