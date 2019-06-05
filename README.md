# 知识点梳理
#### 目录

- [数组](#数组)
- [DevTools面板](#DevTools面板)

## 数组
### 数组乱序

``` html
var arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
arr.sort(function () {
    return Math.random() - 0.5;
});
```

### 操作数组

## DevTools面板

### 快捷键

```` html
Ctrl + Shift + D —— 切换面板位置，从开始位置切换到右边的位置

Ctrl + [ 和 Ctrl + ] —— 向左、向右切换面板选项卡

Ctrl + Shift + M —— 切换手机模拟模式和普通模式

Ctrl + Shift + C —— 选择元素

样式递增/递减
    0.1 —— Alt + 上下箭头
    1 —— 上下箭头
    10 —— Shift + 上下箭头
    100 —— Ctrl + 上下箭头

Ctrl + Shift + P —— 打开Command菜单
    输入screen，可选择节点截图、全屏截图等
    输入theme，可切换黑、白主题
````

Sources > Snippets

    存放js代码，方便复用
    
    运行：Ctrl + p，打开command menu，用 ! + 代码块名，查找预设代码块

### console篇

$0 对当前选中的 html 节点的引用

$1 对上一次选择的节点的引用

s2、s3、s4

$ —— 未被定义过，则对应document.querySelector

$$ —— 执行 document.QuerySelectorAll，返回一个节点的数组

$_ —— 引用上次执行的结果







