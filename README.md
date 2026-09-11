# 網站設計作品集

這份資料夾可直接上傳至 GitHub，作為 GitHub Pages 靜態網站。

首頁顯示 17 件作品縮圖；點選後進入獨立作品頁，圖片以瀏覽器內容區域的 100% 寬度呈現，依原比例顯示完整高度。上方「返回作品」可回到首頁對應作品。

## 在電腦上開啟

1. 先解壓縮 `portfolio-preview.zip`。
2. 開啟 `portfolio-preview` 資料夾。
3. 用瀏覽器開啟 `index.html`，即可查看首頁與所有作品。

使用純 HTML 與 CSS，沒有 JavaScript、CSS 自訂變數、外部字型或套件，也不需要安裝或編譯。

## 上傳 GitHub

1. 建立一個 GitHub repository，或開啟要放這份網站的 repository。
2. 將 `portfolio-preview` **資料夾裡面的所有檔案與子資料夾**上傳到 repository 最外層，並保留 `images`、`works` 的結構。請先解壓縮，不要只上傳 ZIP。最外層要能直接看到 `index.html`。
3. 到 repository 的 **Settings → Pages**。
4. 在 **Build and deployment → Source** 選擇 **Deploy from a branch**。
5. Branch 選擇你剛剛上傳的分支（通常是 `main`），資料夾選擇 **/ (root)**，按 **Save**。
6. 等 GitHub Pages 完成部署後，開啟 Pages 頁面顯示的網站網址，即可提供給客戶。

發佈來源設定可參考 [GitHub Pages 官方說明](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。

## 檔案用途

| 檔案或資料夾 | 用途 |
| --- | --- |
| `index.html` | 首頁與 17 張作品縮圖 |
| `style.css` | 首頁排版、手機版與全寬預覽樣式 |
| `images/` | 17 張作品原始 JPG，僅改為英文檔名 |
| `works/` | 17 個獨立作品預覽頁 |
| `favicon.png` | 瀏覽器分頁圖示 |
| `README.md` | 本說明 |

## 更換圖片或文字

圖片原檔完整保留，沒有壓縮、裁切或改色。首頁的縮圖裁切只透過 CSS 顯示圖片上方，作品頁則完整呈現。原始圖片寬度約 256–906px，若想提高桌面全寬預覽的清晰度，可使用更高解析度的原稿替換。

- 更換作品圖片：用相同檔名替換 `images` 裡的 JPG。若新圖比例不同，請同步更新首頁與對應作品頁 `<img>` 的 `width`、`height` 數值，使其等於新圖片的原始像素尺寸。CSS 仍會以 100% 寬度顯示。
- 更改首頁標題：編輯 `index.html` 的 `<h1>作品一覽</h1>`。
- 更改作品名稱：修改首頁該作品的文字與對應 `works` 頁面的標題、`alt` 及 `aria-label`。
- 圖片全寬設定：`style.css` 裡的 `.preview-image` 使用 `width: 100%; height: auto;`，外層沒有左右留白或最大寬度限制。

| 作品 | images 裡的檔名 |
| --- | --- |
| 水果行 | `fruit.jpg` |
| 滷味 | `braised-food.jpg` |
| 飲料行 01 | `drinks-01.jpg` |
| 飲料行 02 | `drinks-02.jpg` |
| 攝影 | `photography.jpg` |
| 植物 | `plants.jpg` |
| 健康餐 | `healthy-meals.jpg` |
| 貓舍 | `cattery.jpg` |
| 內褲 | `underwear.jpg` |
| 餐車 | `food-truck.jpg` |
| 模特兒 | `models.jpg` |
| 室內設計 | `interior-design.jpg` |
| 律師 | `lawyer.jpg` |
| 影像 | `film.jpg` |
| 音樂 | `music.jpg` |
| 機車 | `motorcycle.jpg` |
| 教練 | `coach.jpg` |
