### 拉取pull
```shell
# 克隆仓库 
git clone https://gitee.com/username/repo.git 

# 进入仓库目录 
cd repo 

# 列出远程分支 
git branch -r 

# 拉取特定分支 
git checkout mybranch

#拉取远程更新
git pull


```
或者

```shell
# 拉取指定远程分支的更新 
git pull origin mybranch

```

### 推送
```shell
#加入所有追踪文件
git add .

#提交更改
git commit -m "主页面布局"

#将本地分支推送到远程仓库的指定分支。
git push origin mybranch
```
