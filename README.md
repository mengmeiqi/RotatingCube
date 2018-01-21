# rotatingCube
### 旋转的立方体
# 知识点
## transform:
     rotate(-deg) 旋转的角度
     translate(-px) 移动的位移
## perspective:
## 指定观察者与「z=0」平面的距离，使具有三维位置变换的元素产生透视效果。
     加在父元素上和加在子元素上是不一样的
     加在父元素上：perspective:length;
     (谁做3D变换，就把这个的父元素加perspective)
     加在子元素上：transform:perspective(length);
## perspective-origin:指定透视点的位置。
     两个参数第一个用于横坐标，第二个用于纵坐标
     perspective-origin:100px 100px;//长度
     perspective-origin:50% 50%;//百分比
## 3d效果先旋转后位移和先位移后旋转不一样,旋转的过程中轴也跟着动
## transform-style: preserve-3d;使被转换的子元素保留其 3D 转换
## animation动画
    用animation时要定义关键帧：
    	animation: xx  2s  linear  1s  forwards;
    	animation-name:xx;
    	animation-duration: 2s; //time,动画的持续时间
    	animation-timing-function:linear;
    	//过渡 ease|ease-in|ease-out|ease-in-out
    	animation-delay:1s;
    	animation-fill-mode:forwards;//backwards|both|infinite(无限的)
    	//检索或设置对象动画时间之外的状态
    关键帧：@keyframes
    		@-webkit-keyframes xx{
    		    0%{
    		        width:200px;
    		    }
    		    50%{
    		        width:300px;
    		    }
    		    100%{
    		        width:400px;
    		    }
    		} //帧分成了三段
         如果只有两段，可以写成
    		@-webkit-keyframes xx{
    		    from{
    		        width:300px;
    		    }
    		    to{
    		        width:400px;
    		    }
    		}