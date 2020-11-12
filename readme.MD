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

#### 4.1.3 索引

索引是个临时的、动态的二进制文件，它描述整个版本库的目录结构。

思考：索引和目录树的关系。

#### 4.1.4 可寻址内容名称

* 原文

Git对象库被组织及实现成一个内容寻址的存储系统。具体而言，对象库中的每个对象都有一个唯一的名称，
这个名称是向对象的内容应用SHA1得到的SHA1散列值。因为一个对象的完整内容决定了这个散列值，并且认为这个散列值能有效并唯一地对应特定的内容，
所以SHA1散列值用来做对象数据库中对象的名字和索引是完全充分的。文件的任何微小变化都会导致SHA1散列值的改变，使得文件的新版本被单独编入索引。

SHA1的值是一个160位的数，通常表示为一个40位的十六进制数，比如，9da581d910c9c4ac93557ca4859e767f5caf5169。有时候，在显示期间，
SHA1值被简化成一个较小的、唯一的前缀。Git用户所说的SHA1、散列码和对象ID都是指同一个东西。


#### 4.1.5 Git追踪内容

* 原文

理解Git不仅仅是一个VCS是很重要的，Git同时还是一个内容追踪系统（content tracking system）。这种区别尽管很微小，但是指导了Git的很多设计，并且也许这就是处理内部数据操作相对容易的关键原因。然而，因为这也可能是对新手来讲最难把握的概念之一，所以做一些论述是值得的。

Git的内容追踪主要表现为两种关键的方式，这两种方式与大多数其他 ① 修订版本控制系统都不一样。

首先，Git的对象库基于其对象内容的散列计算的值，而不是基于用户原始文件布局的文件名或目录名设置。因此，当Git放置一个文件到对象库中的时候，它基于数据的散列值而不是文件名。事实上，Git并不追踪那些与文件次相关的文件名或者目录名。再次强调，Git追踪的是内容而不是文件。

如果两个文件的内容完全一样，无论是否在相同的目录，Git在对象库里只保存一份blob形式的内容副本。Git仅根据文件内容来计算每一个文件的散列码，如果文件有相同的SHA1值，它们的内容就是相同的，然后将这个blob对象放到对象库里，并以SHA1值作为索引。项目中的这两个文件，不管它们在用户的目录结构中处于什么位置，都使用那个相同的对象指代其内容。

如果这些文件中的一个发生了变化，Git会为它计算一个新的SHA1值，识别出它现在是一个不同的blob对象，然后把这个新的blob加到对象库里。原来的blob在对象库里保持不变，为没有变化的文件所使用。

其次，当文件从一个版本变到下一个版本的时候，Git的内部数据库有效地存储每个文件的每个版本，而不是它们的差异。因为Git使用一个文件的全部内容的散列值作为文件名，所以它必须对每个文件的完整副本进行操作。Git不能将工作或者对象库条目建立在文件内容的一部分或者文件的两个版本之间的差异上。

文件拥有修订版本和从一个版本到另一个版本的步进，用户的典型看法是这种文件简直是个工艺品。Git用不同散列值的blob之间的区别来计算这个历史，而不是直接存储一个文件名和一系列差异。这似乎有些奇怪，但这个特性让Git在执行某些任务的时候非常轻松。


#### 4.1.6　路径名与内容

* 原文

跟很多其他VCS一样，Git需要维护一个明确的文件列表来组成版本库的内容。然而，这个需求并不需要Git的列表基于文件名。实际上，Git把文件名视为一段区别于文件内容的数据。这样，Git就把索引从传统数据库的数据中分离出来了。看看表4-1会很有帮助，它粗略地比较了Git和其他类似的系统。

表4-1　数据库对比
<table width="100%">
    <thead>
        <tr>
        <th>系　　统</th>
        <th>索 引 机 制</th>
        <th>数 据 存 储</th>
        </tr>
    </thead>
        <tr>
        <td>传统数据库</td>
        <td>索引顺序存取方法（ISAM）</td>
        <td>数据记录</td>
        </tr>
        <tr>
        <td>UNIX文件系统</td>
        <td>目录（/path/to/file ）</td>
        <td>数据块</td>
        </tr>
        <tr>
        <td>Git</td>
        <td>.git/objects/hash 、树对象内容</td>
        <td>blob对象、树对象</td>
        </tr>
        
</table>


文件名和目录名来自底层的文件系统，但是Git并不真正关心这些名字。Git仅仅记录每个路径名，并且确保能通过它的内容精确地重建文件和目录，这些是由散列值来索引的。

Git的物理数据布局并不模仿用户的文件目录结构。相反，它有一个完全不同的结构却可以重建用户的原始布局。在考虑其自身的内部操作和存储方面，Git的内部结构是一种更高效的数据结构。

当Git需要创建一个工作目录时，它对文件系统说：“嘿！我这有这样大的一个blob数据，应该放在路径名为path/to/directory/file 的地方。你能理解吗？”文件系统回复说：“啊，是啊，我认出那个字符串是一组子目录名，并且我知道把你的blob数据放在哪里！谢谢！”
