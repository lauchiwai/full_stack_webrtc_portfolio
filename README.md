# 🚀 WebRTC 視訊通話與媒體處理全端專案

這是一個由我獨立開發的全端專案，整合了高品質的 WebRTC 視訊通話、信令交換、設備管理與媒體處理（錄影、轉檔）功能。專案清晰展示了從前端 UI 互動、後端信令協調到媒體處理的完整技能。

## 📁 專案架構與倉庫連結

本專案由兩個核心部分構成，點擊連結查看各部分的詳細程式碼與說明：

| 服務名稱 | 技術堆疊 | 倉庫連結 | 核心功能 |
| :--- | :--- | :--- | :--- |
| **信令與媒體後端服務** | Node.js, Express, Socket.io, FFmpeg | [webrtc_nodejs](https://github.com/lauchiwai/webrtc_nodejs) | WebRTC 信令交換 (Offer/Answer/ICE)、房間管理、WebM 至 MP4 影片轉換 |
| **前端視訊應用** | Vue 3, TypeScript, Pinia, Ant Design Vue | [webrtc_vue](https://github.com/lauchiwai/webrtc_vue) | 視訊通話界面、設備管理、遠端畫面錄製與截圖、即時連線狀態監控 |

## 🛠️ 技術亮點 (Technical Highlights)

### 🔐 通訊與協商
- **完整 WebRTC 信令流程**: 基於 Socket.io 實作穩定的信令伺服器，可靠地處理 `offer`, `answer`, `ICE candidate` 的交換與協商。
- **房間管理機制**: 實現簡單高效的房間號系統，讓用戶能輕鬆加入同一個通話 session。

### 🎥 媒體與設備控制
- **動態設備管理**: 前端可動態偵測、列舉並切換音訊輸入設備，提供無縫的設備更換體驗。
- **媒體軌道控制**: 獨立控制音頻與視頻軌道的啟用/禁用，實現靜音、關閉鏡頭等功能。
- **進階媒體處理**: 實作 `MediaRecorder API` 進行遠端畫面錄製與多格式輸出，並提供即時畫面截圖功能。

### ⚙️ 後端媒體處理
- **FFmpeg 整合**: 後端服務整合 FFmpeg，提供將前端錄製的 WebM 格式影片轉換為通用性更高的 MP4 格式之服務。
- **RESTful API 設計**: 提供清晰的 API 端點 (`/convert`) 用於提交轉檔任務與下載轉換後的檔案。

### 🚀 前端架構與體驗
- **現代化前端堆疊**: 採用 Vue 3 與 TypeScript 構建類型安全的組件，使用 Pinia 進行清晰的可響應式狀態管理。
- **優質使用者介面**: 基於 Ant Design Vue 組件庫開發，提供專業且直覺的用戶操作界面。
- **即時狀態反饋**: 在 UI 上清晰展示連線狀態、錄影計時等資訊，確保用戶知情權。
