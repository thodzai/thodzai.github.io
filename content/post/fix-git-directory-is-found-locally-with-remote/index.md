---
title: Cách fix không thể thêm git submodule do thư mục đã tồn tại hoặc trùng tên
description:
date: 2022-09-20
slug: fix-git-directory-is-found-locally-with-remote
image:
categories:
  - Git
tags:
  - Submodule
---

**A git directory for 'submodule_name' is found locally with remote(s)**

Lỗi này xuất hiện vì thư mục trùng tên đã khai báo với git local trước đó.

```
fatal: A git directory for 'submodule_name' is found locally with remote(s):
use the '--force' option. If the local git directory is not the correct repo
or you are unsure what this means choose another name with the '--name' option.
```

## Cách xử lý

### English

* remove the submodule folder
* remove declaration in .gitmodules
* clone the git submodule
* re-add the git submodule

### Vietnamese

* xóa thư mục submodule
* xóa khai báo trong .gitmodules
* clone lại git submodule
* chạy lại lệnh add git submodule
