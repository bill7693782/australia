# 澳洲 11 天 · v014

線上：https://bill7693782.github.io/australia/

## 上傳（7 個檔）
Add file → Upload files → 全部拖進去（不要拖資料夾）→ Commit

index.html / sw.js / manifest.webmanifest
icon-192.png / icon-512.png / icon-512-maskable.png / favicon.ico  ← 新增

## v013 → v014 修了什麼
分頁一直顯示灰色地球，因為 index.html 從來沒有 <link rel="icon">。
manifest 的圖示只管「加到主畫面」，不管瀏覽器分頁——那要靠 rel="icon"。
本版補上 rel="icon"、shortcut icon、apple-touch-icon，並附 favicon.ico 保底。

## 換了圖示還是舊的？
瀏覽器和系統會把圖示快取住。
・分頁圖示：強制重新整理，或關掉分頁重開
・主畫面圖示：移除再重新加一次
資料存在 localStorage，都不會消失。

## 四處版本號必須同步
header 版本鈕 ／ 說明頁「版本：vXXX」 ／ APPVER ／ sw.js 的 CACHE
🚨 分頁標題不放版本號。

## 與關西版的隔離
Cache `australia-v14` ／ localStorage `australia_v1`
備份碼 `AUBK` ／ 同步碼 `AULG` ／ Firebase australia-2026-40745

## 尚未確認
B、C、D 三位的 ETA 601 簽證（唯一沒做就走不了的）
