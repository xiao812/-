## 安装Ubuntu 后做的事
### 添加root用户
```
sudo passwd root
```
### 安装vim 
```
    sudo apt install vim
```
### 切换源
#### 备份源
```
    sudo cp /etc/apt/sources.list /etc/apt/sources.list.bak
```
#### 打开源
```
    sudo vim /etc/apt/sources.list
```
#### 切换源
```
    # 默认注释了源码镜像以提高 apt update 速度，如有需要可自行取消注释
    deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic main restricted universe multiverse
    # deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic main restricted universe multiverse
    deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-updates main restricted universe multiverse
     deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-updates main restricted universe multiverse
    deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-backports main restricted universe multiverse
    # deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-backports main restricted universe multiverse
    deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-security main restricted universe multiverse
    # deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-security main restricted universe multiverse
```
#### 更新软件包列表
```
    sudo apt-get update
```
#### 更新软件
可选，全部最新不一定好
```
    sudo apt-get  upgrade
```
### 安装 GCC和GDB
``` 
    sudo apt install build-essential
    gcc --version
```
### 安装 QT
```
    sudo apt install qtcreator 
    sudo apt install sudo apt-get install qt5-default
``` 
### 安装 Pycharm 
官网下载包，解压
```
    cd pycharm-community-2019.3.4/bin
    sh pycharm.sh
```
添加 桌面图标





