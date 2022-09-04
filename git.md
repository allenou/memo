# Git

## Repository

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

本地强制推送到远程

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

## Tag

删除本地 tag

```bash
git tag -d <tag_name>
```

推送本地 tag 到远程

```bash
git pubash origin <local_tag_name>
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

将所有文件加入到暂存区

```bash
git add .
```

输入提交信息

```bash
git commit -m "<commit_message>"
```