# Git笔记

## 工作区与版本库（Working Dir/Repository）

工作区指的就是需要进行管理的文件夹，工作区有一个隐藏目录```.git```，这个目录就是Git的版本库。
![](https://cdn.webxueyuan.com/cdn/files/attachments/001384907702917346729e9afbf4127b6dfbae9207af016000/0)

Git版本库包含两个重要的东西：
- 暂存区（stage/index）
- 分支与指针（master、HEAD）

1. 创建版本库

```
cd ./Working Dir
git init
```

2. 文件或文件夹添加至暂存区

```
git add Files
```

3. 暂存区删除文件或文件夹

- 删除文件
```
git rm file
```
- 删除文件夹
```
git rm -r --cached files
```

4. 暂存区提交至当前分支（默认为master分支）

```
git commit -m [something]
```

5. 查看版本库与工作区状态

```
git status
```

6. 创建远程仓库

```
git remote add [name] [git@github.com:beingWH/git.git]
```

7. 推送至远程仓库

```
## 首次使用-u
git push -u [remote] [local branch]
```
8. 更新远程仓库分支至本地暂存区

```
git fetch [remote] [remote branch]
```
9. 拉取至本地工作区

```
git merge [remote/remote branch]
```
10. 直接拉取远程分支至工作区

```
git pull [remote] [local branch]
```
