# Hi there

## About Me

我是資料科學系的學生。因為厭倦生活中重複且瑣碎的任務，我習慣把遇到的痛點轉化為開發專案——從跨平台的資訊分發到遊戲的無人值守腳本，只要能自動化的流程我都想動手實作。

目前專注於系統整合 (System Integration) 與自動化工作流 (Workflow Automation)。在開發過程中，我特別重視系統的容錯機制、例外排查 (Logging) 以及多執行緒效能優化，致力於寫出穩定且具備防呆架構的應用程式。

---

## My Projects

### [ImageBOT](https://github.com/NekoMaTA864/tg-to-discord-bot)
跨平台 Telegram to Discord 圖文分類與雲端分流管家。

- **Tech Stack:** `Python (asyncio)` `Telegram / Discord API` `boto3 (S3 API)` `FFmpeg`
- **工程亮點：** 
  - **資料聚合與路由：** 實作記憶體緩衝區解決社群相簿訊息破碎的問題，並透過 Regex 與 JSON 進行動態的頻道分發。
  - **雙軌大檔處理：** 整合 FFmpeg 實作 AMD 硬體加速影片壓縮（具備 CPU 降級備援機制），並透過 boto3 實作 Cloudflare R2 多執行緒分塊上傳 (Multipart Upload) 以突破社群平台的檔案限制。
- **進度：** 核心管線穩定運作中。目前正在實作 Cloudflare Workers 串流整合與 SQLite 紀錄持久化。

---

### [Chaos Bot](https://github.com/NekoMaTA864/CHAOS_BOT)
基於 OpenCV 與 ADB 的遊戲自動周回與資源收集腳本。

- **Tech Stack:** `Python` `OpenCV` `ADB` `PySide6 (QThread)`
- **工程亮點：** 
  - **架構解耦：** 實作 QThread 多執行緒，將 GUI 渲染與底層 OpenCV 畫面辨識、ADB 設備控制完美分離，解決傳統自動化腳本容易造成的 UI 阻塞問題。
  - **主動異常預防：** 捨棄被動報錯，內建 Watchdog 看門狗機制與狀態機邏輯。當連續辨識失敗時，系統會自動啟動喚醒機制，並擷取當下畫面與寫入 Log。
- **進度：** 穩定掛機運作中。目前正持續透過防呆機制收集失敗案例 (fail_cases)，計畫未來導入 TensorFlow 訓練專屬的動態環境辨識模型。

---

## Tech Stack

**Languages & Data**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**Libraries & Core Tools**
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![PySide6](https://img.shields.io/badge/PySide6-41CD52?style=flat-square&logo=qt&logoColor=white)
![boto3](https://img.shields.io/badge/boto3_(S3)-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white)

**DevOps & APIs**
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST_APIs-005571?style=flat-square&logo=fastapi&logoColor=white)

**Focus**
Automation / System Architecture / API Integration / Computer Vision
