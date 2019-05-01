#非必要的指定
---
## 指定python到python3(非必要)
```
alternatives --install /usr/bin/python python /usr/local/bin/python3.6 1
alternatives --install /usr/bin/python python /usr/bin/python2.7 2
alternatives --config python
python -V
```
## 修改脚本声明（非必要）
```
vi /usr/bin/yum
vi /usr/libexec/urlgrabber-ext-down
```
