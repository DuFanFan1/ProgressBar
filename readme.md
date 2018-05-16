常见的网页进度条加载

或许有用的网站
1、免费的gif动画下载;
2、另外一个免费的gif动画下载;
3、自动处理CSS 3前缀在线网站,代码粘贴进去，等待一段时间即可。

demo1定时的进度条
这是一个伪加载完成的进度条，页面跳转时间由自己来设置，实用性并不高。


demo2通过加载状态触发的进度条
知识点：
1、document.onreadystatechange 页面加载状态改变时的事件
2、document.readyState 返回当前文档的状态
相关readyState状态码：
1、uninitialized 还未开始载入
2、loading 载入中
3、interactive 已加载，文档与用户可以开始交互
4、complete 载入完成
通过对页面的加载状态来触发相应的事件，这是一种合适的进度条制作。


demo3通过CSS3制作进度条
利用CSS3动画制作的进度条效果，简单好玩，同样也是通过加载状态来触发相应的事件。


demo4固定在头部的进度条
在每一段结构代码后面添加jQuery中的animate方法增加固定在顶部元素的长度，当长度达100%后触发事件，隐藏遮罩层，这也是一种伪加载完毕事件，实用性并不强。


demo5实时监测加载的进度条
知识点：
1、建立图像对象：var 名称 = new Image()
2、属性：border complete height...
3、事件：onload onerror onkeydown onkeypress...
4、src属性一定要写到onload的后面，否则程序在IE中会出错
用户体验比较好的一种加载方式，能够随时随地知道资源加载到了哪一步。
