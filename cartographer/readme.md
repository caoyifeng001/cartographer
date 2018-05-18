cartographer代码结构

common：定义了基本数据结构以及一些工具的使用接口。

sensor：定义了雷达数据及点云等相关的数据结构。

transform：定义了位姿的数据结构及其相关的转换。

kalman_filter:
主要通过kalman滤波器完成对IMU、里程计及基于雷达数据的估计位姿的融合，进而估计新进的laser
 scan的位姿。

mapping：定义了上层应用的调用接口以及局部submap构建和基于闭环检测的位姿优化等的接口。

mapping_2d和mapping_3d：对mapping接口的不同实现。
