# travel-site

這個倉庫放多個旅遊行程網站，每個行程一個資料夾，裡面一個 `index.html`。

**要新增或修改任何行程之前，先完整讀 `TRIP-GUIDE.md`**，裡面有製作流程、頁面樣板（以 `dolomites/index.html` 為範本）、必須保留的雲端同步程式、發佈規則與測試清單。

三個最重要的規則：

1. 只改自己這次的行程資料夾，不動其他行程。
2. 必須保留 `noindex` meta、`const SYNC`、`SYNC.push(...)`、檔尾的 `applyRemote` 與 `SYNC.sync` 與 `visibilitychange` 區塊。
3. 發佈時只 `git add` 自己的檔案，不要用 `git add -A`；`git pull --rebase` 要加 `--autostash`。
