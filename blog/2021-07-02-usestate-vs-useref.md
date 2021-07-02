---
slug: usestate-vs-useref
title: useState与useRef的区别
author: Lucasllin
author_title: 前端
author_url: https://github.com/lucasllin
author_image_url: https://avatars.githubusercontent.com/u/10697191?s=400&v=4
tags: [useState, useRef]
---

## 主要区别

- 两者都会保存之前的数据，但是只有`useState`调用 updater 时，让组件渲染
- `useRef`返回一个包含`current`属性的对象，`useState`返回一个数据，第一个是`state`，第二个是`state updater`
- `useRef`的`current`属性是可变的，而`useState`的状态不是，所以`useState`的值不能直接赋值，应该用 state updater 进行赋值
- `useRef`可以用于获取 DOM 元素
