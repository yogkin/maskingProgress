#### 图片遮罩带进度上传的 ImageView
##### 做个萌哒哒的包子君

###### 这个效果来源于 一个朋友项目的需求，而这个需求恰恰是仿的咸鱼发布任务里面的一个图片上传带进度的功能，而我最近刚好在复习 View 的知识，内心就萌发了要实现这个效果。 废话不多说，先看效果图 ：
![效果图](https://github.com/shuangqingfeng/maskingProgress/raw/master/screen/maskingProgress.gif)

###### 此项目分为两部分：
+ 效果中的图片选择框架用的是 [okhttp-OkGo](https://github.com/jeasonlzy) 网络框架的作者 jeasonlzy,再次感谢作者提供轮子，供我们使用， 点击查看[图片选择框架](https://github.com/jeasonlzy/ImagePicker)
+ 自定义 ImageView
  
###### 如何自定义view
+ 自定义 View 分为三步曲
 + 继承 View
 + 重写 onMeasure
 + 重写 onDraw()<br/>
 三步曲 是自定义View的基础步骤，我们细细说说  onMeasure() 和 onDraw() 方法 ，在下面文字中，如果有理解不对的地方的地方还望指教，共同进步。<br/>
    + onMeasure()<br/>
    字面理解为：测量。即对View进行宽高测量,以便在屏幕显示多大空间<br/>
      + View的测量有三种模式：<br/>
       + EXACTLY<br/>
          字面理解：精确。何为精确模式呢？也就是说是有具体的数值来表示的。比如我们在xml 指定 View的宽高分别给定的是 具体的值，那么系统在调用onMeasure() 方法的时候就使用这种模式测量View.<br/>
       + UNSPECIFIED<br/>
          
 

 
 
 
 
 
