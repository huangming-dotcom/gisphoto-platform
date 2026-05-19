📸 Professional Field Survey Report System (專業現勘調查報告系統)
A lightweight, web-based GIS tool designed for field workers to spatializing photos, correcting coordinates, and generating professional PDF survey reports instantly.
一個輕量級的網頁版 GIS 工具，專為外業人員設計，用於照片空間化、座標動態校正，並能快速產生專業的現勘 PDF 報告書。
🌟 Key Features (功能亮點)
1. Automated Photo Mapping (自動照片空間化)
EXIF Data Extraction: Automatically reads GPS coordinates, timestamps, and camera heading (orientation) from uploaded photos.
自動提取元數據： 上傳照片後，系統會自動讀取 GPS 座標、拍攝時間及鏡頭方位角（Heading）。
2. Advanced Map Interaction (進階地圖互動)
Multi-BaseMaps: Toggle between OpenStreetMap (OSM) and Esri Satellite Imagery.
Heading Pointers: Every marker features a white pointer showing the exact direction the camera was facing.
Manual Correction: Draggable markers allow users to manually correct GPS offsets caused by signal interference.
Independent Clusters: Manual toggle for overlapping points. Expand one cluster without closing others to compare nearby stations.
多底圖切換： 支援 OpenStreetMap 標準地圖與 Esri 衛星影像切換。
方位指針： 每個點位均帶有白色三角形指針，直觀顯示拍照當下的鏡頭朝向。
手動校正： 支援點位拖拽功能，可手動修正因訊號干擾造成的 GPS 偏移。
獨立叢集控制： 獨家開發「手動展開/收合」叢集功能，點開一組重疊點後不會因操作其他區域而收縮，方便精細對照。
3. Professional PDF Reporting (專業現勘報表)
Overview Map: Generates a high-resolution snapshot of the survey area.
Smart Pagination: Automatically formats 4 photos per page to fit A4 layout, ensuring titles and notes are correctly displayed on every page.
Detailed Records: Includes Photo ID, Coordinates, Heading, Timestamp, and Field Notes.
總覽地圖： 自動擷取當前地圖範圍的高解析度畫面。
智慧分頁： 針對 A4 紙張優化，每頁自動排列 4 張照片，確保每一頁都有標題、編號與備註。
詳盡紀錄： 報表包含站號、座標、方位角、拍攝時間及現場備註。
4. Privacy & Performance (隱私與效能)
Client-Side Processing: All data is processed locally in the browser. No photos are uploaded to any server.
Image Compression: Automatically resizes high-res mobile photos to ensure smooth performance on low-end devices.
本地端處理： 所有操作均在瀏覽器內完成，照片不會上傳至伺服器，確保數據隱私。
自動壓縮： 內建壓縮引擎，自動將手機大圖優化，確保地圖縮放流暢不卡頓。
🚀 How to Use (使用說明)
Upload: Click the "📸 Import Photos" button. (Android users: Select "Files" to ensure GPS data is preserved).
Edit:
Click a marker to input Field Notes.
Drag a marker to correct its location.
Click a cluster (e.g., "2, 3") to expand overlapping points.
Export: Click "📄 Generate Report", review the layout, and click "Print / Save as PDF".
匯入： 點擊「📸 匯入照片」按鈕。（Android 用戶建議從「檔案」中選取以保留 GPS 資訊）。
編輯：
點擊點位可輸入 現勘筆記。
長按並拖動點位可 修正偏移位置。
點擊數字叢集（如 "2, 3"）可 展開/收合 重疊的點位。
匯出： 點擊「📄 產生現勘報告」，檢查預覽畫面後選擇「列印 / 存為 PDF」。
🛠 Tech Stack (技術架構)
Map Engine: Leaflet.js
Data Parsing: Exifr.js (GPS & Metadata)
Rendering: html2canvas (Map Snapshots)
Clustering: Leaflet.markercluster (Modified for Independent Toggling)
🔒 Privacy Disclaimer (資安聲明)
This tool is a purely client-side application. Your photos and field data stay on your device. Refreshing the page or closing the tab will clear all current data from memory.
本工具為 純前端應用程式。您的照片與現勘數據僅儲存在您的設備中，重新整理網頁或關閉分頁將會清除所有數據。
📄 License (授權)
This project is open-source. Feel free to use and modify for your field work needs.
本專案開放原始碼，歡迎根據您的現勘需求進行修改與使用。
