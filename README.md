# duct-calculator
靜電機&amp;量子網前後風管計算
靜電機擴管縮管規範計算小程式 - GitHub Pages 版本
此資料夾已整理成可部署到 GitHub Pages 的純靜態網站版本。

檔案內容
index.html：主網頁，已內嵌 CSS、JavaScript 與原 Excel 附圖。
.nojekyll：避免 GitHub Pages 以 Jekyll 處理，維持純靜態 HTML。
.github/workflows/pages.yml：若你選擇 GitHub Actions 部署，可直接使用此 workflow。
方法 A：Deploy from a branch，最簡單
建立 GitHub repository。
把本資料夾內所有檔案上傳到 repository 根目錄。
到 repository 的 Settings > Pages。
Source 選 Deploy from a branch。
Branch 選 main，Folder 選 / (root)，儲存。
GitHub Pages 產生網址後，即可分享給別人。
方法 B：GitHub Actions 部署
把本資料夾內所有檔案上傳到 repository 根目錄。
到 repository 的 Settings > Pages。
Source 選 GitHub Actions。
推送到 main 後，.github/workflows/pages.yml 會部署此靜態網站。
預期網址格式
如果 repository 名稱為 duct-calculator，你的網址通常會類似：

https://你的GitHub帳號.github.io/duct-calculator/

若 repository 名稱是 你的GitHub帳號.github.io，網址通常會是：

https://你的GitHub帳號.github.io/

本機測試
直接用 Edge 或 Chrome 開啟 index.html 即可測試。

驗證重點
輸入 a、b、c、d 可即時計算 D1D3、L1L6。
預設範例值 a=113、b=66、c=64、d=64、D2=115。
已修正 JavaScript 字串換行造成的 SyntaxError。
原始公式圖與配置示意圖已保留於 HTML 中。
