# rotatingCube
### 旋转的立方体
# 知识点
## transform:
### rotate(-deg) 旋转的角度
### translate(-px) 移动的位移
## perspective:
## 指定观察者与「z=0」平面的距离，使具有三维位置变换的元素产生透视效果。
### 加在父元素上和加在子元素上是不一样的
### 加在父元素上：perspective:length;
### (谁做3D变换，就把这个的父元素加perspective)
### 加在子元素上：transform:perspective(length);
## perspective-origin:指定透视点的位置。
### 两个参数第一个用于横坐标，第二个用于纵坐标
### perspective-origin:100px 100px;//长度
### perspective-origin:50% 50%;//百分比