# 现代机器人: 力学，规划和控制
# 代码库
本仓库中包括了剑桥大学出版社于2017出版的[_Modern Robotics:
Mechanics, Planning, and Control_](http://modernrobotics.org) 书中的代码，[用户手册](/doc/MRlib.pdf)在这里

中文译版是机械工业出版社的现代机器人学（封面是一个机械臂，区别于机器人学导论）

本文代码通过三种语言进行描述:
* Python
* MATLAB
* Mathematica

每个函数都包括了输入，输出以及如何使用的解释（input,process,output）
同时本仓库也用MATLAB格式提供了函数概览

函数根据书中的顺序进行布局

书中不包括一些基础函数，如计算向量大小，向量正交化，0值测试和其他的矩阵操作，如矩阵乘法和矩阵求逆

提供这个仓库是为了能够更好的阅读和学习，能够加强对书中概念的理解
并没有对函数的效率和鲁棒性进行优化

感谢其他小伙伴的帮助，下边有一些非官方的其他语言版本的仓库：
* [C++ 版本](https://github.com/Le0nX/ModernRoboticsCpp)
* [Julia 版本](https://github.com/ferrolho/ModernRoboticsBook.jl)
* [Nim 版本](https://github.com/Nimbotics/ModernRoboticsNim)


以下为在我们的基础上开发的函数库：

* [tf_rbdl](https://github.com/junhyeokahn/tf_rbdl#tf_rbdl), 在`Python`基础上进行修改的包 `tensorflow`.

我们欢迎各位对我们的仓库进行贡献，但是我们不保证这些库的可靠性