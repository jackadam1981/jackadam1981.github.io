---
title: "Vue_01" #标题
description:      #描述、副标题
date: 2024-01-01T00:00:00+08:00 #自动生成日期
image:            #图片
math:             #是否开启公式
license:          #许可协议
hidden: false     #隐藏
comments: true    #评论
# categories:
#     - node.js
#     - VUE
draft: false      #草稿
---
# 简介：

vue是一个中国流行的js框架，看了不少教程都是vue+js，而且版本还老一些，导致我创建的vue+ts根本没办法运行，一直报错，干脆摸索着自己也写一下吧。毕竟vuejs.org，也写的vue+js或许是没更新吧。

# `<script setup>`

老的写法：

如果不启用TS，可以去掉 lang="ts"

```
<script lang="ts">

export default{
  data() {
    return {
      msg: 'Hello Vue!'
    }
  }
}
</script>

<template>
  <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />
  <div>
    {{ msg }}
  </div>
</template>

<style scoped></style>
```

新写法：

script添加了一个 setup

```
<script setup lang="ts">

const msg = "hello world."
</script>

<template>
  <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />
  <div>
    {{ msg }}
  </div>
</template>

<style scoped></style>
```

据说是这样的演变

```
<script lang="ts">

export default {
  setup() {
    const msg = "hello"
    return {
      msg
    }
  }
}

</script>

<template>
  <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />
  <div>
    {{ msg }}
  </div>
</template>

<style scoped></style>
```
