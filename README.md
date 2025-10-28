[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/yOwut1-r)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=21327690&assignment_repo_type=AssignmentRepo)

# 🧠 Neurosynth Frontend - 神經科學術語查詢系統

這是一個使用 AJAX 技術和 Tailwind CSS 建立的 Neurosynth API 前端介面。

## 🌐 線上展示

### 方法 1：GitHub Pages
```
https://ntu-info.github.io/neurosynth-frontend-athenalin11/
```

### 方法 2：Netlify 部署
1. 訪問：https://app.netlify.com/drop
2. 將整個專案資料夾拖曳到頁面
3. 獲得即時部署的網址

## ✨ 功能特色

### 1. 顯示所有術語
- 自動載入所有可用的神經科學術語
- 美觀的卡片式佈局
- 點擊術語可快速查詢

### 2. 術語即時查詢（AJAX）
- ✅ **邊輸入邊查詢**（不需要按 Enter 或按鈕）
- 使用 debounce 優化效能（500ms）
- 即時顯示術語的詳細資訊

### 3. 研究邏輯搜尋（AJAX）
- ✅ **邊輸入邊搜尋**（不需要按 Enter 或按鈕）
- 支援布林邏輯運算：AND、OR、NOT
- 即時顯示符合條件的研究列表

### 4. 智慧備用系統
- 自動檢測 API 是否可用
- API 無法連線時自動切換到示範資料
- 確保功能展示不受 API 狀態影響

### 5. 美觀的使用者介面
- 使用 Tailwind CSS 美化
- 響應式設計（支援手機、平板、電腦）
- 漸層色彩和動畫效果
- 清晰的狀態提示和錯誤處理

## 🔧 本地開發

```bash
# 啟動本地伺服器
python3 -m http.server 8000

# 訪問
http://localhost:8000

# 測試 API
http://localhost:8000/test-api.html
```

## 📂 檔案說明

- `index.html` - 主頁面（包含智慧備用系統）
- `test-api.html` - API 測試工具
- `index-with-fallback.html` - 備用版本
- `index-original-backup.html` - 原始版本備份

## 🎯 API 端點

```
基礎網址：https://mil.psy.ntu.edu.tw:5000

/terms - 取得所有術語
/terms/<term> - 取得特定術語資訊
/query/<query>/studies - 邏輯搜尋研究
```

## 🚀 部署到 GitHub Pages

1. 進入 Repository Settings → Pages
2. Source 選擇：Deploy from a branch
3. Branch 選擇：main / (root)
4. 點擊 Save，等待 1-3 分鐘

## 📱 Netlify 部署（更簡單）

前往 https://app.netlify.com/drop，拖曳整個資料夾即可！

## 🐛 故障排除

- **API 無法連線**：系統會自動使用示範資料
- **本地測試**：必須使用 HTTP 伺服器
- **GitHub Pages 404**：等待 1-3 分鐘讓部署完成

## 👨‍💻 作者

Ariana Lin - NTU Information 課程作業 - 2025
