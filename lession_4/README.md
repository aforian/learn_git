# 第四課 - 對最後一次 Git commit 的操作方式

## `--amend` 妙用之處

### 1.修改 Git commit message

用於在最後一次 commit 後修改其 message 的方法

* 最後一次 commit 後
* `$ git commit --amend` ： 執行最後一次 commit message 修改

#### 可以與其他 `git commit` 參數連㩗

一行指令直接修改最後一次 commit 內容：

```
$ git commit --amend -m '<your_message>'
```

### 2. 將修改加入到最後一次 commit

用於不想重新 Commit，並把遺漏的檔案放入最後一個 Commit 的情景

* `$ git add <file_name>` ： 將要加入最後一次 Commit 的修改移至暫存庫
* `$ git commit --amend` ： 將暫存庫中修改併入至最後一次 commit 中

### 使用 `--amend` 時的注意事項

謹記修改 commit 的行為仍然是對 **Git 歷史** 進行修改

**建議只對尚未 push 的內容使用！**

