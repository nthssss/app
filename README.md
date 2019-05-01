# README
---
* [Summary](SUMMARY.md)

# 修改CentOS源
修改后部分软件不能更新，待解决

# 修改pypi源
```
mkdir ~/.pip 
tee ~/.pip/pip.conf <<- 'EOF'
[global]
index-url = http://mirrors.aliyun.com/pypi/simple/
[install]
trusted-host = mirrors.aliyun.com
EOF
```

