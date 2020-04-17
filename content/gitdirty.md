---
description: 'Git diff: subproject is dirty'
keywords: ["Subproject", "dirty"]
draft: false
tags: ["hugo"]
categories: ["Web"]
author: "dan"
slug: 'gitdirty'
title: "Subproject commit -dirty"
subtitle: "针对github中出现-DIRTY的解决方法"
date: 2020-04-16
publishdate: 20-04-15
lastmod: 20-04-17
---
keywords:Subproject

A.github中提示：Subproject commit 88bc8ad05dbf978eaae1ab6359a81acae4bfd034-dirty

B.git diff 提示 subproject dirty

> `https://stackoverflow.com/questions/4873980/git-diff-says-subproject-is-dirty`

尝试下面的方法中的一种

```
(1)git submodule foreach --recursive git checkout .

(2)git submodule update

(3)git diff --ignore-submodules
git status --ignore-submodules

(4)git config --global diff.ignoreSubmodules dirty
```

我使用了前两种方法都是合适的

