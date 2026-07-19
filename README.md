# Naomi Su — Snowboard & Ski Instructor

Naomi 的滑雪教練求職網站。這是一個不需要建置流程的靜態網站，可直接由 GitHub Pages 發布。

## 檔案分流

- `index.html`、`assets/` 與證明檔：公開網站內容，會進入 Git。
- `source-materials/`：HEIC、MOV 與其他原始母檔，只保留在本機並由 `.gitignore` 排除。
- 公開照片已移除拍攝裝置、日期與 GPS 等 EXIF metadata。
- 公開影片已轉成 H.264/AAC MP4，移除定位與裝置 metadata，並啟用 fast start。

## 本機預覽

在此資料夾啟動任一靜態 HTTP server，並開啟 `index.html`。不要直接用 `file://` 測試影片。

## GitHub Pages

1. 將此 repository push 到 GitHub。
2. 到 repository 的 **Settings → Pages**。
3. 在 **Build and deployment** 選擇 **Deploy from a branch**。
4. Branch 選 `main`，folder 選 `/(root)`，再按 **Save**。

`.nojekyll` 會讓 GitHub Pages 原樣發布靜態檔案。若之後設定自訂網域，再新增 `CNAME`。
