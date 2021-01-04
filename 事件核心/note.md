# 事件类型

- click：用户单击主鼠标按钮（一般是左键）或者按下在聚焦时按下回车键时触发
- dblclick：用户双击主鼠标按键触发（频率取决于系统配置）
- mousedown：用户按下鼠标任意按键时触发
- mouseup：用户抬起鼠标任意按键时触发
- mousemove：鼠标在元素上移动时触发
- mouseover：鼠标进入元素时触发
- mouseout：鼠标离开元素时触发
- mouseenter：鼠标进入元素时触发，该事件不会冒泡
- mouseleave：鼠标离开元素时触发，该事件不会冒泡

区别：

- over和out，不考虑子元素，从父元素移动到子元素，对于父元素而言，仍然算作离开
- enter和leave，考虑子元素，子元素仍然是父元素的一部分
- mouseenter和mouseleave不会冒泡

## 鼠标位置关系

可以理解成鼠标的相对坐标

- page：pageX、pageY，当前鼠标距离页面的横纵坐标
- client: clientX、clientY，鼠标相对于视口的坐标
- offset：offsetX、offsetY，鼠标相对于事件源的内边距的坐标，后面事件源就是指事件目标对象，this是指绑定对象的真实对象。相对目标事件padding的距离。
- screen: screenX、screenY，鼠标相对于屏幕
- x、y，等同于clientX、clientY
- movement：movementX、movementY，只在鼠标移动事件中有效，相对于上一次鼠标位置，偏移的距离

### 元素位置关系

- offsetParent

获取第一个定位的祖先元素，如果没有就是body

相对于该元素的offsetParent的坐标

- getBoundingClientRect方法

该方法得到一个对象，该对象记录了该元素相对于视口的距离