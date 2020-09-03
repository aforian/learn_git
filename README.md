# 為自己學 Git

以往自己學習的 Git 基礎不夠紮實，常常要左翻右找資料，透過這個機會重新認識 Git。
本文使用 [為自己學 Git](https://gitbook.tw/) 的線上版本進行練習，課程為自己每次看的內容作分野，並記錄自己使用過什麼指令。

## 指令

* `git add` ： 把檔案從工作目錄移至暫存區
  * `-a` ： 加入 repo 中全部更動檔案
  * `.` : 加入該目錄下所有更動檔案
* `git commit` ： 把暫存區的內容移至儲存庫
  * `git commit -a` ： 直接把檔案從工作目錄移至儲存庫
  * `git commit -m <message>` ： 直接輸入 commit 的訊息
* `git log` ： 檢視 Git 記錄日誌
  * `git log --oneline` ： 只列出 Git 簡略序號與 Commit 訊息
  * `git log --graph` ： 較圖像化的方式列出 Git 日誌
  * `git log --author="<author>"` : 作者為 `author` 的 Commit
  * `git log --author="<author1\|author2>"` : 作者為 `author1` , `author2` 的 Commit
  * `git log --grep="<keyword>"` : Commit 訊息包含為 `keyword` 的 Commit (分大小寫)
  * `git log --since="<start_at>" --until="<end_at>"` ： 過濾訊息為 start_at 到 end_at 的 Commit
