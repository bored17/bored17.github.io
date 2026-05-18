---
title: "c++ build工具"
date: 2022-03-12 00:00:00
updated: 2022-03-13 13:18:56
---

# c++ build工具

Edited on
2022-03-13

## important

简单使用
方便的使用别人的代码，分享代码
隔离
构建同时生产文档

## processer + complier + linker  + pkg-config + system

几把

## makefile

几把

## cmake

A step:寻找拥有install(export)config.cmake 的cmake项目在github等网站上。
B step:(external目录)使用external_add下载2类型的项目到指定位置 A step的项目到不侵入系统库的位置,(root目录)使用exteranl_add 指定src项目 pcakge_DIR位置() 使用findpackage CONFIG找到依赖

## xmake

听说很好用

[hexo搭建静态网站](/2022/03/02/hexo%E6%90%AD%E5%BB%BA%E9%9D%99%E6%80%81%E7%BD%91%E7%AB%99/)