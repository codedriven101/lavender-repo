# Github workflow 基本練習

這份作業會帶你走過一次完整的 GitHub 協作流程：從取得專案、開分支、提交修改、發 Pull Request，到處理 Code Review 與合併衝突。

> 每一題都請**實際操作**，並把題目要求的指令輸出或截圖記錄在 `answers/<你的 GitHub 帳號>.md` 中。

---

## 第一部分：基本操作

### 題目 1：取得專案

1. 將本專案 **Fork** 到你自己的 GitHub 帳號下。
2. 將你 Fork 出來的專案 **Clone** 到本機。
3. 執行 `git remote -v`，並把輸出貼到答案檔中。

**思考題：** Fork 和 Clone 有什麼不同？各自發生在哪裡（GitHub 上還是本機）？

---

### 題目 2：第一次 Commit

1. 建立 `answers/<你的 GitHub 帳號>.md`，內容寫上你的名字與今天的日期。
2. 使用 `git status` 觀察檔案狀態。
3. 使用 `git add` 與 `git commit` 提交這個檔案，commit message 為：
   ```
   docs: add answer file for <你的帳號>
   ```
4. 執行 `git log --oneline`，把輸出貼到答案檔中。

**思考題：** `git add` 之前和之後，`git status` 顯示的內容有什麼差別？「工作目錄（working directory）」、「暫存區（staging area）」、「儲存庫（repository）」分別是什麼？

---

### 題目 3：Push 到遠端

1. 將 commit push 到你 Fork 的 GitHub repo。
2. 到 GitHub 網頁上確認檔案已經出現。

**思考題：** `git push origin main` 這行指令中，`origin` 和 `main` 分別代表什麼？

---

## 第二部分：分支與 Pull Request

### 題目 4：建立功能分支

1. 從 `main` 建立一個新分支，命名為 `feature/self-intro`。
2. 在答案檔中新增一段文字。
3. 將分支 push 到遠端。


---

### 題目 5：發 Pull Request

1. 在 GitHub 上，從你的 `feature/self-intro` 分支對**原始專案**的 `main` 發一個 Pull Request。
2. PR 標題請清楚描述修改內容，PR 描述中需包含：
   - 這次修改了什麼

---

### 題目 6：回應 Code Review

我會在你的 PR 上留下 review 意見。

1. 根據意見在**同一個分支**上修改並 push。
2. 在 PR 中回覆。

---

## 加分題（選做）

### 加分題 A：Issue 與 PR 連結

1. 在原始專案開一個 Issue，描述一個你想改進 README 的地方（例如錯字或說明不清楚）。
2. 開一個 PR 修正它，並在 PR 描述中寫上 `Closes #<issue 編號>`。
3. 觀察：PR 被合併後，Issue 發生了什麼事？


## 繳交方式

1. 確認 `answers/<你的 GitHub 帳號>.md` 包含所有題目的輸出與思考題回答。
2. 確認題目 5 的 PR 已經發出，並已回應 review 意見。
3. 在 PR 留言 `@` 我，告知作業已完成。

## 參考資源

- [Git 官方文件（中文）](https://git-scm.com/book/zh-tw/v2)
- [GitHub Docs：關於 Pull Request](https://docs.github.com/zh/pull-requests)
- [Learn Git Branching（互動式練習）](https://learngitbranching.js.org/?locale=zh_TW)
