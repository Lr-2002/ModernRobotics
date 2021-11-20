# “现代机器人” Python介绍

## 环境依赖


`numpy` 需要被安装。

## 安装代码包

### 推荐的方法

通过 [pip](https://en.wikipedia.org/wiki/Pip_(package_manager)) 进行安装
```
pip install modern_robotics
``` 

请通过这个安装[pip](https://pip.pypa.io/en/stable/installing/) 
### 其他的安装方法

下载本仓库，并在仓库目录运行 `python setup.py build` 和 `python setup.py install` 两个命令

## 在你的 Python 文件中引入
你需要使用下面的代码来引入代码
```
import modern_robotics as mr
```

对于每个使用到本仓库代码的 Python 都需要这条命令，最好是在开头引入
## 使用仓库代码
在引入本仓库代码之后，你就能够使用包中的代码了

以 `RotInv` 为例，你可以通过下列命令查看函数的描述和实例
```
help(mr.RotInv)
```

如示例所述，你可以通过运行这个命令来使用函数
```
R = np.array([[0, 0, 1],
              [1, 0, 0],
              [0, 1, 0]])
invR = mr.RotInv(R)
```

之后 `invR` 变量的值就是对 R 求逆之后的结果

完整的演示代码如下
```
import modern_robotics as mr
import numpy as np
R = np.array([[0, 0, 1],
              [1, 0, 0],
              [0, 1, 0]])
invR = mr.RotInv(R)
print invR
```

## 在本地使用本包
你可以不用安装就使用
1. 下载`github`的仓库并把它放在需要使用的目录
2. 注意这个包没有被安装，每次你更换目录，这个仓库也需要对应复制过去
3. 每次使用之前仍然需要导入(import)