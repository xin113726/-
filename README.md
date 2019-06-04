# 知识点梳理
#### 目录

- [数组](#数组)

## 数组
### 数组乱序

``` html
var arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
arr.sort(function () {
    return Math.random() - 0.5;
});

### 操作数组
