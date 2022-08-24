# Git

## Repository

1. 本地仓库关联远程仓库

```sh
git remote add origin <repository_url>
```

2. 本地仓库重新关联远程仓库

```sh
git remote set-url origin <repository_url>
```

3. 取消本地仓库与远程仓库的关联

```sh
git remote remove origin
```

4. 查看本地仓库关联的远程仓库

```sh
git remote -v
```

## Branch

1. 本地强制推送到远程

```sh
git push -f origin <branch_name>
```

2. 本地分支重命名

```sh

//重命名指定分支
git branch -m <old_name> <new_name>

// 重命名当前分支
git branch -m <new_name>
```

## Tag

1. 删除本地 tag

```sh
git tag -d <tag_name>
```

2. 推送本地 tag 到远程

```sh
git push origin <local_tag_name>
```

## Account

1. 查看账户

```sh
git config user.email
git config user.name
```

2. 设置账户

```sh
git config user.email "<your_email>"
git config user.name "<your_name>"
```