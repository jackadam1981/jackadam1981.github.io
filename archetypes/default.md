---
title: "{{ replace .Name "-" " " | title }}" #标题
description:      #描述、副标题
date: {{ .Date }} #自动生成日期
image:            #图片
math:             #是否开启公式
license:          #许可协议
hidden: false     #隐藏
comments: true    #评论
categories:
    - Test
    - 测试
tags:
    - Test
    - 测试
draft: false      #草稿
---
