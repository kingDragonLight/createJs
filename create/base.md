* addChild()
    > 你想把东西放到画布上，你必须使用stage.addChild()。用于添加子视图
* stage.update()
    > 为了能够看到更改，您必须stage.update()在每次更改画布后调用。
* drawRect(a,b,w,h)
    > 画正方形  a,b为左上角位置，w h为宽高
* Bitmap()
    > 用于显示图片，必须在图片加载完后进行操作 如 image.onload=event=>{}
* stage.update()
    > 为了能够看到更改，您必须stage.update()在每次更改画布后调用。
* createjs.Ticker.setFPS(numb)
    > 设置tick函数的帧数
* container
    > 容器。很多时候我们不方便直接操作satge，此时可以添加容器用于操作
* stage.update()
    > 为了能够看到更改，您必须stage.update()在每次更改画布后调用。新建后直接stage.appChild。然后就可以container.appChild()
* Text(x,y,z)
    > x:内容。y:"大小 字体",z:颜色 比如 var text = new createjs.Text("Hello World", "20px Arial", "#ff7700");
    通过getBounds()获取文本宽高，根据画布宽高来定义位置实现居中等
* shape()
    > 绘制矢量图形时必要的形状。
       