**关键要点**

1. 键盘事件
2. 播放声音
3. 改变样式



**延时器清除样式的弊端：**

如果设计师改变了transition过渡效果的持续时间，原先延时器就达不到过渡完毕再删除的效果了

使用transitionend 事件:

在过渡效果执行完毕触发



**为什么不用toggle？**

首先过渡效果结束会触发removeTransition事件，而add class 会有过渡效果结束，remove class 也是，因此会有死循环



**动态DOM和静态DOM**

~~~js
let dynamic=document.getElementsByClassName('key')

let static=document.querySelectorAll('.key')
~~~



通过getElementsByClassName获取的为动态DOM，随元素节点的减少而减少(length值)

querySelectorAll为静态DOM，拿到的值就一直是这个值除非重新获取
