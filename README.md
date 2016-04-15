# bootstrap3的应用
##登录页面和首页的小demo
===========================
以下是相关内容总结：（用例子说话总是比较好记一点）  
####1、登陆界面主要用到表单
      （1）调bootstrap的话最外层div直接调.container，可以用栅格系统来限制一下宽度
      （2）表单中默认的input的控件设成.form-control，同时如果登陆界面占的空间比较大的话还是添个.input-lg吧，看起来会比较舒服
      （3）bootstrap里面也可以直接把文字颜色设为白色的.f-white，内容至右.pull-right，至左同理
      （4）botton那儿也有几个款式可用，示例中的按钮就是用.btn-lg(大按钮) .btn-block(拉伸至父元素100%的宽度) 

####2、主页涉及了导航，侧边栏，还有表格
       （1）导航栏当然得固定顶部好看点所以.navbar-fixed-top
       （2）想让导航栏中有个类似标题或者主旨之类的大号内容的话可以用一个类为.navbar-header的<div>元素，里边包一个类为.navbar-brand的<a>元素就能实现
       （3）如果要响应式的特性，比如折叠等，必须把内容包裹在.navbar-collapse、.collapse的div里面
       （4）.container-fluid用在外层div表示的width是100％，而.container的width是用媒体查询获得的动态尺寸，注意区别
       （5）bootstrap是通过一系列的行（row）与列（column）的组合创建页面布局，所以就有包裹在.container里面的.row用来在水平方向上创建一组列
       （6）
       （）通常都会加role=“”，或者sr-only=“”（意思是screen reader only）之类的，增加网站的可访问性
