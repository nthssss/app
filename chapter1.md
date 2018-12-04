# Python
---
# 编译安装Python
## 安装依赖
`yum install expat-devel gdbm-devel zlib-devel MySQL-python python-devel unzip bzip2-devel openssl-devel ncurses-devel sqlite-devel readline-devel tk-devel gcc gcc-c++ make`

## 下载源码
`wget http://mirrors.sohu.com/python/3.6.6/Python-3.6.6.tgz`
## 编译安装
```
tar -xzvf /usr/local/src/Python-3.6.6.tgz -C /usr/local/src/
cd /usr/local/src/Python-3.6.6
./configure --prefix=/usr/local/bin/python3 --enable-optimizations
make altinstall
```
## 指定python到python3
```
alternatives --install /usr/bin/python python /usr/local/bin/python3.6.6
alternatives --install /usr/bin/python python /usr/bin/python2.7 1
alternatives --config python
python -V
```
## 指定pip到pip3


```
cd 
```


