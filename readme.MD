# Git版本控制管理

参考书籍：《Git版本控制管理》(Jon Loeliger & Mattbew McCullough)

学前掌握程度：熟练

学习目标：巩固，理解，精通,master

略过背景、安装、与svn结合等内容。

## 第3章 起步

### 3.1 Git命令行



重点：命令行格式，基础命令（即git这个命令），子命令，选项（子命令选项）,专用子命令选项，命令参数，长选项，短选项

NOTE：这些东西多用就熟悉并能融会贯通，没必要死记硬背。

* "git --选项"，选项包括：version,help等十来个，记得前面带上"--"，如：git --version；

* "git 子命令"，如: "git pull"；

* "git 子命令 --子命令选项"，如："git commit --amend"，这里--amend是commit子命令的专用子命令选项，当然应该还有非专用的子命令选项比如常用的"git commit --all；

* "git --选项 子命令 --子命令选项"，如："git --git-dir=project.git repack -d",这里-d是个段选项，见后面关于长选项和短选项的区别；

* "git 子命令 子命令参数 --子命令选项"，如："git add index.html --ignore-errors"

注意：

1. 书中将选项和命令选项统称为"选项"，我为了区分将第二个"选项"称为"子命令选项"。当然，不区分"选项"和"子命令选项"并没有问题，
记住"命令可以带上选项，因为git本身也是一个命令，所以可以带上选项，子命令当然也可以带上选项"；

2. 某些选项可以带上值。

3. 区分命令选项和命令参数

#### 长选项和短选项：
举例：git commit -m 'some message'等价于git commit --message='some message'，-m是短选项，--message就是短选项

#### "裸双破折号"分离参数

```text
# checkout the tag named "main.c"
$ git checkout main.c

# checkout the file named "main.c"
$ git checkout -- main.c
```
这个因为对checkout子命令不甚了解，先不深入。

```text


$ git

usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone     Clone a repository into a new directory
   init      Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

```

### 3.2 快速入门

#### 3.2.1 初始化一个空仓库

理解：实际是创建一个.git目录
```text
git init
```

#### 3.2.2 将文件添加到版本库中

##### git add

```text
# 将文件添加到版本库
$ git add 文件名
```

文件未提交(commit)前在版本库中的几种状态：

1. Untracked：未add之前的状态；

2. 暂存(staged):git add之后的文件状态；

3. modified:新文件相对于暂存，或老文件相对于git库处于被修改的状态,修改后不管是否add都是modified状态,但是如果add了，
用status命令查看，文件颜色是绿色的，否则是红色;

4. deleted:被删除

NOTE:git add并不仅仅只是添加新文件,当文件状态是modified的时候，git add可以将改变的文件重新暂存。可以这样理解：staged状态的文件，暂存起来
的内容和正在编辑的内容是一样的，它们随时可以提交。

##### git status

```text
# 
$ git status

On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore
        modified:   readme.MD


```
NOTE:根据命令提示，(use "git restore --staged <file>..." to unstage)，我尝试将一个已暂存的文件a.txt移出版本库：
```text
# 从版本库中移除a.txt，使其变为untracked状态
$ git restore --staged a.txt
``` 

##### git commit

```text
# 查看commit子命令格式
$ git help commit
git commit [-a | --interactive | --patch] [-s] [-v] [-u<mode>] [--amend]
                  [--dry-run] [(-c | -C | --fixup | --squash) <commit>]
                  [-F <file> | -m <msg>] [--reset-author] [--allow-empty]
                  [--allow-empty-message] [--no-verify] [-e] [--author=<author>]
                  [--date=<date>] [--cleanup=<mode>] [--[no-]status]
```

NOTE:commit提交那些被add的文件，add之后如果文件有变化，这些变化不会被提交到版本库。所以除非特殊情况，commit之前确认是否add可能是个好习惯。

如果git add --all（添加所有）后commit,用git status查看：
```text
$ git status
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
```
工作目录干净(working tree clean),意思我理解应该是：我工作的地方(文本编辑器，IDE)等这些地方的文件内容和版本库一样了。

#### 3.2.3 配置提交作者

```text
$ git config user.name "Shame on Joe Biden"
$ git config user.email "trump4moreyears@donald.com"
```

也可以设置环境变量GIT_AUTHOR_NAME和GIT_AUTHOR_EMAIL.

#### 3.2.4 再次提交

NOTE:记得add! 书上说文件已经添加到版本库就没必要add，这与我使用的结果不一样。这是版本差异还是作者错了？

#### 3.2.5 查看提交

```text
$ git log

commit 5fda9bdf727db118dd41cf00267cbec39d8e54e0 (HEAD -> master)
Author: yuxingxie <185246042@qq.com>
Date:   Tue Nov 10 15:00:21 2020 +0800

    must add before commit?

commit 39f1662f767217bea2055927fe153524c0ca2895
Author: yuxingxie <185246042@qq.com>
Date:   Tue Nov 10 14:55:43 2020 +0800

    ds
:

```

5fda9bdf727db118dd41cf00267cbec39d8e54e0这一串东西叫提交ID。看下面的命令：

```text
$ git show d89dc2fedea05fa019a8edc846b0a000f53755e8
commit d89dc2fedea05fa019a8edc846b0a000f53755e8 (HEAD -> master)
Author: yuxingxie <185246042@qq.com>
Date:   Tue Nov 10 15:16:40 2020 +0800

    add exists file a.txt

diff --git a/a.txt b/a.txt
index d518ffc..e6c17c7 100644
--- a/a.txt
+++ b/a.txt
@@ -1 +1 @@
-dsdfsfds的范德萨发生的双方都胜多负少
\ No newline at end of file
+dsdfsfds的范德萨发生的双方都胜多负少dsfsdfdsdsf
\ No newline at end of file

```
git show-branch是查看当前分支的单行摘要,可以带上命令选项--more=n。n是一个整数，表示看更多的提交次数。
```text
 git show-branch --more=10
[master] add exists file a.txt
[master^] must add before commit?
[master~2] ds
[master~3] aaa
[master~4] some files not staged
[master~5] Initial commit

```
关于分支日后研究，现在我们这个分支叫master分支。

#### 3.2.6 查看提交差异

命令格式为：git diff 提交ID1 提交ID2

#### 3.2.7 版本库内文件的删除和重命名

##### 删除

```text
$ git rm a.txt
error: the following file has local modifications:
    a.txt
(use --cached to keep the file, or -f to force removal)
```

注意-f和--cached两个不同的命令选项。

rm之后需要git会暂存"删除"这个变更(不需要add了)，然后可以commit到版本库。

##### 重命名

书中介绍了两种方法，我并不打算使用他的git rm和git add组合方法，仅推荐如下方法：
```text
$ git mv a.txt b.txt
```

#### 3.2.8 创建版本库副本

git clone用于创建版本库副本。

这个命令我们从github或从gitee上克隆用过无数次了。对于一个本地git仓库我们克隆的方法是：
```text
$ git clone 源版本库目录全路径 目的版本库目录全路径
``` 

如：git clone ~/a_project ~/b_project。这个操作和copy文件夹是不一样的。

### 3.3 配置文件

NOTE:这个先不重点学习

有几个地方可以找到配置文件，并有不同的优先级。

* .git/config(版本库特定)

* ~/.gitconfig(用户级别)

* /etc/gitconfig(linux系统级)

* /usr/local/git/etc/gitconfig(我的mac，不知道是不是系统级)



## 第四章 基本的Git概念

### 4.1 基本概念

* 版本库(repository)

* 对象库(object store)

* 索引(index)

* 块(blob)、目录树(tree)、提交(commit)、标签(tag)

#### 4.1.1 版本库

版本库存什么呢？顾名思义，存各个版本。那么何谓版本呢？我暂时理解为：每一次提交就是一个版本。

版本库位于.git目录。

版本库中，git维护两个主要的数据结构：对象库(object store)和索引(index)。

对象库在复制操作的时候能进行有效复制，这也是用来支持完全分布式VCS的一种技术。

#### 4.1.2 Git对象类型

* 块(blob)

文件的每一个版本表示为一个块。blob是"二进制大对象"(binary large object)的缩写。

* 目录树(tree)

一个目录树对象代表一层目录信息。

* 提交(commit)

一个提交对象保存版本库中每一次变化的元数据，包括作者、提交者、提交日期和日志信息。

* 标签(tag)

一个标签对象分配一个任意的且人类可读的名字给一个特定对象，通常是一个提交对象。



