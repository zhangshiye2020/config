# python/Anaconda settings

## pip 设置国内源

1. 直接命令行设置
```bash
pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
```

2. 修改配置文件

**配置文件路径：**
- windows
```code
%HOME%/pip/pip.ini
```
- linux
```code
~/pip/pip.conf
```

添加如下配置

```ini
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
```

## Anaconda 国内源配置

清华anaconda镜像：

```bash
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
conda config --set show_channel_urls yes
```

Conda 附加库：
```bash
# Conda Forge
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/

# msys2
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/

# bioconda
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/bioconda/

#menpo
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/menpo/

# pytorch
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
```

## pytorch 安装

***注意：*** pytorch安装时从官网复制过来的命令记得去掉-c torch，否则由于优先级问题还是会从官网下载