**关键要点**

1. 指针旋转样式
1. 获取实时时间
1. 每秒钟改变一次



**指针旋转样式：**

用`transform-origin`更换中心点。默认中心点是center，即50% 50%。对于length长度单位px或percentage是先x轴再y轴，位置关键字就按顺序来选择中心点。

把中心点变为最右下角来旋转

~~~css
transform-origin:100%
//transform-origin:right bottom
~~~



