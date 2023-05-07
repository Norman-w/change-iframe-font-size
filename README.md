# 自动设置Iframe的字体大小(rem)
##### 开发自适应页面时,使用rem搭配响应式控制类或media等是其中一种解决方案
### 本历程解决在iframe中使用rem时,字体大小不随iframe大小变化而变化的问题
##### iframe本身没有背景色,当变成黄色时,说明iframe的onload事件已经触发,并且iframe的html元素已经加载完毕

## 注意点
### 1. iframe中的html文件通常应与引用处在同一域名下,否则iframe应允许跨域访问
### 2. 当iframe使用百分比动态停靠到父元素时,自身设置的style中的width=100%这样的并不会触发resize事件,需要使用js动态设置iframe的宽高
### 3. 类似夏威夷,bridgeLegal等项目中的setRem方法通常供应当绑定到iframe的onresize上,用iframe的size变化来触发时间而不是直接在父容器中直接设置iframe的html元素的font-size





2023年05月07日