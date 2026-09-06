# 澳洲 11 天 · v001

2026/9/17（四）－ 9/27（日）．4 人

## 上傳步驟

1. 到 https://github.com/bill7693782/australia
2. Add file → Upload files
3. **把這個資料夾裡的 6 個檔一起拖進去（不要拖資料夾本身）**
4. Commit changes
5. Settings → Pages → Branch 選 `main` `/ (root)` → Save
6. 等 1–3 分鐘，出現 https://bill7693782.github.io/australia/

## 檔名不能改

- `index.html` — GitHub Pages 靠這個名字決定開啟資料夾時給哪個檔
- `sw.js` — 路徑決定 Service Worker 的權限範圍
- `manifest.webmanifest` — index.html 內以相對路徑引用

## 跨專案隔離

與 bill7693782.github.io/osaka/ 同一個 origin，已做命名空間隔離：

| 項目 | 本專案 | 關西版 |
|:---|:---|:---|
| Cache Storage | `australia-v1` | `kansai5-v194` |
| localStorage | `australia_v1` | `kansai5_v3` |
| 備份碼前綴 | `AUBK` | `K5BK` |
| 同步碼前綴 | `AULG` | `K5` |
| Firebase | australia-2026-40745 | kansai-a631b |

`sw.js` 的 activate 只刪除 `australia-` 開頭的快取，fetch 全部使用
`caches.open(CACHE).then(c => c.match(req))`，不使用全域 `caches.match`。

## 上線後先做三件事

1. 開「分享」頁 — 會自動測 Firebase，規則沒設對會直接印出該貼的 JSON
2. 按「產生房號」，四支手機輸入同一組
3. 加到主畫面，之後可離線使用

## 尚未確認

- 9/19 大洋路上車點 — 打 03 8080 2288。該格已標「🚨 上車點待查」，
  查到後用 ⋯ → ✎ 改，不用重新上傳
- 9/20 導遊服務費金額 — 先按 AU$5／人備現金
