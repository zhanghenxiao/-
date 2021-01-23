技术选型: rem + fixeible +再加其他布局方案如flex

当然我们也可以用  rem+less+ fixeible.js+再加其他布局方案如flex

vscode有个插件cssrem     px转换成rem, cssrem默认字体大小是16px,

fixeible 是把页面平均分为10等分

我们的设计稿是750px

html字体大小是750 / 10 = 75px

修改默认配置：https://blog.csdn.net/weixin_43604680/article/details/107163736

还有坑需要主要当我们页面大于750px 的时候，我们html大小就按 750/10 = 75

```html
@media screen and (min-width:750px){

 html {

  font-size: 75px!important;

  }

}
```



