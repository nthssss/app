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

## pull
1. 拉取分支并切换
```
git pull origin :<my_branch>
git checkout <my_branch>
```
- 拉取代码

    `git pull origin`
    
## add>commit>pull>push
```
    git add -all
    git commit -am "<commit_name>"
    git pull origin <develop_branch>
    git push origin <my_branch>
```

## debug
- `git stash 缓存当前未add、commit修改`
- 远程从release分支新建debug分支：`release_v1.0.0>release_v1.0.1`
- 拉取分支并切换
    ```
        git pull origin :release_v1.0.1
        git checkout release_v1.0.1
    ```
- 改bug、`add&commit`
- `push`
    ```
    git push origin release_v1.0.1
    git push origin release_v1.0.1
    ```
- `checkout`
    ```
    git checkout <my_branch>
    git stash pop
    ```