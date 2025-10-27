### 修改远程仓库地址
```
git remote set-url origin http://192.168.0.23:3000/luo/React18StudyMooc.git
git remote set-url github https://github.com/darkArmy/React18StudyMooc.git
```
拉取
```
git pull origin main
git pull github main
```

### 查看当前远程仓库设置
```
git remote -v
```
输出：
```
github	git@github.com:darkArmy/React18StudyMooc.git (fetch)
github	git@github.com:darkArmy/React18StudyMooc.git (push)
origin	git@192.168.0.23:luo/React18StudyMooc.git (fetch)
origin	git@192.168.0.23:luo/React18StudyMooc.git (push)
```

### 明确要 pull 哪一个
 - 从“当前分支追踪的远程分支”拉取
```
git pull
```

 - 从 GitHub 拉取
```
git pull github main
```
 - 从本地服务器仓库拉取
```
git pull origin main
```

如果主分支不是 main，而是 master，改成对应的名字。


### 如果忘了远程仓库名或分支名，可以这样查：
查看所有远程：
```
git remote
```

查看当前分支追踪哪个远程：
```
git branch -vv
```
输出示例：
```
* main  123abc [origin/main]  更新日志
```
表示当前分支 main 追踪的是 origin/main。

