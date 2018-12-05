# Git
---
## config
```
git config --global user.name "<name>"
git config --global user.email "<email>"
```
直接配好密码方便提交代码：
`git config -e  # 打开配置，修改其中的url`
`url=http:<username>:<pwd>@<...>`

## clone
```
git clone <pro_url>.git  # 克隆master分支
git clone -b <branch\_name> <pro_url>.git  # 克隆指定分支
```
## remote
`git remote add origin <pro_url>.git`



