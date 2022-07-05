# Git

## Repository

1. 本地仓库关联远程仓库：
git remote add origin <repository_url>

1. 本地仓库重新关联远程仓库：
git remote set-url origin <repository_url>

1. 查看远程仓库：
git remote -v

## Branch

1. 本地强制推送到远程：
git push -f origin <branch_name>

1. 本地分支重命名：
git branch -m <old_name> <new_name>

## Tag

1. 删除本地 tag：
git tag -d <tag_name>

1. 推送本地 tag 到远程：
git push origin <local_tag_name>

## Account

1. 查看账户

- git config user.email
- git config user.name

1. 设置账户

- git config user.email "<your_email>" 
- git config user.name "<your_name>" 
