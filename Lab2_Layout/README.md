# exp_02_Layout

## 1.线性布局
</br>
(1)虚拟设备横屏，在manifests下AndroidManifest.xml的activity标签中加入如下代码<br>
![](https://github.com/Xiaohui-Song/exp_02_Layout/blob/main/pictures/4.PNG)<br>
(2)要实现目标布局，可采用垂直布局嵌套四个水平布局或者水平布局嵌套四个垂直布局，我采用垂直布局嵌套四个水平布局,一个水平布局包含四个按钮组件<br>
(3)实现按钮均等分，可以使用layout_weight，将一行分成“4”份一个按钮占“1”份。<br>
(4)实现按钮边框及背景色，可在res的drawble下新建xml文件 "solid android:color="指定背景色"stroke android:width= android:color="分别指定边框大小和边框颜色，
在layout中直接用android：background=“@drawable/button”即可达到目标效果<br>
(5)实现边框之间距离可以用layout_margin控制按钮与按钮，按钮与父组件间距离<br>
最后效果如下图所示：<br>
![exp_01](https://github.com/Xiaohui-Song/exp_02_Layout/blob/main/pictures/exp1.PNG)</br>

## 2.约束布局
</br>
(1)约束布局一定要确保水平和垂直方向至少有一个约束。</br>
(2)要达到目标效果，可以新建约束布局的xml后，在design中直接拖动按钮到预览中，在右侧Attributes中添加必要属性后加入约束条件。</br>
(3)先给四周的按钮添加约束，固定好后，再固定其他的按钮，其他按钮以固定好的按钮为基准添加约束。</br>

 最后效果如下图所示：</br>
![exp_02](https://github.com/Xiaohui-Song/exp_02_Layout/blob/main/pictures/exp2.PNG)</br>

## 3.表格布局
 </br>
 (1)gravity,Layout_marginLeft，Layout_marginRight控制位置</br>
 (2)用view可以实现分割线background设置颜色 layout_weight设置分割线宽度</br>
 最后效果如下图所示：</br>
 ![exp-03](https://github.com/Xiaohui-Song/exp_02_Layout/blob/main/pictures/exp3.PNG)</br>
 
## 4.问题及解决
 </br>
 (1)实验中遇到预览显示和虚拟设备显示不相同问题，可在预览中点击view option勾选Show Layout Decorations显示根布局解决该问题</br>
 (2)不小心误删layout下xml文件可右击layout点击Local history->show history进行恢复
