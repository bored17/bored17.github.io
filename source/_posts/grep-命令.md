---
title: "grep 命令"
date: 2022-03-14 00:00:00
updated: 2022-03-14 14:39:19
---

# grep 命令

## 背景

一个软件，配置文件很多行，版本多，与网上资料行数一般不一致，用肉眼不好找。通过grep字段找到。

## grep 使用
```
shiyanlou:~/ $ sudo grep -n requirepass /etc/redis/redis.conf
212:# If the master is password protected (using the "requirepass" configuration
396:requirepass "test123"

```

轻松找到对应行数-v-

[# linux cli](/tags/linux-cli/)

[c++ build工具](/2022/03/12/c-build%E5%B7%A5%E5%85%B7/)