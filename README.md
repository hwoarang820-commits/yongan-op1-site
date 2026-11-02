# 永安新村都更案・方案一 — GitHub Pages 發布說明

本包使用最新「TOD範圍面更新預覽」版本，保留五項TOD的深藍標籤、下引線與半透明淺紅色範圍面。

## 檔案
- index.html：完整網站，已內嵌模型、貼圖與分析資料。
- .nojekyll：停用Jekyll處理，直接發布靜態檔案。
- README.md：本操作說明。

不需要另行上傳SKP、GLB或其他模型檔案。不需要安裝開發工具或執行建置。

## 1. 建立新的儲存庫
1. 登入 https://github.com/ ，右上角「+」→「New repository」。
2. Owner選擇自己的帳號。
3. Repository name填入 yongan-op1-site；若已有同名儲存庫，另取新名稱。
4. Description可填「永安新村都更案方案一｜基地環境互動分析」。
5. 使用GitHub Free時，選Public才能使用此Pages發布方式。這代表原始檔與內嵌模型可被公眾存取。
6. 開啟Add README（或Add a README file），讓main分支先建立；其他項目維持預設。
7. 點Create repository。

## 2. 上傳檔案
1. 先將下載的ZIP解壓縮；不要直接上傳ZIP。
2. 在新儲存庫的Code頁點Add file → Upload files。
3. 上傳解壓縮後的index.html、.nojekyll與README.md三個檔案，讓它們位於儲存庫最上層。不要把外層資料夾一起拖入。
4. Commit訊息可填「Publish Yongan OP1 site」。選直接提交至main，點Commit changes。
5. 回到Code頁確認可直接看到index.html。首頁不可更名為index.html.txt，也不要放到子資料夾。

## 3. 啟用GitHub Pages
1. 在儲存庫上方點Settings。
2. 左側選Pages。
3. Build and deployment區塊的Source選Deploy from a branch。
4. Branch選main，右側資料夾選/ (root)。
5. 點Save。不需要填Custom domain。
6. 等待發布；GitHub官方說明變更最多可能需要10分鐘。
7. 到Actions查看pages build and deployment工作是否成功，再回Settings → Pages點Visit site或開啟顯示的網址。

## 4. 網址與驗收
一般專案網站網址：https://你的GitHub帳號.github.io/yongan-op1-site/
若仍使用hwoarang820-commits帳號，且儲存庫名稱確實為yongan-op1-site，預期網址為：
https://hwoarang820-commits.github.io/yongan-op1-site/
這是預期格式，並不代表網站已發布；以Pages頁面顯示的網址為準。

開啟網站後確認：
- 案名為方案一，模型及材質正常載入。
- 綠化與庭園有五項TOD深藍標籤、下引線、淺紅色半透明範圍面與外框。
- 旋轉、縮放模型後，範圍面跟隨模型。
- 其他分析章節可切換，手機直向畫面可操作。

## 5. 日後更新
1. 取得新版完整HTML，將檔名改為index.html。
2. 在同一個儲存庫的Code頁點Add file → Upload files。
3. 上傳新版index.html到原本位置，提交至main；同名檔案會被更新。
4. 等待Actions發布成功，再重新整理網站。若仍看到舊版，Windows可用Ctrl+F5或無痕視窗查看。
5. 不必重建儲存庫或重設Pages；維持相同儲存庫名稱即可保留網址。

## 常見問題
- 404：確認發布完成、Source為Deploy from a branch、Branch為main、資料夾為/ (root)，且index.html在儲存庫最上層。
- 看見README文字而非模型：確認index.html確實已上傳，名稱及所在位置正確。
- main無法選取：先提交至少一個檔案或README，再回Pages設定。
- 上傳ZIP後沒有網站：GitHub不會自動解壓，請上傳ZIP裡的三個檔案。
- 更新後沒變：先確認Actions成功，再用Ctrl+F5或無痕視窗查看。
- 模型未顯示：使用近期版本Chrome或Edge，確認WebGL可用且index.html上傳完整。

## 驗證狀態
發布版index.html與最新預覽內容逐位元相同；模型、貼圖與分析資料內嵌。先前已完成語法、邊界資料與多視角繪製邏輯檢查。本次未代為建立GitHub儲存庫或發布，仍需依上述步驟操作並驗收線上畫面。

## GitHub官方說明
- 建立Pages網站：https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- 設定發布來源：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- 上傳檔案：https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
