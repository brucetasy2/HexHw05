# 網頁切版直播班 Gulp 範例

## 指令列表

- `gulp` - 執行開發模式(會開啟模擬瀏覽器並監聽相關檔案)
- `gulp build` - 執行編譯模式(不會開啟瀏覽器)
- `gulp clean` - 清除 dist 資料夾
- `gulp deploy` - 將 dist 資料夾部署至 GitHub Pages

## 說明
除了 Boostrap CSS 與 Boostrap JavaScript 需要掛 CDN 之外，本身已經內建打包 jQuery 3.5.1。
若有需要調整相關路徑參數可在 envOptions.js 中調整，但建議不要隨意調整導致 Gulp 無法正常運行。
假使對於 Gulp 不熟悉會建議不要任意調整 gulpfile.js 底下的資料任一檔案，避免出現無法正常運作之問題。

## 支援的監聽
目前支援 HTML、ejs、JavaScript、Images、SCSS 監聽並自動重新刷新。
圖片新增時也會自動刷新。

## 部署 gh-pagse 流程說明
部署前請務必先將該 Gulp 原始碼上傳到 GitHub Repositories 也就是初始化 GitHub，因此通常第一步驟會輸入以下指令
```cmd
git add .
git commit -m 'first commit'
git remote add origin [GitHub Repositories Url]
git push -u origin master // 僅限第一次輸入，往後只需要輸入 git push
```


https://xd.adobe.com/view/bd869667-ead5-4620-4329-ee0709cfef9e-cbb7/screen/94d39942-dfd2-4978-872a-8f826cd279c1/Modal-edit-full