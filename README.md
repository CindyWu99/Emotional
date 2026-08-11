# 安靜一下 — iPhone PWA

## GitHub Pages 部署
1. 在 GitHub 新建一個 repository，例如 `quiet-calm`.
2. 把本 ZIP 解壓後的所有檔案上傳到 repository 根目錄。
3. 打開 Repository → Settings → Pages。
4. 在 Build and deployment 中選擇 `Deploy from a branch`。
5. Branch 選 `main`，Folder 選 `/(root)`，保存。
6. GitHub Pages 生成網址後，用 iPhone 的 Safari 打開。

## 添加到 iPhone 主屏幕
1. 一定要使用 Safari 打開 GitHub Pages 網址。
2. 點底部「分享」按鈕。
3. 選「加入主畫面 / Add to Home Screen」。
4. 確認名稱後加入。
5. 之後可像 App 一樣從主屏幕全屏打開。

## 離線
首次正常打開一次網站後，service worker 會緩存主要檔案。
之後即使暫時沒有網絡，主功能仍可使用。

## 文件
- `index.html`：完整 App
- `manifest.json`：PWA 設定
- `service-worker.js`：離線緩存
- `icons/`：iPhone / PWA 圖標
