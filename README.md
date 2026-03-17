# 📦 盤點小工具 (Inventory Tool)

![Version](https://img.shields.io/badge/version-2.0-0ABAB5.svg)
![Platform](https://img.shields.io/badge/platform-Mobile%20Web-blue.svg)

一個專為行動裝置與單手操作設計的輕量級網頁盤點工具。完全運行於前端，無需架設後端伺服器，支援 Excel 匯入與條碼掃描，讓庫存盤點變得簡單高效。

## ✨ 核心功能 (Features)

* **📱 單手操作優化 (Mobile-First)**：懸浮相機按鈕與底部膠囊搜尋框，完美適配單手持機情境。具備智慧防遮擋機制，打字搜尋時畫面會自動避開虛擬鍵盤。
* **📷 智慧相機掃描**：內建高畫質條碼掃描功能，掃描成功自動 +1，並具備自動降級重試機制以確保舊機型相容性。
* **💾 本地自動儲存 (Auto-Save)**：利用瀏覽器 `localStorage` 實作自動存檔，意外重整或關閉網頁也不會遺失進度。
* **🎯 極簡專注介面**：自動隱藏數量已盤點正確的品項，頂部狀態儀表板恆常顯示「未完成數量」與「最後盤點物品」，減少視覺干擾。
* **📊 Excel 整合**：支援直接讀取 `.xlsx` / `.xls` 檔案匯入初始庫存資料。

## 🚀 使用方式 (Usage)

1.  **開啟工具**：以手機瀏覽器（推薦 Safari 或 Chrome）開啟 `index.html`。
2.  **匯入資料**：點擊右上角「📄 匯入」，選擇盤點清單的 Excel 檔案。
3.  **開始盤點**：
    * 點擊左下角「相機圖示」進行實體條碼掃描。
    * 點擊右下角「搜尋框」輸入代號手動修改數量。
4.  **PWA 支援**：強烈建議使用手機瀏覽器的「加入主畫面」功能，獲得全螢幕的 App 級體驗，且能獲得更穩定的本地儲存空間。

## 🛠️ 技術疊代 (Tech Stack)
* HTML5 / CSS3 / Vanilla JavaScript
* [SheetJS (xlsx.js)](https://github.com/SheetJS/sheetjs) - Excel 檔案解析
* [HTML5-QRCode](https://github.com/mebjas/html5-qrcode) - 鏡頭呼叫與條碼辨識
---
> Created by PJ | 2026
