# 事件循环

1. 主线程，这里发生大量事情，是Javascript执行的地方，也是产生渲染的地址，更是生成新dom的地方；
2. 任务队列和渲染执行队列是俩个不同的队列，使用requestAnimationFrame在执行渲染队列的时候会回调这个函数，所以把一些渲染处理的逻辑放到该函数中。
3. 