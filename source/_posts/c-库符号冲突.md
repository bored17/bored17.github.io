---
title: "c++库符号冲突"
date: 2022-03-20 00:00:00
updated: 2022-03-20 11:36:57
---

# c++库符号冲突

## description

c++继承c的sdk,使用别人的库,使用链接器，会有符号冲突。因为sdk不知道什么原因没很好的解决问题，只能靠规范了。

## linker

不同的linker，不同的实现。但是都没有根本解决冲突。根据linker的不同，库函数调用顺序，链接库顺序都会影响link，造成各种情况。

## 规范

当这个世界混乱的时候，只能依靠规范了。
库必须全局隐藏所有符号，只暴露用户使用的符号。

```
1
2
3

```
```
linux gnu sdk 下
complier flag  -fvisibility=hidden -fvisibility-inlines-hidden 
源文件中使用  __attribute__((visibility("default"))) 对需要的符号导出

```

## reference

[https://www.jianshu.com/p/fb5a5550f858](https://www.jianshu.com/p/fb5a5550f858)
CMake Cookbook (Writing an Installer(Generating export headers)))

[grep 命令](/2022/03/14/grep-%E5%91%BD%E4%BB%A4/)