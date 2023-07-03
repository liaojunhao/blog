---
title: JavaScript代码优化技巧
date: 2021-07-03 10:08:03
tags:
categories:
  - JavaScript
---

## 1.if 多条件判断

在 if 多条件判断的情况下建议使用 include 方法。

```javascript
const day = "星期二";
if (day === "星期二" || day === "星期三" || day === "星期四") {
  console.log(day);
}

// 优化
if (["星期二", "星期三", "星期四"].includes(day)) {
  console.log(day);
}
```

