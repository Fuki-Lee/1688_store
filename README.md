# HTML+CSS+JS——学习小组项目

# 1. 项目内容：
	1688跨境电商平台。1688跨境商城是阿里巴巴的一个分站.主要展示优秀的商品和对跨境商品的搜索以及根据你的浏览相对的推荐商品。

# 2. 个人职责：

    1. 编写小组公共头部的代码，并将其样式以及脚本提取出来形成公共的css和js文件。
    2. 完成商城首页的制作。
    3. 完成小组成员代码的整合，进行公共链接跳转的事件编写。


# 3. 项目过程：

     1. 由于头部导航栏需要被其他人引用。需要考虑代码合并，使用css和js外链的方式将公共样式提取出来，而各个页面有一些细微的调整，则需要小组成员在引用之后，在相应的css中进行修改。因此我在需要修改的两个部分进行代码注释。
     2. 商城主页中页面内容较多，很多地方比较细节化，因此每个模块都需要提前布局，设置好各个模块的宽高以及其相应位置。然后再对每个模块得内容进行相应的实现。
     3. 页面布局的实现其实大同小异。实现过程中有点困难的是导航栏一个小样式和两个轮播图的实现。一开始内容头部的轮播图是打算使用新学的swiper组件来写。毕竟swiper都已经搭好基础轮播图的样式和动画了，不用白不用，但是最后实践的时候发现由于不熟悉组件的使用，并且研究耗时过长就放弃了。毕竟后面的布局内容虽然很基础但是顶不住时间少，内容还挺多的。因此最后采用了最传统的方式完成。基本实现思路就是先完成基础轮播图的移动，然后在轮播图移动完之后设置延迟执行第二三张图片移动动画的效果。而点击事件的实现要点是隐藏上一张轮播图的㲏。通过记录上一张轮播图序号，在移动到当前张轮播图的位置之后就将上一张轮播图的图片隐藏。这样在页面跳转的时候就不会出现，二三张图片移动动画不出来的现象。




#  4. 个人小结：

    1. 小组分工需要明确，项目前期策划的完善程度也需要提高，在后续工作中才能起指导作用，本来底部也算是公共部分。但是页面太长，在讨论的时候忽略了。不过之后在群里有提出来，所以保持良好的沟通对于合作来说很重要。
    2. 小组之间协调合作，分部分配合更能够提高效率。
    3. 在遇到问题的时候不要一个人钻牛角尖，先跳过或者和别人讨论一下。比如，在写布局的时候，犯了一个低级错误，可能是我写布局写傻了。本来以为clear:both；清除浮动影响的效果是无敌的。结果在编写底部两个同级的div中元素浮动的时候，竟然不生效！而明明我已经清除浮动了。结果不管怎么看都没给看出来。然后我就跳过了。完成下面的内容之后才开始来看这个问题。和同学讨论了一下这个问题，结论发现clear:both;是生效，但是顶不住ul中li框的固定宽高影响了下面浮动元素的位置，所以，最后用overflow：hidden；直接清掉第一了ul中li的浮动影响。所以，不管在学习还是生活中，遇到问题不要太钻牛角尖，暂停跳过一下或者和别人多沟通也许会有不一样的解决方案。