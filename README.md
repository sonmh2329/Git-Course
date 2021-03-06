# Git-Course

## 1. Các trạng thái:

Tên TT | Mô tả | Ảnh
-------|-------|----
Unstaging Area/ working directory| code chưa được `git add`|![ảnh](./1.png)
Staging area| code sau khi được `git add`, sẵn sàng để `git commit`|![ảnh](./2.png)

Sau khi git commit thì working tree sẽ trống, sẵn sàng để thực hiện push từ local lên repository.

![ảnh](./3.png)

## 2. Bỏ thay đổi sau khi thực hiện 'git add .'

- git restore --staged <tên file>

hoặc

- git reset : reset hết
- git reset <tên file>: reset file mình muốn

## 3. Hủy bỏ thay đổi trong file ( trước khi thực hiện 'git add .'):

- git checkout -- <tên file>

hoặc

- git restore <tên file>

## 4. Hủy/ reset/ trở về commit mình muốn:

Lệnh | chức năng | ảnh
-----|-----------|----
`git reset --soft <mã commit>`| đưa code về trạng thái staging area của commit chỉ định (sau khi thực hiện `git add`)|
`git reset --hard <mã commit>`| đưa code về trạng thái nguyên thủy, chưa có gì hết (working tree trống)|
`git rest --mixed <mã commit>`| đưa code về trạng thái trước khi thực hiện `git add` của commit.|