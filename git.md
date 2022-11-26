# Git

## Repository

初始化本地仓库

```bash
git init
```

本地仓库关联远程仓库

```bash
git remote add origin <repository_url>
```

本地仓库重新关联远程仓库

```bash
git remote set-url origin <repository_url>
```

取消本地仓库与远程仓库的关联

```bash
git remote remove origin
```

查看本地仓库关联的远程仓库

```bash
git remote -v
```

## Branch

本地分支强制推送到远程

```bash
git pubash -f origin <branch_name>
```

本地分支重命名

```bash

// 重命名指定分支
git branch -m <old_name> <new_name>

// 重命名当前分支
git branch -m <new_name>
```

删除本地分支

```bash
git branch -D <branch_name>
```

检出新分支并清除原提交记录

```bash
git checkout --orphan <branch_name>
```

### Pull

拉取远程分支

```bash
git pull
git pull --rebase
```

## Tag

删除本地 tag

```bash
git tag -d <tag_name>
```

推送本地 tag 到远程

```bash
git pubash origin <tag_name>
```

## Account

查看账户

```bash
git config user.email
git config user.name
```

设置账户

```bash
git config user.email "<your_email>"
git config user.name "<your_name>"
```

## Commit

查看本次修改的文件

```bash
git status -s
```

将所有文件加入到暂存区

```bash
git add .
```

将所有文件移出暂存区

```bash
git reset
```

输入提交信息

```bash
git commit -m "<commit_message>"
```

撤销最后一次提交

```bash
git reset --soft HEAD~
```

合并多次提交记录为一次

```bash
git reset --soft HEAD~3
```

## Merge

合并其它分支的某次提交

```bash
git cherry-pick <commit_id>
```

## Stash

查看所有缓存

```bash
git stash list
```

清除所有缓存

```bash
git stash clear
```

缓存当前变更

```bash
// 直接缓存
git stash

// 添加信息再缓存
git stash save "<stash_message>"
```

弹出最新缓存

```bash
git stash pop
```

删除缓存

```bash
// 删除最新缓存
git stash

// 删除指定缓存
git stash drop <stash_id>
```
