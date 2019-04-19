## 基本流程
* sprite那个暂时没搞懂。
* 点击和鼠标滑动时触发`addS()`函数。鼠标点击时生成数量较多，移动时较少
* `addS()`作用：
    * `stagemousedown()`和`stagemousemove()`的时候触发。
    * 随机生成一定数量的图。根据鼠标位置确定当前图出现的位置。
    * 在`createjs.Ticker.addEventListener("tick",function(){})`里面进行动画实现。进行位置（从上到下）以及大小变化和透明度变化。在透明度低于0后直接`removeChild()`删除子组件。
