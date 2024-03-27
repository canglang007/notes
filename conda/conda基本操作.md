# anaconda 相关命令

- 创建虚拟环境

&#x20; conda create -n your_env_name python\=x.x

- 查看有哪些虚拟环境

&#x20; conda info -e （查看所有的虚拟环境）

- 重命名虚拟环境

先 clone 原有环境：

&#x20; conda create -n conda-new --clone conda-old

再删除原有环境：

&#x20; conda remove -n conda-old --all

- bash 下启动 conda 命令

  source activate
