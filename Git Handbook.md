# Git_Handbook

> ### 1.创建一个 Git 管理的本地仓库

#### 1.创建版本库

```python
$ mkdir learngit
$ cd learngit
$ pwd  
# pwd命令用于显示当前目录 /Users/michael/learngit
```

#### 2.使用`git init`命令使其变成 Git 可以管理的仓库

```python
$ git init
# Initialized empty Git repository in /Users/michael/learngit/.git/
```

#### 3.添加新文件到仓库

```python
$ git add readme.txt
$ git commit -m "wrote a readme file"
# [master (root-commit) eaadf4e] wrote a readme file
# 1 file changed, 2 insertions(+)
# create mode 100644 readme.txt
```

#### 4.使用`git status`命令查看当前仓库的状态

```python
$ git status
# On branch master
# Changes not staged for commit:
#  (use "git add <file>..." to update what will be committed)
#  (use "git checkout -- <file>..." to discard changes in working directory)

#	modified:   readme.txt

# no changes added to commit (use "git add" and/or "git commit -a")
```

#### 5.使用`git diff`命令查看修改内容

```python
$ git diff readme.txt 
# diff --git a/readme.txt b/readme.txt
# index 46d49bf..9247db6 100644
# --- a/readme.txt
# +++ b/readme.txt
# @@ -1,2 +1,2 @@
# -Git is a version control system.
# +Git is a distributed version control system.
# Git is free software.
```

#### 6.使用`git rm`删除文件

```python
$ git rm test.txt
# rm 'test.txt'

$ git commit -m "remove test.txt"
# [master d46f35e] remove test.txt
#  1 file changed, 1 deletion(-)
#  delete mode 100644 test.txt
```

> ### 2.远程仓库

#### 1.创建SSH Key

#### 2.在GitHub添加SSH Key

> ### 3.本地仓库推送到远程仓库 (先有本地库，后有远程库)

#### 1.先在GitHub创建一个新仓库

#### 2.在本地对应仓库下运行命令，关联对应远程库

```python
$ git remote add origin git@github.com:michaelliao/learngit.git
```

#### 3.把本地仓库所有内容推送到远程库上

```python
$ git push -u origin master
# Counting objects: 20, done.
# Delta compression using up to 4 threads.
# Compressing objects: 100% (15/15), done.
# Writing objects: 100% (20/20), 1.64 KiB | 560.00 KiB/s, done.
# Total 20 (delta 5), reused 0 (delta 0)
# remote: Resolving deltas: 100% (5/5), done.
# To github.com:michaelliao/learngit.git
#  * [new branch]      master -> master
# Branch 'master' set up to track remote branch 'master' from 'origin'.
```

#### 4.后面，只要本地做了提交，可以通过以下命令把本地最新修改推送到远程库

```python
$ git push origin master
```

> ### 3.远程仓库拉到本地仓库 (先创建远程库，克隆到本地库)

#### 1.在GitHub创建一个gitskills新仓库,使用命令`git clone`克隆到本地

```python
$ git clone git@github.com:michaelliao/gitskills.git
# Cloning into 'gitskills'...
# remote: Counting objects: 3, done.
# remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 3
# Receiving objects: 100% (3/3), done.
```

> ### 4.本地仓库进行修改或删除文件操作后，如何更新到远程仓库

```python
$ git add -u
$ git commit -m "delete test"
$ git push
```

#### `git add -u`只会处理已修改或已删除的文件，不会处理新建的文件。

#### 进入某一目录：cd git

#### 返回上一级目录：cd ..

> ### 5.添加子文件夹 temp

```python
$ git add temp/
$ git commit -m "add temp folder"
$ git push
```

#### 这样操作，temp子文件夹及其里面的文件都会被推送到远程仓库。

#### Github图床显示图片链接地址示例：

https://raw.githubusercontent.com/Tao-Zhou/MarkdownPhoto/master/AI_ML_DL.png

https://raw.github.com/Tao-Zhou/MarkdownPhoto/master/AI_ML_DL.png

https://github.com/Tao-Zhou/MarkdownPhoto/raw/master/AI_ML_DL.png

#### 以上三种链接均可显示图片，但必须是公开仓库，私有仓库无法显示。



