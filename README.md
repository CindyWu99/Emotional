# 安靜一下 — V2.1 iPhone PWA

## V2 主要修改
- 呼吸引導現在會自動開始；只有點擊「不想跟著節奏」才停止節奏提示。
- 「惡心的時候」改為「我胃不舒服」。
- Grounding 改成更生活化的觀察 / 觸覺 / 聲音任務，並且每次隨機抽取 4 個。
- 大幅增加安慰話，包含一般焦慮、身體不適、胃部不舒服、停止反覆檢查、逐漸緩下來等情境。
- Service Worker 更新為 V2，HTML 使用 network-first，方便你在 GitHub 分支持續測試新版，不容易被舊快取卡住。

## 發到 GitHub 分支
如果你的分支已經包含 V1，建議直接覆蓋：
- `index.html`
- `manifest.json`
- `service-worker.js`

`icons/` 可以沿用 V1；本 ZIP 也完整保留了一份。

提交後，如果是 GitHub Pages 的測試分支，要在 Pages 設定中把發布 Branch 切到對應分支。
如果仍看到舊版，可把主屏幕 App 完全關閉後重新打開；V2 service worker 啟用後會清理舊的 `quiet-calm-v1` 快取。

## 本地資料
收藏、設定和「我的安全角落」仍沿用原本相同的 LocalStorage key，因此覆蓋 V1 後不會主動清除你已保存的內容。


## V2.1
- 收藏按鈕移除白色背景，只保留稍微放大的愛心圖示；透明點擊區仍保留約 48px，方便 iPhone 觸控。
