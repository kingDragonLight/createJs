## stage
>`const stage=new createjs.Stage("id");`新建舞台。一切都在舞台上开始
>> 貌似stage不能直接添加事件。<br>
   **addChild()**向舞台中添加内容，可直接用stage，也可以用**container**

## container
>`const stage=new createjs.Container()`新建容器。很多时候我们不能直接对舞台进行操作，会影响别的元素。此刻对容器进行操作再方便不过

## bitMap()
>用于显示图片，一般等图片加载完调用，即在**image.onload**函数里调用最好。也可以**tick**函数一直刷新舞台。可以通过**getBounds()**获取宽高，也可也通过**x**,**y**来设置位置

## shape
> ### graphics
>> ### drawRect(x,y,w,h)
>>>绘矩形，**x**,**y**,为位置，**w**,**h**为宽高。**graphics**调用
>> ### beginFill("color")
>>>填充颜色用来，一般和**endFill**一起用
>> ### drawCircle(x,y,r)
>>>graphics方法，用于画圆 **x**,**y**为圆心位置,**r**为半径
>> ### beginPath()
>>>开始新的绘制
>> ### moveTo(x,y)
>>>设置绘制起点
>> ### lineTo(x,y)
>>>与moveTo(x,y)搭配便可以进行直线绘图
>> ### drawRoundRect(x,y,w,h)
>>>绘制椭圆<br>
**x**,**y**为位置,**w**,**h**是宽高
>> ### drawPolyStar(x,y,radius,sides,pointSize,angle)
>>> 绘制星星 **sides**为角数<br>
**pointSize**为角的深度
**angle**第一个点/角的角度,例如,值为0时表示在中心点的右侧开始绘制第一个点
## text
> `const text=new createjs.Text("内容","30px Arial","color");`可以通过**getBounds()**来获取当前文本的宽高，再结合canvas舞台的宽高将文字进行各种定位

## DOMElement
> 可以在canvas里面添加dom元素。貌似没有全部开发完

## Ticker
>   `createjs.Ticker.addEventListener('tick',function(){})`<br>
    可以利用 createjs.Ticker.setFPS()设置帧数。帧数越大速度越快



