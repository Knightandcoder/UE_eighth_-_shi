UE4 第8次课渲染基础 作业-shi



链接：https://pan.baidu.com/s/1r5U7eLEcJYDCftXhcA-hMg 
提取码：kksk 

 

场景内有透明方块和半透明物体方块，还有玻璃材质（有折射）的方板   还有 

半透明光罩（在与地面的交界处用上了depthfade和 1-x ->不做衰减而是做增强光，再与本色相加 作为emissive color）        （半透明物体 加点菲涅尔，真实感更好）



蓝图驱动修改材质：   初始放置一个完全透明不可见的方块物体（在3个方块中间那个方块的上方） 按“1”键 材质 变为 不透明（opacity改为1）   再按“1”键可将opacity改为0.1（实现：opacity  通过flipflop在0.1到1两个值之间切换



后期处理： 泛光（bloom） 加了点卷积 （光罩的亮度较强的那部分区域增加了泛光效果），加了点镜头眩光（lens flares）