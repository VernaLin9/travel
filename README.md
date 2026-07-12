# 名古屋夏日之旅 9天8夜（防暑調整版）

單一檔案網頁（`index.html`），無任何外部相依，可直接放上 GitHub Pages。

## 功能
- **三種閱讀模式**：卡片（看重點）、時間軸（上午／正午／傍晚防暑節奏）、表格（總覽）
- **四個分頁**：每日行程、防暑對策、室內備案雷達、美食清單
- **響應式**：手機單欄、電腦多欄自動切換
- **列印版**：按右上「🖨️ 列印版」或 Ctrl+P，會輸出專用的精簡 A4 版面（含備案速查與裝備清單）

## 放上 GitHub Pages 的步驟

### 方法一：網頁拖曳上傳（最簡單，不用裝任何東西）
1. 到 <https://github.com/new> 建立新 repo，名稱例如 `nagoya-trip`，選 **Public**
2. 在 repo 頁面點 **uploading an existing file**，把 `index.html` 和 `README.md` 拖進去，按 **Commit changes**
3. 到 repo 的 **Settings → Pages**，Source 選 **Deploy from a branch**，Branch 選 `main` / `(root)`，按 **Save**
4. 等 1–2 分鐘，網址就是 `https://<你的帳號>.github.io/nagoya-trip/`

### 方法二：git 指令（本資料夾已初始化好）
```bash
git remote add origin https://github.com/<你的帳號>/nagoya-trip.git
git push -u origin main
```
然後同樣到 Settings → Pages 開啟即可。

## 修改行程
所有行程資料都集中在 `index.html` 內 `<script>` 開頭的 `DAYS`、`BACKUPS`、`FOODS` 三個陣列，直接改文字即可，不需要懂程式。
