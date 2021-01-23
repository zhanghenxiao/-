响应布局：一个端的页面能响应多端的页面展示

原理：媒体查询.父级布局容器

bootstraphttps://bootstrap.css88.com/css/#helper-classes

有个很多定制的类如container,container-fluid等布局容器

栅格系统是通过行row和列cloumn来组成页面的  自动分为12列， 类前缀大屏 col-lg-3

中屏col-md-4  小屏col-sm-6 超小屏col-xs-12

```
<!-- 完整的写法  需要布局容器 + row + col-lg  -->
  <div class="container">
    <div class="row">
      <div class="col-lg-3">1</div>
      <div class="col-lg-3">2</div>
      <div class="col-lg-3">3</div>
      <div class="col-lg-3">4</div>
    </div>
  </div>
```



技术选型

方案：我们采取响应式页面开发方案

技术： bootstrap 框架

设计图：采用1280px设计尺寸

需求分析策略： 先整体分为几档布局，先布局md（pc端） 以上的 ，在布局其他的

响应式布局也不关心高度，因为页面变小高度也会随之改变 ，我们无法写固定的

##### 这点很关键!!,决定是否能成功做响应布局

先确定改页面乃至这个单独的盒子（如list 盒子）！！！ 在  四档（大屏 中屏 小屏 超小屏中是如何显示的这个很关键） 观察我们的页面在哪档会变化  list盒子在col-xs小屏下才会有变化 我们代码就写

row  然后再写列 col-sm才行

页面盒子在不同屏幕区别这个很重要 



总结混合技术开发： flex 为主 rem为辅 ，或者rem为主 flex 为辅





















