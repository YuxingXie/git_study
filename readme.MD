# Git版本控制管理

参考书籍：《Git版本控制管理》(Jon Loeliger & Mattbew McCullough)

学前掌握程度：熟练

学习目标：巩固，理解，精通,master

略过背景、安装、与svn结合等内容。

本内容目录与书中的目录一样，有些地方也会抄一抄书，但我的目的并不是要把这本书抄一遍，主要目的应该是记录自己的学习理解心得。

#### 目录

> <a href='#3'>第3章 起步</a>
>> <a href='#3.1' id='c3.1'>3.1 Git命令行</a>
>>
>> <a href='#3.2' id='c3.2'>3.2 快速入门</a>
>>>
>>> <a href='#3.2.1' id='c3.2.1'>3.2.1 创建初始版本库</a>
>>>
>>> <a href='#3.2.2' id='c3.2.2'>3.2.2 将文件添加到版本库中</a>
>>>
>>> <a href='#3.2.3' id='c3.2.3'>3.2.3 配置提交作者</a>
>>>
>>> <a href='#3.2.4' id='c3.2.4'>3.2.4 再次提交</a>
>>>
>>> <a href='#3.2.5' id='c3.2.5'>3.2.5 查看提交</a>
>>>
>>> <a href='#3.2.6' id='c3.2.6'>3.2.6 查看提交差异</a>
>>>
>>> <a href='#3.2.7' id='c3.2.7'>3.2.7 版本库内文件的删除和重命名</a>
>>>
>>> <a href='#3.2.8' id='c3.2.8'>3.2.8 创建版本库副本</a>
>>
>> <a href='#3.3' id='c'>3.3 配置文件</a>
>
> <a href='#4' id='c4'>第4章 基本的Git概念</a>
>
>> <a href='#4.1' id='c4.1'>4.1 基本概念</a>
>>
>> <a href='#4.2' id='c4.2'>4.2 基本概念</a>
>>
>> <a href='#4.3' id='c4.3'>4.3 Git在工作时的概念</a>
>>> <a href='#4.3.1' id='c4.3.1'>4.3.1 进入.git目录</a>
>>>
>>> <a href='#4.3.2' id='c4.3.2'>4.3.2 对象、散列和blob</a>
>>>
>>> <a href='#4.3.3' id='c4.3.3'>4.3.3 文件和树</a>
>>>
>>> <a href='#4.3.4' id='c4.3.4'>4.3.4 对Git使用SHA1的一点说明</a>
>>>
>>> <a href='#4.3.5' id='c4.3.5'>4.3.5 树层次结构</a>
>>>
>>> <a href='#4.3.6' id='c4.3.6'>4.3.6 提交</a>
>>>
>>> <a href='#4.3.7' id='c4.3.7'>4.3.7 标签</a>
>
> <a href='#5' id='c5'>第5章 文件索引和管理</a>
>>
>> <a href='#5.1' id='c5.1'>5.1 关于索引的一切</a>
>>
>> <a href='#5.2' id='c5.2'>5.2 Git中的文件分类</a>
>>
>> <a href='#5.3' id='c5.3'>5.3 使用git add</a>
>>
>> <a href='#5.4' id='c5.4'>5.4 使用git commit的一些注意事项</a>
>>>
>>> <a href='#5.4.1' id='c5.4.1'>5.4.1 使用git commit --all</a>
>>>
>>> <a href='#5.4.2' id='c5.4.2'>5.4.2 编写提交日志消息</a>
>>
>> <a href='#5.5' id='c5.5'>5.5 使用git rm</a>
>>
>> <a href='#5.6' id='c5.6'>5.6 使用git mv</a>
>>
>> <a href='#5.7' id='c5.7'>5.7 追踪重命名注解</a>
>>
>> <a href='#5.8' id='c5.8'>5.8 .gitignore文件</a>
>>
>> <a href='#5.9' id='c5.9'>5.9 Git中对象模型和文件的详细视图</a>
>
> <a href='#6' id='c6'>第6章 提交</a>
>> <a href='#6.1' id='c6.1'>6.1 原子变更集</a>
>>
>> <a href='#6.2' id='c6.2'>6.2 识别提交</a>
>>>
>>> <a href='#6.2.1' id='c6.2.1'>6.2.1 绝对提交名</a>
>>>
>>> <a href='#6.2.2' id='c6.2.2'>6.2.2 引用和符号引用</a>
>>>
>>> <a href='#6.2.3' id='c6.2.3'>6.2.3 相对提交名</a>
>>
>> <a href='#6.3' id='c6.3'>6.3 提交历史记录</a>
>>>
>>> <a href='#6.3.1' id='c6.3.1'>6.3.1 查看旧提交</a>
>>>
>>> <a href='#6.3.2' id='c6.3.1'>6.3.2 提交图</a>
>>>
>>> <a href='#6.3.3' id='c6.3.3'>6.3.3 提交范围</a>
>>
>> <a href='#6.4' id='c6.4'>6.4 查找提交</a>
>>>
>>> <a href='#6.4.1' id='c6.4.1'>6.4.1 使用git bisect</a>
>>>
>>> <a href='#6.4.2' id='c6.4.2'>6.4.2 使用git blame</a>
>>>
>>> <a href='#6.4.3' id='c6.4.3'>6.4.3 使用Pickaxe</a>
>
> <a href='#7' id='c7'>第7章 分支</a>
>>
>> <a href='#7.1' id='c7.1'>7.1 使用分支的原因</a>
>>
>> <a href='#7.2' id='c7.2'>7.2 分支名</a>
>>
>> <a href='#7.3' id='c7.3'>7.3 使用分支</a>
>>
>> <a href='#7.4' id='c7.4'>7.4 创建分支</a>
>>
>> <a href='#7.5' id='c7.5'>7.5 列出分支名</a>
>>
>> <a href='#7.6' id='c7.6'>7.6 查看分支</a>
>>
>> <a href='#7.7' id='c7.7'>7.7 检出分支</a>
>>>
>>> <a href='#7.7.1' id='c7.7.1'>7.7.1 检出分支的一个简单例子</a>
>>>
>>> <a href='#7.7.2' id='c7.7.2'>7.7.2 有未提交的更改时进行检出</a>
>>>
>>> <a href='#7.7.3' id='c7.7.3'>7.7.3 合并变更到不同分支</a>
>>>
>>> <a href='#7.7.4' id='c7.7.4'>7.7.4 创建并检出分支</a>
>>>
>>> <a href='#7.7.5' id='c7.7.5'>7.7.5 分离HEAD分支</a>
>>
>> <a href='#7.8' id='c7.8'>7.8 删除分支</a>
>
> <a href='#8' id='c8'>第8章 diff</a>
>
> <a href='#9' id='c9'>第9章 合并</a>
>
> <a href='#10' id='c10'>第10章 更改提交</a>
>
> <a href='#11' id='11c'>第11章 储存和引用日志</a>
>
> <a href='#12' id='c12'>第12章 远程版本控制</a>
>
> <a href='#13' id='c13'>第13章 版本库管理</a>
>
> <a href='#14' id='c14'>第14章 补丁</a>
>
> <a href='#15' id='c15'>第15章 钩子</a>
>
> <a href='#16' id='c16'>第16章 合并项目</a>
>
> <a href='#17' id='c17'>第17章 子模块最佳实践</a>
>
> <a href='#18' id='c18'>第18章 结合SVN版本库使用Git</a>
>
> <a href='#19' id='c19'>第19章 高级操作</a>
>
> <a href='#20' id='c20'>第20章 提示、技巧和技术</a>
>
> <a href='#21' id='c21'>第21章 Git和GitHub</a>







## <a id='3' href='#c3'>第3章 起步</a>



### <a id='3.1' href='#c3.1'>3.1 Git命令行</a>


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

### <a id='3.2' href='#c3.2'>3.2 快速入门</a>

#### <a id='3.2.1' href='#c3.2.1'>3.2.1 初始化一个空仓库</a>

理解：实际是创建一个.git目录
```text
git init
```

#### <a id='3.2.2' href='#c3.2.2'>3.2.2 将文件添加到版本库中</a>

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

#### <a id='3.2.3' href='#c3.2.3'>3.2.3 配置提交作者</a>

```text
$ git config user.name "Shame on Joe Biden"
$ git config user.email "trump4moreyears@donald.com"
```

也可以设置环境变量GIT_AUTHOR_NAME和GIT_AUTHOR_EMAIL.

#### <a id='3.2.4' href='#c3.2.4'>3.2.4 再次提交</a>

NOTE:记得add! 书上说文件已经添加到版本库就没必要add，这与我使用的结果不一样。这是版本差异还是作者错了？

#### <a id='3.2.5' href='#c3.2.5'>3.2.5 查看提交</a>

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

#### <a id='3.2.6' href='#c3.2.6'>3.2.6 查看提交差异</a>

命令格式为：git diff 提交ID1 提交ID2

#### <a id='3.2.7' href='#c3.2.7'>3.2.7 版本库内文件的删除和重命名</a>

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

#### <a id='3.2.8' href='#c3.2.8'>3.2.8 创建版本库副本</a>

git clone用于创建版本库副本。

这个命令我们从github或从gitee上克隆用过无数次了。对于一个本地git仓库我们克隆的方法是：
```text
$ git clone 源版本库目录全路径 目的版本库目录全路径
``` 

如：git clone ~/a_project ~/b_project。这个操作和copy文件夹是不一样的。

### <a id='3.3' href='#c3.3'>3.3 配置文件</a>

NOTE:这个先不重点学习

有几个地方可以找到配置文件，并有不同的优先级。

* .git/config(版本库特定)

* ~/.gitconfig(用户级别)

* /etc/gitconfig(linux系统级)

* /usr/local/git/etc/gitconfig(我的mac，不知道是不是系统级)



## <a id='4' href='#c4'>第四章 基本的Git概念</a>

NOTE:本章多为概念和原理，所以先照抄一遍。

### <a id='4.1' href='#c4.1'>4.1 基本概念</a>

* 版本库(repository)

* 对象库(object store)

* 索引(index)

* 块(blob)、目录树(tree)、提交(commit)、标签(tag)

#### <a id='4.1.1' href='#c4.1.1'>4.1.1 版本库</a>

版本库存什么呢？顾名思义，存各个版本。那么何谓版本呢？我暂时理解为：每一次提交就是一个版本。

版本库位于.git目录。

版本库中，git维护两个主要的数据结构：对象库(object store)和索引(index)。

对象库在复制操作的时候能进行有效复制，这也是用来支持完全分布式VCS的一种技术。

#### <a id='4.1.2' href='#c4.1.2'>4.1.2 Git对象类型</a>

* 块(blob)

文件的每一个版本表示为一个块。blob是"二进制大对象"(binary large object)的缩写。

* 目录树(tree)

一个目录树对象代表一层目录信息。

* 提交(commit)

一个提交对象保存版本库中每一次变化的元数据，包括作者、提交者、提交日期和日志信息。

* 标签(tag)

一个标签对象分配一个任意的且人类可读的名字给一个特定对象，通常是一个提交对象。

#### <a id='4.1.3' href='#c4.1.3'>4.1.3 索引</a>

索引是个临时的、动态的二进制文件，它描述整个版本库的目录结构。

思考：索引和目录树的关系。

#### <a id='4.1.4' href='#c4.1.4'>4.1.4 可寻址内容名称</a>

* 原文

Git对象库被组织及实现成一个内容寻址的存储系统。具体而言，对象库中的每个对象都有一个唯一的名称，
这个名称是向对象的内容应用SHA1得到的SHA1散列值。因为一个对象的完整内容决定了这个散列值，并且认为这个散列值能有效并唯一地对应特定的内容，
所以SHA1散列值用来做对象数据库中对象的名字和索引是完全充分的。文件的任何微小变化都会导致SHA1散列值的改变，使得文件的新版本被单独编入索引。

SHA1的值是一个160位的数，通常表示为一个40位的十六进制数，比如，9da581d910c9c4ac93557ca4859e767f5caf5169。有时候，在显示期间，
SHA1值被简化成一个较小的、唯一的前缀。Git用户所说的SHA1、散列码和对象ID都是指同一个东西。


#### <a id='4.1.5' href='#c4.1.5'>4.1.5 Git追踪内容</a>

* 原文

理解Git不仅仅是一个VCS是很重要的，Git同时还是一个内容追踪系统（content tracking system）。这种区别尽管很微小，但是指导了Git的很多设计，并且也许这就是处理内部数据操作相对容易的关键原因。然而，因为这也可能是对新手来讲最难把握的概念之一，所以做一些论述是值得的。

Git的内容追踪主要表现为两种关键的方式，这两种方式与大多数其他 ① 修订版本控制系统都不一样。

首先，Git的对象库基于其对象内容的散列计算的值，而不是基于用户原始文件布局的文件名或目录名设置。因此，当Git放置一个文件到对象库中的时候，它基于数据的散列值而不是文件名。事实上，Git并不追踪那些与文件次相关的文件名或者目录名。再次强调，Git追踪的是内容而不是文件。

如果两个文件的内容完全一样，无论是否在相同的目录，Git在对象库里只保存一份blob形式的内容副本。Git仅根据文件内容来计算每一个文件的散列码，如果文件有相同的SHA1值，它们的内容就是相同的，然后将这个blob对象放到对象库里，并以SHA1值作为索引。项目中的这两个文件，不管它们在用户的目录结构中处于什么位置，都使用那个相同的对象指代其内容。

如果这些文件中的一个发生了变化，Git会为它计算一个新的SHA1值，识别出它现在是一个不同的blob对象，然后把这个新的blob加到对象库里。原来的blob在对象库里保持不变，为没有变化的文件所使用。

其次，当文件从一个版本变到下一个版本的时候，Git的内部数据库有效地存储每个文件的每个版本，而不是它们的差异。因为Git使用一个文件的全部内容的散列值作为文件名，所以它必须对每个文件的完整副本进行操作。Git不能将工作或者对象库条目建立在文件内容的一部分或者文件的两个版本之间的差异上。

文件拥有修订版本和从一个版本到另一个版本的步进，用户的典型看法是这种文件简直是个工艺品。Git用不同散列值的blob之间的区别来计算这个历史，而不是直接存储一个文件名和一系列差异。这似乎有些奇怪，但这个特性让Git在执行某些任务的时候非常轻松。


#### <a id='4.1.6' href='#c4.1.6'>4.1.6　路径名与内容</a>

* 原文

跟很多其他VCS一样，Git需要维护一个明确的文件列表来组成版本库的内容。然而，这个需求并不需要Git的列表基于文件名。实际上，Git把文件名视为一段区别于文件内容的数据。这样，Git就把索引从传统数据库的数据中分离出来了。看看表4-1会很有帮助，它粗略地比较了Git和其他类似的系统。

表4-1　数据库对比
<table style="width:100%">
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

当Git需要创建一个工作目录时，它对文件系统说：“嘿！我这有这样大的一个blob数据，应该放在路径名为path/to/directory/file 的地方。你能理解吗？”文件系统回复说：
“啊，是啊，我认出那个字符串是一组子目录名，并且我知道把你的blob数据放在哪里！谢谢！”

#### <a id='4.1.7' href='#c4.1.7'>4.1.7　打包文件</a>

* 原文

一个聪明的读者也许已经有了关于Git的数据模型及其单独文件存储的挥之不去的问题：直接存储每个文件每个版本的完整内容是否太低效率了？即使它是压缩的，把相同文件的不同版本的全部内容都存储的效率是否太低了？
如果你只添加一行到文件里，Git是不是要存储两个版本的全部内容？

幸运的是，答案是“不是，不完全是！”

相反，Git使用了一种叫做 打包文件（pack file） 的更有效的存储机制。要创建一个打包文件，Git首先定位内容非常相似的全部文件，然后为它们之一存储整个内容。之后计算相似文件之间的差异并且只存储差异。
例如，如果你只是更改或者添加文件中的一行，Git可能会存储新版本的全部内容，然后记录那一行更改作为差异，并存储在包里。

存储一个文件的整个版本并存储用来构造其他版本的相似文件的差异并不是一个新伎俩。这个机制已经被其他VCS（如RCS）用了好几十年了，它们的方法本质上是相同的。

然而，Git文件打包得非常巧妙。因为Git是由内容驱动的，所以它并不真正关心它计算出来的两个文件之间的差异是否属于同一个文件的两个版本。这就是说，Git可以在版本库里的任何地方取出两个文件并计算差异，
只要它认为它们足够相似来产生良好的数据压缩。因此，Git有一套相当复杂的算法来定位和匹配版本库中潜在的全局候选差异。此外，Git可以构造一系列差异文件，从一个文件的一个版本到第二个，第三个，等等。

Git还维护打包文件表示中每个完整文件（包括完整内容的文件和通过差异重建出来的文件）的原始blob的SHA1值。这给定位包内对象的索引机制提供了基础。

打包文件跟对象库中其他对象存储在一起。它们也用于网络中版本库的高效数据传输。


### <a id='4.2' href='#c4.2'>4.2 对象库图示</a>

* 原文

让我们看看Git的对象之间是如何协作来形成完整系统的。

blob对象是数据结构的“底端”；它什么也不引用而且只被树对象引用。在接下来的图里，每个blob由一个矩形表示。

树对象指向若干blob对象，也可能指向其他树对象。许多不同的提交对象可能指向任何给定的树对象。每个树对象由一个三角形表示。

一个圆圈表示一个提交对象。一个提交对象指向一个特定的树对象，并且这个树对象是由提交对象引入版本库的。

每个标签由一个平行四边形表示。每个标签可以指向最多一个提交对象。

分支不是一个基本的Git对象，但是它在命名提交对象的时候起到了至关重要的作用。把每个分支画成一个圆角矩形。

图4-1展示了所有部分如何协作。这张图显示了一个版本库在添加了两个文件的初始提交后的状态。两个文件都在顶级目录中。同时它们的master分支和一个叫V1.0的标签都指向ID为1492的提交对象。


![](https://github.com/YuxingXie/git_study/raw/master/assets/image/04-01.jpg)  

图4-1　Git对象

现在，让我们使事情变得复杂一点。保留原来的两个文件不变，添加一个包含一个文件的新子目录。对象库就如图4-2所示。

![](https://github.com/YuxingXie/git_study/raw/master/assets/image/04-02.jpg)  

图4-2　二次提交后的Git对象


就像前一张图里，新提交对象添加了一个关联的树对象来表示目录和文件结构的总状态。在这里，它是ID为cafed00d的树对象。

因为顶级目录被添加的新子目录改变了，顶级树对象的内容也跟着改变了，所以Git引进了一个新的树对象：cafed00d。

然而，blob对象dead23和feeb1e在从第一次到第二次提交的时候没有发生变化。Git意识到ID没有变化，所以可以被新的cafed00d树对象直接引用和共享。

请注意提交对象之间箭头的方向。父提交在时间上来得更早。因此，在Git的实现里，每个提交对象指回它的一个或多个父提交。很多人对此感到困惑，因为版本库的状态通常画成反方向：数据流从父提交流向子提交。

第6章扩展了这些图来展示版本库的历史是如何建立和被不同命令操作的。

### <a id='4.3' href='#c4.3'>4.3　Git在工作时的概念</a>

#### <a id='4.3.1' href='#c4.3.1'>4.3.1　进入.git目录</a>
* 原文

带着一些原则，来看看所有这些概念和组件是如何在版本库里结合在一起的。让我们创建一个新的版本库，并更详细地检查内部文件和对象库。

```text
$ mkdir /tmp/hello

$ cd /tmp/hello

$ git init
Initialized empty Git repository in /tmp/hello/.git/

# 列出当前目录中的所有文件
$ find .

.
./.git
./.git/hooks
./.git/hooks/commit-msg.sample
./.git/hooks/applypatch-msg.sample
./.git/hooks/pre-applypatch.sample
./.git/hooks/post-commit.sample
./.git/hooks/pre-rebase.sample
./.git/hooks/post-receive.sample
./.git/hooks/prepare-commit-msg.sample
./.git/hooks/post-update.sample
./.git/hooks/pre-commit.sample
./.git/hooks/update.sample
./.git/refs
./.git/refs/heads
./.git/refs/tags
./.git/config
./.git/objects
./.git/objects/pack
./.git/objects/info
./.git/description
./.git/HEAD
./.git/branches
./.git/info
./.git/info/exclude


```

可以看到，.git目录包含很多内容。这些文件是基于模板目录显示的，根据需要可以进行调整。根据使用的Git的版本，实际列表可能看起来会有一点不同。例如，旧版本的Git不对.git/hooks 文件使用.sample 后缀。

在一般情况下，不需要查看或者操作.git目录下的文件。认为这些“隐藏”的文件是Git底层（plumbing）或者配置的一部分。Git有一小部分底层命令来处理这些隐藏的文件，但是你很少会用到它们。

最初，除了几个占位符之外，.git/objects 目录（用来存放所有Git对象的目录）是空的。
```text
$ find .git/objects

.git/objects
.git/objects/pack
.git/objects/info
```





现在，让我们来小心地创建一个简单的对象。

```text
$ echo "hello world" > hello.txt




$ git add hello.txt

```








如果输入的“hello world”跟这里一样（没有改变间距和大小写），那么objects目录应该如下所示：

```text
$ find .git/objects




.git/objects
.git/objects/pack
.git/objects/3b
.git/objects/3b/18e512dba79e4c8300dd08aeb37f8e728b8dad
.git/objects/info



```


所有这一切看起来很神秘。其实不然，下面各节会慢慢解释原因。

#### <a id='4.3.2' href='#c4.3.2'>4.3.2　对象、散列和blob</a>

当为hello.txt 创建一个对象的时候，Git并不关心hello.txt 的文件名。Git只关心文件里面的内容：表示“hello world”的12个字节和换行符（跟之前创建的blob一样）。Git对这个blob执行一些操作，计算它的SHA1散列值，把散列值的十六进制表示作为文件名它放进对象库中。

```text
如何知道一个SHA1散列值是唯一的？

两个不同blob产生相同SHA1散列值的机会十分渺茫。当这种情况发生的时候，称为一次碰撞。然而，一次SHA1碰撞的可能性太低，你可以放心地认为它不会干扰我们对Git的使用。

SHA1是“安全散列加密”算法。直到现在，没有任何已知的方法（除了运气之外）可以让一个用户刻意造成一次碰撞。但是碰撞会随机发生吗？让我们来看看。

对于160位数，你有2160 或者大约1048 （1后面跟48个0）种可能的SHA1散列值。这个数是极其巨大的。即使你雇用一万亿人来每秒产生一万亿个新的唯一blob对象，持续一万亿年，你也只有1043 个blob对象。

如果你散列了280 个随机blob，可能会发生一次碰撞。

不相信我们的话，就去读读Bruce Schneier的书吧 ② 。
```

在这种情况下散列值是3b18e512dba79e4c8300dd08aeb37f8e728b8dad。160位的SHA1散列值对应20个字节，这需要40个字节的十六进制来显示，因此这内容另存为.git/objects/3b/18e512dba79e4c8300dd08aeb37f8e728b8dad 。Git在前两个数字后面插入一个“/”以提高文件系统效率（如果你把太多的文件放在同一个目录中，一些文件系统会变慢；使SHA1的第一个字节成为一个目录是一个很简单的办法，可以为所有均匀分布的可能对象创建一个固定的、256路分区的命名空间）。

为了展示Git真的没有对文件的内容做很多事情（它还是同样的内容“hello world”），可以在任何时间使用散列值把它从对象库里提取出来。

```text
$ git cat-file -p 3b18e512dba79e4c8300dd08aeb37f8e728b8dad




hello world
```

提示

Git也知道手动输入40个字符是很不切实际的，因此它提供了一个命令通过对象的唯一前缀来查找对象的散列值。

```text

# 注意，前面3b是文件夹名称，连写就行，不要用任何东西分割
$ git rev-parse 3b18e512d




3b18e512dba79e4c8300dd08aeb37f8e728b8dad
```

##### 我的补充

我新建了一个git仓库，然后执行了如下git命令：
```text
$ touch a.txt
$ echo "hello world" > a.txt
$ git add a.txt
$ touch b.txt
$ echo "hello world" > b.txt
$ git add b.txt

```
![](https://github.com/YuxingXie/git_study/raw/master/assets/image/04-03-01-01.png) 

可以看到在.git/objects/3b目录下并没有两个文件。然后，我继续执行如下命令：
```text
$ echo "hello git" > b.txt
$ git add b.txt 
```
![](https://github.com/YuxingXie/git_study/raw/master/assets/image/04-03-01-02.png) 

可以看到并没有在3d目录下多出一个文件，而是多出一个8d/0e41234f24b6da002d962a26c2495ea16a425f文件。
所以工作区的文件目录与git仓库并不是简单的做一个映射而已，也就是书中所说的"目录树"有自己的一套规则。

另外，文件内容都为"hello world"的两个文件,git并没有创建一个object,而是引用同一个object。为了验证这一点，做如下操作：

```text
$ mkdir t
$ cd t
$ touch c.txt
$ echo "hello world" > c.txt
$ git add c.txt 

```
可以看到，在objects下没有新目录和文件生产，这似乎印证了我的想法，但是别急，看下面的操作：
```text
$ git commit --all -m 'sss'
[master (root-commit) 19cfe15] sss
 3 files changed, 3 insertions(+)
 create mode 100644 a.txt
 create mode 100644 b.txt
 create mode 100644 t/c.txt
```
![](https://github.com/YuxingXie/git_study/raw/master/assets/image/04-03-01-03.png) 

喔,提交(commit)以后，objects下多出了6a、19、c4三个文件夹。

```text
$ find .git/objects
.git/objects
.git/objects/3b
.git/objects/3b/18e512dba79e4c8300dd08aeb37f8e728b8dad
.git/objects/6a
.git/objects/6a/b6f1e2bd40b2a0440de63c2e235c22c3201a91
.git/objects/.DS_Store
.git/objects/pack
.git/objects/19
.git/objects/19/cfe1593d7232f7ee419a9a171d09ae309fdc48
.git/objects/info
.git/objects/c4
.git/objects/c4/a1f291510b4b1a7065e4e18143b8af822d5bbb
.git/objects/8d
.git/objects/8d/0e41234f24b6da002d962a26c2495ea16a425f
```
3b文件夹里面的文件的散列值并没有变化，而生成的新文件中并没有和3b文件夹相同散列值的文件，我用git cat-file看看这些文件都是什么:

```text
# git cat-file 看看6a目录下的这个文件代表什么
git cat-file -p git cat-file -p 6ab6f1e2bd40b2a0440de63c2e235c22c3201a91

100644 blob 3b18e512dba79e4c8300dd08aeb37f8e728b8dad	a.txt
100644 blob 8d0e41234f24b6da002d962a26c2495ea16a425f	b.txt
040000 tree c4a1f291510b4b1a7065e4e18143b8af822d5bbb	t
```
所以6a下的这个文件(散列码)包含三个对象：a.txt,b.txt,t。可以认为它表示根目录树结构。

再看看19和c4：
```text
git cat-file -p 19cfe1593d7232f7ee419a9a171d09ae309fdc48
tree 6ab6f1e2bd40b2a0440de63c2e235c22c3201a91
author yuxingxie <185246042@qq.com> 1605601275 +0800
committer yuxingxie <185246042@qq.com> 1605601275 +0800

sss

```


#### <a id='4.3.3' href='#c4.3.3'>4.3.3　文件和树</a>


既然“hello world”那个blob已经安置在对象库里了，那么它的文件名又发生了什么事呢？如果不能通过文件名找到文件Git就太没用了。

正如前面提到的，Git通过另一种叫做目录树（tree）的对象来跟踪文件的路径名。当使用git add命令时，Git会给添加的每个文件的内容创建一个对象，但它并不会马上为树创建一个对象。相反，索引更新了。索引位于.git/index 中，它跟踪文件的路径名和相应的blob。每次执行命令（比如，git add、git rm或者git mv）的时候，Git会用新的路径名和blob信息来更新索引。

任何时候，都可以从当前索引创建一个树对象，只要通过底层的git write-tree命令来捕获索引当前信息的快照就可以了。

目前，该索引只包含一个文件，hello.txt.

```text
$ git ls-files -s




100644 3b18e512dba79e4c8300dd08aeb37f8e728b8dad 0　　　hello.txt



```


在这里你可以看到文件的关联，hello.txt 与3b18e4...的blob。

接下来，让我们捕获索引状态并把它保存到一个树对象里。
```text

$ git write-tree




68aba62e560c0ebc3396e8ae9335232cd93a3f60

$ find .git/objects
.git/objects
.git/objects/68
.git/objects/68/aba62e560c0ebc3396e8ae9335232cd93a3f60
.git/objects/pack
.git/objects/3b
.git/objects/3b/18e512dba79e4c8300dd08aeb37f8e728b8dad
.git/objects/info



```


现在有两个对象：3b18e5的“hello world”对象和一个新的68aba6树对象。可以看到，SHA1对象名完全对应.git/objects 下的子目录和文件名。

但是树是什么样子的呢？因为它是一个对象，就像blob一样，所以可以用底层命令来查看它。
```text
# NOTE:记住这个命令
$ git cat-file -p 68aba6
100644 blob 3b18e512dba79e4c8300dd08aeb37f8e728b8dad　　 hello.txt
```



对象的内容应该很容易解释。第一个数100644，是对象的文件属性的八进制表示，用过UNIX的chmod命令的人应该对这个很熟悉了。这里，3b18e5是hello world 的blob的对象名，hello.txt 是与该blob关联的名字。

当执行git ls-file -s的时候，很容易就可以看到树对象已经捕获了索引中的信息。

#### <a id='4.3.4' href='#c4.3.4'>4.3.4　对Git使用SHA1的一点说明</a>

在更详细地讲解树对象的内容之前，让我们先来看看SHA1散列的一个重要特性。

#### <a id='4.3.5' href='#c4.3.5'>4.3.5　树层次结构</a>

#### <a id='4.3.6' href='#c4.3.6'>4.3.6　提交</a>

#### <a id='4.3.7' href='#c4.3.7'>4.3.7　标签</a>




## <a id='5' href='#c5'>第5章 文件索引和管理</a>

## <a id='6' href='#c6'>第6章 提交</a>

## <a id='7' href='#c7'>第7章 分支</a>

## <a id='8' href='#c8'>第8章 diff</a>

## <a id='9' href='#c9'>第9章 合并</a>

## <a id='10' href='#c10'>第10章 更改提交</a>

## <a id='11' href='#c11'>第11章 储存和引用日志</a>

## <a id='12' href='#c12'>第12章 远程版本控制</a>

## <a id='13' href='#c13'>第13章 版本库管理</a>

## <a id='14' href='#c14'>第14章 补丁</a>

## <a id='15' href='#c15'>第15章 钩子</a>

## <a id='16' href='#c16'>第16章 合并项目</a>

## <a id='17' href='#c17'>第17章 子模块最佳实践</a>

## <a id='18' href='#c18'>第18章 结合SVN版本库使用Git</a>

## <a id='19' href='#c19'>第19章 高级操作</a>

## <a id='20' href='#c20'>第20章 提示、技巧和技术</a>

## <a id='21' href='#c21'>第21章 Git和GitHub</a>

