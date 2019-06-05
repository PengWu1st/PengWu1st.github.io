---
layout: "post"
title: "如何解决ubuntu错误“not enough disk on boot”"
date: 2019-04-08 17:55:00 -0700
---

# check what kernel you’re currently using with the following command:


```
uname -r
```

# remove old kernel files

```
sudo apt remove --purge linux-image-x.xx.x-xx-generic
```