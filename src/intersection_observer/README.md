# IntersectionObserver API 介绍

项目[示例](https://zhengjunxin.github.io/web-samples/src/intersection_observer/) ([源文件](https://github.com/zhengjunxin/web-samples/blob/master/src/intersection_observer/index.html))

用途：用于获得指定 dom 元素相对其他元素的位置。可以用于如：广告展示的检测、懒加载的检测
好处：
- 不用监听 scroll 事件（有可能会导致阻塞）
- 位置检测（查询元素的 scrollTop 或 clientHeight 等操作）会导致重排

其中 intersection 表示指定两个元素的交集部分

最佳实践：
指定 `threshold` 为一个极小值，如 0.0001，这样就能防止贴边误判情况

