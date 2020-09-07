# 第三課 - 在 Git 中刪除檔案或更名檔案

## 在 Git 中刪除檔案

### 使用 command-line 指令刪除檔案（或在 finder 刪除）

這種方式透過系統的檔案管理進行，Git會追蹤到檔案被刪除的資訊。

* `$ rm <file_name>` ： 刪除名為 file_name 的檔案
* `$ git add <file_name>` ： 將刪除 file_name 檔案的修改加至 Git 暫存區
* `$ git commit` ： 修改寫入儲存庫

### 直接加入刪除檔案的修改到暫存區

這種方式是使用 Git 的指令執行，省去一個步驟。

* `$ git rm <file_name>` ： 刪除 file_name 檔案，並同時將修改加至 Git 暫存區
* `$ git commit` ： 修改寫入儲存庫

### 將檔案從 Git 控管中移除

這種方式是只把檔案從 Git 的版本控管中移除，在檔案總管中仍會保留該檔案

* `$ git rm <file_name> --cached` ： 將 file_name 檔案從 Git 的版本控管中移除

## 在 Git 中變更檔名

在 Git 中變更檔名，在加至暫存區前，皆會被認為是兩個行為，分別是刪除原有名稱的檔案，以及新增了新名稱的檔案，但加入暫存區後，Git 會根據檔案內容辨別出是修改檔名的行為。

### 使用 command-line 指令更名檔案（或在 finder 更名）

* `$ mv <old_name> <new_name>` ： 將名為 old_name 的檔案更名為 new_name
* `$ git add --all` ： 將更名的修改行為加至 Git 暫存區
* `$ git commit` ： 修改寫入儲存庫

### 在 Git 中進行改名

* `$ git mv <old_name> <new_name>` ：將名為 old_name 的檔案更名為 new_name，並將修改加至暫存區
* `$ git commit` ： 修改寫入儲存庫
