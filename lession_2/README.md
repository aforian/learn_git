# 第二課 - commit 記錄日誌

## Commit 日誌有什麼用

* Commit 的作者是誰
* 提交 Commit 的時間
* 該次 Commit 修改的大概內容

## Commit 的亂碼

一種名為 **SHA-1** 的雜湊演算法，可以產生幾乎不會重複的序號

## Commit 日誌過濾方式

* 作者 `--author`
* 時間 `--since --until`, `--after`
* 內容

## 指令

* `git log` ： 檢視 Git 記錄日誌
  * `git log --oneline` ： 只列出 Git 簡略序號與 Commit 訊息
  * `git log --graph` ： 較圖像化的方式列出 Git 日誌
  * `git log --author="<author>"` : 作者為 `author` 的 Commit
  * `git log --author="<author1\|author2>"` : 作者為 `author1` , `author2` 的 Commit
  * `git log --grep="<keyword>"` : Commit 訊息包含為 `keyword` 的 Commit (分大小寫)
  * `git log --since="<start_at>" --until="<end_at>"` ： 過濾訊息為 start_at 到 end_at 的 Commit
