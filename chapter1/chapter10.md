# 编译安装Python3
## 切换root用户
```
su
```
## 安装依赖
`yum install libffi-devel expat-devel gdbm-devel zlib-devel MySQL-python python-devel unzip bzip2-devel openssl-devel ncurses-devel sqlite-devel readline-devel tk-devel gcc gcc-c++ make`

## 下载源码
`wget http://mirrors.sohu.com/python/3.6.6/Python-3.6.6.tgz`
## 编译安装
```
tar -xzvf /usr/local/src/Python-3.6.6.tgz -C /usr/local/src/
cd /usr/local/src/Python-3.6.6
# 以下两行分开执行
./configure --prefix=/usr/local/bin/python3 
./configure --enable-optimizations
make altinstall
```
