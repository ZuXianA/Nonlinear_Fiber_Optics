# 2022秋学期戴一堂老师非线性光纤光学
如果代码存在问题，或者有不懂的地方，欢迎提问，企鹅8927714

## Assignment 1：利用Sellmeier公式拟合折射率

使用爬虫获取网页上的 101 组波长和折射率数据  
使用 scipy.optimize.curve_fit 进行非线性拟合  
使用 matplotlib 库画出原始 Sellmeier 公式对应的曲线，以及经由101组数据拟合后的曲线  
  
 latex 文件夹下包含 TEX 文档代码以及生成的 PDF 文件  
 python 文件夹下包含程序源代码以及 HTML 网页  
   
 PS. 运行 python 程序需要 requests、numpy、scipy 和 matplotlib 第三方库
 
 ## Assignment 2：仿真啁啾脉冲在色散光纤内的传输
 本次作业提供 Matlab 和 Python 实现，两个版本的 demo
 
 均可实现三维曲线绘制展示，即光纤长度取不同值时对应的传输特性
 
 没有什么可说的，具体可以看程序注释，不懂的地方欢迎提问
 
 ## Assignment 3：高阶孤子的振荡  
光纤参数自取，入射光脉冲满足色散长度为非线性长度的4倍  
通过不同传输长度下得到的结果，解释高阶孤子周期性演化的原因  

本次作业提供 Matlab 版本的代码，分别采用 SSFT 和 RK4 两种算法进行求解

在具备一定专业知识的基础上，看懂这个程序是很容易的，记得配合注释进行理解消化

## nonlinear_optics_1：张晓光老师的非线性光学 1024 作业
利用塞尔迈耶公式和牛顿公式画出纯石英玻璃对应 1~2um 的折射率曲线  
利用塞尔迈耶公式，画出左图那样的折射率-波长、色散参量D-波长、时延差Δτ - 波长（假定激光器波长谱宽Δλ=0.1nm）的曲线

提供 Matlab 和 Python 实现，两个版本的 demo

非常简单的画图题，具体实现过程直接看程序吧

## nonlinear_optics_2：张晓光老师的非线性光学 1121 作业
问题在书本83页，4.4题要求画角度调谐曲线图  
KDP晶体色散公式在书本56页(3.2.2)，负单轴晶体第Ⅰ类相位匹配的匹配角公式在书本57页(3.2.5)  

提供 Matlab 和 Python 实现，两个版本的 demo

红色虚线表示的是0~8°区间，调谐范围就是两个交点处的横坐标
