### 关于和显卡有关的问题与命令

> 参考链接[连接远程服务器使用 GPU-指南 - 知乎 (zhihu.com](https://zhuanlan.zhihu.com/p/95792578)

#### 1.基本命令

1.  查看显卡的基本信息

    \*\*nvidia-smi \*\*

2.  查看所有可用的 NVIDIA 设备信息

&#x20; \*\*nvidia-smi -L \*\*

1.  **CUDA_VISIBLE_DEVICES\=1 python test.py**  在终端执行程序时指定 GPU

2.  **python 代码中指定 GPU**

    import os\
    os.environ\["CUDA_VISIBLE_DEVICES"]\="0"

3.  查看自己的 cuda 的信息

    nvcc -V

4.

#### 2.相关问题

一般来说云服务器上默认的 gpu 的 device 编号为 0

#### 3.基本安装地址

cudnn 安装地址[cuDNN Download | NVIDIA Developer](https://developer.nvidia.com/rdp/cudnn-download)
