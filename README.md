# 澳洲 11 天 · v013

線上：https://bill7693782.github.io/australia/

## 上傳（6 個檔全部）
Add file → Upload files → 把這 6 個檔一起拖進去（不要拖資料夾）→ Commit

index.html / sw.js / manifest.webmanifest
icon-192.png / icon-512.png / icon-512-maskable.png

## 這一版改了什麼
- 分頁標題拿掉版本號，改成單純「澳洲 11 天」
- 圖示重做：眼睛加高光、鼻子縮小成橢圓、耳朵實心加內耳、臉加下巴
- 沒有導航目標的行程格不再顯示「帶我去」

## 圖示換了看不到？
瀏覽器和系統會把圖示快取住。移除主畫面圖示再重新加一次即可。
資料存在 localStorage，不會消失。

## 四處版本號必須同步（依補充規格）
header 版本鈕 ／ 說明頁「版本：vXXX」 ／ APPVER ／ sw.js 的 CACHE
分頁標題不放版本號。

## 與關西版的隔離
Cache `australia-v13` ／ localStorage `australia_v1`
備份碼 `AUBK` ／ 同步碼 `AULG` ／ Firebase australia-2026-40745

## 尚未確認
B、C、D 三位的 ETA 601 簽證（唯一沒做就走不了的）
