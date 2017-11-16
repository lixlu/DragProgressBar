# DragProgressBar
js
使用原生的js实现进度条拖动功能,同时通过点击也能实现拖动变化
一、实现原理：
①需要创建两个div,其中progress这个div负责实现点击功能,做为遮罩层通过z-index属性放在最上面;
②"first-face"这个div包含两个子元素,分别是进行拖动效果展示的bar,默认宽度为0,拖动过程中通过bar的宽度变化显示拖动效果,还有一个span作为拖动按钮,但是由于遮罩层的影响,所以需要设置它的z-index属性,放在最上面
③使用了flex的align-items: center属性,使子元素都居中显示
④需要注意clientX,offsetX的区别
