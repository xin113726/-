## Chrome 开发者工具

![image](https://github.com/xin113726/Blog/blob/master/imgs/devtools.png?raw=true)

[元素面板 Elements](https://github.com/xin113726/Blog/issues/1)

[控制台面板 Console](https://github.com/xin113726/Blog/issues/2)

[源代码面板 Sources](https://github.com/xin113726/Blog/issues/3)

[网络面板 Network](https://github.com/xin113726/Blog/issues/4)

[性能面板 Performance](https://github.com/xin113726/Blog/issues/5)


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
    输入timestamps，开启、关闭console的时间信息
````

### Sources > Snippets

存放js代码，方便复用
    
运行：Ctrl + p，打开command menu，用 ! + 代码块名，查找预设代码块

### console篇

$0 对当前选中的 html 节点的引用

$1 对上一次选择的节点的引用

s2、s3、s4

$ —— 未被定义过，则对应document.querySelector

$$ —— 执行 document.QuerySelectorAll，返回一个节点的数组

$_ —— 引用上次执行的结果

条件断点 Add conditional breakpoint

````html
// 第一个参数为 假 时，打印后面的值
console.assert(assertion, obj1[, obj2, ..., objN]);

// 添加大括号，可以显示每个值对应的变量
console.log({a, b, c...});

// 将数组 (或者是 类数组 的对象，或者就是一个 对象 )以表格的形式打印出来；第二个参数，传入你想要展示的列的名字
// 和大括号结合使用
console.table(arr, ['', ''...]);
console.table({a, b, c...});

// 打印对象、DOM节点，并能查看相关信息
console.dir(object);

// 开启一个计时器，结束计时并将结果打印出来
console.time()
console.timeEnd()

// 添加css样式
console.log('%c牛逼','font-size: 50px; color: #F00;');
````

### Elements

展开所有节点：右击节点后的 expand recursively 命令；Alt + 左键点击DOM节点左侧的箭头

支持拖动&放置元素
Ctrl + Shift + Z: 撤销所有修改
Ctrl + Z: 撤销上次修改

### Drawer

Esc：打开/关闭

Sensors(传感器) ：模拟特定的位置，支持从预定义的位置中进行选择，添加自己的位置，或者手动键入纬度/经度

Network conditions：模拟特定的网络行为，3G网络甚至是离线









