# JS-value-in-obj
关于数组的值传递，对象的地址传递和console.log的处理时间。

问题：为什么输出的两个数组值都是经过排序后的。
原因：console.log处理时间较长 还没输出 for循环就执行了，for循环就把数组的值改变了（即重新排序了）。而数组的值是对象，对象不是直接值传递，而是地址传递。
