
# Git版本控制管理

参考书籍：

* 《Git版本控制管理》(Jon Loeliger & Mattbew McCullough)

* <a href='https://git-scm.com/book/en/v2'>《Pro Git》</a>

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
>>>
>>> <a id='c4.1.1' href='#4.1.1'>4.1.1　版本库</a>
>>>
>>> <a id='c4.1.2' href='#4.1.2'>4.1.2　Git对象类型</a>
>>>
>>> <a id='c4.1.3' href='#4.1.3'>4.1.3　索引</a>
>>>
>>> <a id='c4.1.4' href='#4.1.4'>4.1.4　可寻址内容名称</a>
>>>
>>> <a id='c4.1.5' href='#4.1.5'>4.1.5　Git追踪内容</a>
>>>
>>> <a id='c4.1.6' href='#4.1.6'>4.1.6　路径名与内容</a>
>>>
>>> <a id='c4.1.7' href='#4.1.7'>4.1.7　打包文件</a>
>>
>> <a href='#4.2' id='c4.2'>4.2 对象库图示</a>
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
>>
>> <a id='cafter4' href='#after4'>第4章个人总结</a>
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
>>> <a href='#after6.2.2' id='cafter6.2.2'>补充内容:master,head,origin等概念</a>
>>>
>>> <a href='#6.2.3' id='c6.2.3'>6.2.3 相对提交名</a>
>>
>> <a href='#6.3' id='c6.3'>6.3 提交历史记录</a>
>>>
>>> <a href='#6.3.1' id='c6.3.1'>6.3.1 查看旧提交</a>
>>>
>>> <a href='#6.3.2' id='c6.3.2'>6.3.2 提交图</a>
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
>>
>> <a href='#8.1' id='c8.1'>8.1 git diff命令的格式</a>
>>
>> <a href='#8.2' id='c8.2'>8.2 简单的git diff例子</a>
>>
>> <a href='#8.3' id='c8.3'>8.3 git diff和提交范围</a>
>>
>> <a href='#8.4' id='c8.4'>8.4 路径限制的git diff</a>
>>
>> <a href='#8.5' id='c8.5'>8.5 比较SVN和Git如何产生diff</a>
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
**NOTE：这些东西多用就熟悉并能融会贯通，没必要死记硬背。**
```

* "git --选项"，选项包括：version,help等十来个，记得前面带上"--"，如：git --version；

* "git 子命令"，如: "git pull"；

* "git 子命令 --子命令选项"，如："git commit --amend"，这里--amend是commit子命令的专用子命令选项，
当然应该还有非专用的子命令选项比如常用的"git commit --all；

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
**NOTE:git add并不仅仅只是添加新文件,当文件状态是modified的时候，git add可以将改变的文件重新暂存。可以这样理解：staged状态的文件，
暂存起来的内容和正在编辑的内容是一样的，它们随时可以提交。**


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

**NOTE:根据命令提示，(use "git restore --staged <file>..." to unstage)，我尝试将一个已暂存的文件a.txt移出版本库：**

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
**NOTE:commit提交那些被add的文件，add之后如果文件有变化，这些变化不会被提交到版本库。所以除非特殊情况，
commit之前确认是否add可能是个好习惯。**

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

**NOTE:记得add! 书上说文件已经添加到版本库就没必要add，这与我使用的结果不一样。这是版本差异还是作者错了？**

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

**NOTE:另外，我认为还有一个重要的命令需要了解一下：**
```text
git rev-list --all
会列出所有的提交散列值。
```

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
**NOTE:这个先不重点学习**

有几个地方可以找到配置文件，并有不同的优先级。

* .git/config(版本库特定)

* ~/.gitconfig(用户级别)

* /etc/gitconfig(linux系统级)

* /usr/local/git/etc/gitconfig(我的mac，不知道是不是系统级)



## <a id='4' href='#c4'>第四章 基本的Git概念</a>

**NOTE:本章多为概念和原理，所以先照抄一遍。**

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

下面这个命令可以根据索引索引生成树：
```text
git write-tree
```

该命令详见4.3.3<a href='c4.3.3'>文件和树</a>和4.3.4<a href='c4.3.4'>对Git使用SHA1的一点说明</a>。

#### <a id='4.1.4' href='#c4.1.4'>4.1.4 可寻址内容名称</a>

* 原文

Git对象库被组织及实现成一个内容寻址的存储系统。具体而言，对象库中的每个对象都有一个唯一的名称，
这个名称是向对象的内容应用SHA1得到的SHA1散列值。因为一个对象的完整内容决定了这个散列值，并且认为这个散列值能有效并唯一地对应特定的内容，
所以SHA1散列值用来做对象数据库中对象的名字和索引是完全充分的。文件的任何微小变化都会导致SHA1散列值的改变，使得文件的新版本被单独编入索引。

SHA1的值是一个160位的数，通常表示为一个40位的十六进制数，比如，9da581d910c9c4ac93557ca4859e767f5caf5169。有时候，在显示期间，
SHA1值被简化成一个较小的、唯一的前缀。Git用户所说的SHA1、散列码和对象ID都是指同一个东西。


#### <a id='4.1.5' href='#c4.1.5'>4.1.5 Git追踪内容</a>

* 原文

理解Git不仅仅是一个VCS是很重要的，Git同时还是一个内容追踪系统（content tracking system）。这种区别尽管很微小，但是指导了Git的很多设计，
并且也许这就是处理内部数据操作相对容易的关键原因。然而，因为这也可能是对新手来讲最难把握的概念之一，所以做一些论述是值得的。

Git的内容追踪主要表现为两种关键的方式，这两种方式与大多数其他 ① 修订版本控制系统都不一样。

首先，Git的对象库基于其对象内容的散列计算的值，而不是基于用户原始文件布局的文件名或目录名设置。因此，当Git放置一个文件到对象库中的时候，
它基于数据的散列值而不是文件名。事实上，Git并不追踪那些与文件次相关的文件名或者目录名。再次强调，Git追踪的是内容而不是文件。

如果两个文件的内容完全一样，无论是否在相同的目录，Git在对象库里只保存一份blob形式的内容副本。Git仅根据文件内容来计算每一个文件的散列码，
如果文件有相同的SHA1值，它们的内容就是相同的，然后将这个blob对象放到对象库里，并以SHA1值作为索引。项目中的这两个文件，
不管它们在用户的目录结构中处于什么位置，都使用那个相同的对象指代其内容。

如果这些文件中的一个发生了变化，Git会为它计算一个新的SHA1值，识别出它现在是一个不同的blob对象，然后把这个新的blob加到对象库里。
原来的blob在对象库里保持不变，为没有变化的文件所使用。

其次，当文件从一个版本变到下一个版本的时候，Git的内部数据库有效地存储每个文件的每个版本，而不是它们的差异。
因为Git使用一个文件的全部内容的散列值作为文件名，所以它必须对每个文件的完整副本进行操作。
Git不能将工作或者对象库条目建立在文件内容的一部分或者文件的两个版本之间的差异上。

文件拥有修订版本和从一个版本到另一个版本的步进，用户的典型看法是这种文件简直是个工艺品。Git用不同散列值的blob之间的区别来计算这个历史，
而不是直接存储一个文件名和一系列差异。这似乎有些奇怪，但这个特性让Git在执行某些任务的时候非常轻松。


#### <a id='4.1.6' href='#c4.1.6'>4.1.6　路径名与内容</a>

* 原文

跟很多其他VCS一样，Git需要维护一个明确的文件列表来组成版本库的内容。然而，这个需求并不需要Git的列表基于文件名。实际上，
Git把文件名视为一段区别于文件内容的数据。这样，Git就把索引从传统数据库的数据中分离出来了。看看表4-1会很有帮助，
它粗略地比较了Git和其他类似的系统。



<p align="center">表4-1　数据库对比</p>



| 系统 | 索引机制 | 数据存储 |
| :---: | :----: | :----: |
| 传统数据库 | 索引顺序存取方法（ISAM） | 数据记录 |
| UNIX文件系统    | 目录（/path/to/file ）      | 数据块|
| Git    | .git/objects/hash 、树对象内容| blob对象、树对象|


文件名和目录名来自底层的文件系统，但是Git并不真正关心这些名字。Git仅仅记录每个路径名，并且确保能通过它的内容精确地重建文件和目录，
这些是由散列值来索引的。

Git的物理数据布局并不模仿用户的文件目录结构。相反，它有一个完全不同的结构却可以重建用户的原始布局。在考虑其自身的内部操作和存储方面，
Git的内部结构是一种更高效的数据结构。

当Git需要创建一个工作目录时，它对文件系统说：“嘿！我这有这样大的一个blob数据，应该放在路径名为path/to/directory/file 的地方。你能理解吗？
”文件系统回复说：“啊，是啊，我认出那个字符串是一组子目录名，并且我知道把你的blob数据放在哪里！谢谢！”

#### <a id='4.1.7' href='#c4.1.7'>4.1.7　打包文件</a>

* 原文

一个聪明的读者也许已经有了关于Git的数据模型及其单独文件存储的挥之不去的问题：直接存储每个文件每个版本的完整内容是否太低效率了？
即使它是压缩的，把相同文件的不同版本的全部内容都存储的效率是否太低了？
如果你只添加一行到文件里，Git是不是要存储两个版本的全部内容？

幸运的是，答案是“不是，不完全是！”

相反，Git使用了一种叫做 打包文件（pack file） 的更有效的存储机制。要创建一个打包文件，Git首先定位内容非常相似的全部文件，
然后为它们之一存储整个内容。之后计算相似文件之间的差异并且只存储差异。
例如，如果你只是更改或者添加文件中的一行，Git可能会存储新版本的全部内容，然后记录那一行更改作为差异，并存储在包里。

存储一个文件的整个版本并存储用来构造其他版本的相似文件的差异并不是一个新伎俩。这个机制已经被其他VCS（如RCS）用了好几十年了，
它们的方法本质上是相同的。

然而，Git文件打包得非常巧妙。因为Git是由内容驱动的，所以它并不真正关心它计算出来的两个文件之间的差异是否属于同一个文件的两个版本。这就是说，
Git可以在版本库里的任何地方取出两个文件并计算差异，
只要它认为它们足够相似来产生良好的数据压缩。因此，Git有一套相当复杂的算法来定位和匹配版本库中潜在的全局候选差异。
此外，Git可以构造一系列差异文件，从一个文件的一个版本到第二个，第三个，等等。

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

图4-1展示了所有部分如何协作。这张图显示了一个版本库在添加了两个文件的初始提交后的状态。两个文件都在顶级目录中。
同时它们的master分支和一个叫V1.0的标签都指向ID为1492的提交对象。


![](https://github.com/YuxingXie/git_study/raw/master/assets/image/04-01.jpg)  

图4-1　Git对象

现在，让我们使事情变得复杂一点。保留原来的两个文件不变，添加一个包含一个文件的新子目录。对象库就如图4-2所示。

![](https://github.com/YuxingXie/git_study/raw/master/assets/image/04-02.jpg)  

图4-2　二次提交后的Git对象


就像前一张图里，新提交对象添加了一个关联的树对象来表示目录和文件结构的总状态。在这里，它是ID为cafed00d的树对象。

因为顶级目录被添加的新子目录改变了，顶级树对象的内容也跟着改变了，所以Git引进了一个新的树对象：cafed00d。

然而，blob对象dead23和feeb1e在从第一次到第二次提交的时候没有发生变化。Git意识到ID没有变化，所以可以被新的cafed00d树对象直接引用和共享。

请注意提交对象之间箭头的方向。父提交在时间上来得更早。因此，在Git的实现里，每个提交对象指回它的一个或多个父提交。很多人对此感到困惑，
因为版本库的状态通常画成反方向：数据流从父提交流向子提交。

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

可以看到，.git目录包含很多内容。这些文件是基于模板目录显示的，根据需要可以进行调整。根据使用的Git的版本，实际列表可能看起来会有一点不同。
例如，旧版本的Git不对.git/hooks 文件使用.sample 后缀。

在一般情况下，不需要查看或者操作.git目录下的文件。认为这些“隐藏”的文件是Git底层（plumbing）或者配置的一部分。
Git有一小部分底层命令来处理这些隐藏的文件，但是你很少会用到它们。

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

**NOTE:散列值就是文件blob对象的40位字符串表示法。**

当为hello.txt 创建一个对象的时候，Git并不关心hello.txt 的文件名。Git只关心文件里面的内容：表示“hello world”的12个字节和换行符
（跟之前创建的blob一样）。Git对这个blob执行一些操作，计算它的SHA1散列值，把散列值的十六进制表示作为文件名它放进对象库中。



```text

如何知道一个SHA1散列值是唯一的？

两个不同blob产生相同SHA1散列值的机会十分渺茫。当这种情况发生的时候，称为一次碰撞。
然而，一次SHA1碰撞的可能性太低，你可以放心地认为它不会干扰我们对Git的使用。

SHA1是“安全散列加密”算法。直到现在，没有任何已知的方法（除了运气之外）可以让一个用户刻意造成一次碰撞。
但是碰撞会随机发生吗？让我们来看看。

对于160位数，你有2160 或者大约1048 （1后面跟48个0）种可能的SHA1散列值。
这个数是极其巨大的。即使你雇用一万亿人来每秒产生一万亿个新的唯一blob对象，持续一万亿年，你也只有1043 个blob对象。

如果你散列了280 个随机blob，可能会发生一次碰撞。

不相信我们的话，就去读读Bruce Schneier的书吧 ② 。

```


在这种情况下散列值是3b18e512dba79e4c8300dd08aeb37f8e728b8dad。160位的SHA1散列值对应20个字节，这需要40个字节的十六进制来显示，
因此这内容另存为.git/objects/3b/18e512dba79e4c8300dd08aeb37f8e728b8dad 。Git在前两个数字后面插入一个“/”以提高文件系统效率（
如果你把太多的文件放在同一个目录中，一些文件系统会变慢；使SHA1的第一个字节成为一个目录是一个很简单的办法，
可以为所有均匀分布的可能对象创建一个固定的、256路分区的命名空间）。

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
$ git cat-file -p 3b18e512dba79e4c8300dd08aeb37f8e728b8dad
hello world

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
$ git cat-file -p 6ab6f1e2bd40b2a0440de63c2e235c22c3201a91

100644 blob 3b18e512dba79e4c8300dd08aeb37f8e728b8dad	a.txt
100644 blob 8d0e41234f24b6da002d962a26c2495ea16a425f	b.txt
040000 tree c4a1f291510b4b1a7065e4e18143b8af822d5bbb	t
```
所以6a下的这个文件(散列码)包含三个对象：a.txt,b.txt,t。可以认为它表示根目录树结构。

再看看19和c4：
```text


$ git cat-file -p 19cfe1593d7232f7ee419a9a171d09ae309fdc48
tree 6ab6f1e2bd40b2a0440de63c2e235c22c3201a91
author yuxingxie <185246042@qq.com> 1605601275 +0800
committer yuxingxie <185246042@qq.com> 1605601275 +0800

sss

$ git cat-file -p c4a1f291510b4b1a7065e4e18143b8af822d5bbb
100644 blob 3b18e512dba79e4c8300dd08aeb37f8e728b8dad	c.txt

```
注意一点，我们使用git cat-file -p命令后，获得的信息有可能是：
* 内容，如:hello world
* blob，指向一个文件
* tree，指向一个目录，比如上面的6ab6f1e2bd40b2a0440de63c2e235c22c3201a91，似乎是git项目的根目录，
而c4a1f291510b4b1a7065e4e18143b8af822d5bbb则是t目录。

#### <a id='4.3.3' href='#c4.3.3'>4.3.3　文件和树</a>


既然“hello world”那个blob已经安置在对象库里了，那么它的文件名又发生了什么事呢？如果不能通过文件名找到文件Git就太没用了。

正如前面提到的，Git通过另一种叫做目录树（tree）的对象来跟踪文件的路径名。当使用git add命令时，Git会给添加的每个文件的内容创建一个对象，
但它并不会马上为树创建一个对象。相反，索引更新了。索引位于.git/index 中，它跟踪文件的路径名和相应的blob。每次执行命令
（比如，git add、git rm或者git mv）的时候，Git会用新的路径名和blob信息来更新索引。

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
**NOTE:记住这个命令git cat-file -p**
```text
$ git cat-file -p 68aba6
100644 blob 3b18e512dba79e4c8300dd08aeb37f8e728b8dad　　 hello.txt
```

对象的内容应该很容易解释。第一个数100644，是对象的文件属性的八进制表示，用过UNIX的chmod命令的人应该对这个很熟悉了。这里，
3b18e5是hello world 的blob的对象名，hello.txt 是与该blob关联的名字。

当执行git ls-file -s的时候，很容易就可以看到树对象已经捕获了索引中的信息。

#### <a id='4.3.4' href='#c4.3.4'>4.3.4　对Git使用SHA1的一点说明</a>

**NOTE:git write-tree命令，大致这样理解吧：git仓库中有个索引，根据这个索引可以生成一个树形对象。根据前面的研究，树可以包含(引用)其它的树，
所以我猜测，这个树应该是根目录树。**

我来证实一下我的猜测：

```text
$ git write-tree
6ab6f1e2bd40b2a0440de63c2e235c22c3201a91
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

$ git cat-file -p 6ab6f1e2bd40b2a0440de63c2e235c22c3201a91 
100644 blob 3b18e512dba79e4c8300dd08aeb37f8e728b8dad	a.txt
100644 blob 8d0e41234f24b6da002d962a26c2495ea16a425f	b.txt
040000 tree c4a1f291510b4b1a7065e4e18143b8af822d5bbb	t
```
没错，根据索引生成的tree的散列值(SHA1)就是根目录的散列值。


```text
命名
git-write-tree  - 从当前索引创建一个树形对象

概要
git write-tree [--missing-ok] [--prefix=<prefix>/]
描述
使用当前索引创建树对象。新树对象的名称被打印到标准输出。

索引必须处于完全合并状态。

从概念上讲，git write-treesync（）将当前索引内容同步到一组树文件中。
为了让您的目录中的内容与您的目录匹配，您需要先完成一个git update-index阶段git write-tree。

选项
   --missing-ok   

通常git write-tree确保目标引用的对象存在于对象数据库中。该选项禁用此检查。

   --prefix=<prefix>/   

写一个表示子目录的树对象<prefix>。这可以用于为位于指定子目录中的子项目编写树对象。

```


* 原文

在更详细地讲解树对象的内容之前，让我们先来看看SHA1散列的一个重要特性。
```text
$ git write-tree
68aba62e560c0ebc3396e8ae9335232cd93a3f60

$ git write-tree
68aba62e560c0ebc3396e8ae9335232cd93a3f60

$ git write-tree
68aba62e560c0ebc3396e8ae9335232cd93a3f60
```

每次对相同的索引计算一个树对象，它们的SHA1散列值仍是完全一样的。Git并不需要重新创建一个新的树对象。如果你在计算机前按照这些步骤操作，
你应该看到完全一样的SHA1散列值，跟本书所刊印的一样。

这样看来，散列函数在数学意义上是一个真正的函数：对于一个给定的输入，它总产生相同的输出。这样的散列函数有时也称为摘要，
用来强调它就像散列对象的摘要一样。当然，任何散列函数（即使是低级的奇偶校验位）也有这个属性。

这是非常重要的。例如，如果你创建了跟其他开发人员相同的内容，无论你俩在何时何地工作，相同的散列值就足以证明全部内容是一致的。
事实上，Git确实将它们视为一致的。

但是等一下——SHA1散列是唯一的吗？难道万亿人每秒产生的万亿个blob永远不会产生一次碰撞吗？这在Git新手中是一个常见的疑惑。因此，请仔细阅读，
因为如果你能理解这种区别，那么本章的其他内容就很简单了。

在这种情况下，相同的SHA1散列值并不算碰撞。只有两个不同的对象产生一个相同的散列值时才算碰撞。在这里，你创建了相同内容的两个单独实例，
相同的内容始终有相同的散列值。

Git依赖于SHA1散列函数的另一个后果：你是如何得到称为68aba62e560c0ebc3396 e8ae9335232cd93a3f60的树的并不重要。如果你得到了它，
你就可以非常有信心地说，它跟本书的另一个读者的树对象是一样的。
Bob通过合并Jennie的提交A、提交B和Sergey的提交C来创建这个树，而你是从Sue得到提交A，然后从Lakshmi那里更新提交B和提交C的合并。
结果都是一样的，这有利于分布式开发。

如果要求你查看对象68aba62e560c0ebc3396e8ae9335232cd93a3f60，并且你能找到这样的一个对象，同时因为SHA1是一个加密散列算法，
因此你就可以确信你找的对象跟散列创建时的那个对象的数据是相同的。

反过来也是如此：如果你在你的对象库里没找到具有特定散列值的对象，那么你就可以肯定你没有持有那个对象的副本。
总之，你可以判断你的对象库是否有一个特定的的对象，即使你对它（可能非常大）的内容一无所知。因此，散列就好似对象的可靠标签或名称。

但是Git也依赖于比那个结论更强的东西。考虑最近的一次提交（或者它关联的树对象）。因为它包含其父提交以及树的散列，
反过来又通过递归整个数据结构包含其所有子树和blob的散列，因此可归结为它通过原始提交的散列值唯一标识整个数据结构在提交时的状态。

最后，我们在上一段中的声明可以推出散列函数的强大应用：它提供了一种有效的方法来比较两个对象，甚至是两个非常大而复杂的数据结构 ③ ，
而且并不需要完全传输。

#### <a id='4.3.5' href='#c4.3.5'>4.3.5　树层次结构</a>
* 原文

只有单个文件的信息是很好管理的，就像上一节所讲的一样，但项目包含复杂而且深层嵌套的目录结构，并且会随着时间的推移而重构和移动。
通过创建一个新的子目录，该目录包含hello.txt 的一个完全相同的副本，让我们看看Git是如何处理这个问题的。

```text
$ pwd
/tmp/hello

$ mkdir subdir

$ cp hello.txt subdir/

$ git add subdir/hello.txt

$ git write-tree
492413269336d21fac079d4a4672e55d5d2147ac

$ git cat-file -p 4924132693
100644 blob 3b18e512dba79e4c8300dd08aeb37f8e728b8dad　　hello.txt
040000 tree 68aba62e560c0ebc3396e8ae9335232cd93a3f60　　subdir

```
新的顶级树包含两个条目：原始的hello.txt 以及新的 子目录 ，子目录是 树 而不是blob。

注意到不寻常之处了吗？仔细看subdir 的对象名。是你的老朋友，68aba62e560c0 ebc3396e8ae9335232cd93a3f60！

刚刚发生了什么？subdir 的新树只包含一个文件hello.txt ，该文件跟旧的“hello world”内容相同。所以subdir 树跟以前的顶级树是完全一样的！
当然它就有跟之前一样的SHA1对象名了。

**NOTE:所以一个目录的SHA1值跟目录的名称没什么关系，只跟里面的内容有关系。**

让我们来看看.git/objects 目录，看看最近的更改有哪些影响。

```text
$ find .git/objects
.git/objects
.git/objects/49
.git/objects/49/2413269336d21fac079d4a4672e55d5d2147ac
.git/objects/68
.git/objects/68/aba62e560c0ebc3396e8ae9335232cd93a3f60
.git/objects/pack
.git/objects/3b
.git/objects/3b/18e512dba79e4c8300dd08aeb37f8e728b8dad
.git/objects/info

```
这只有三个唯一的对象：一个包含“hello world”的blob；一棵包含hello.txt 的树，文件里是“hello world”加一个换行；
还有第一棵树旁边包含hello.txt 的另一个索引的另一棵树。

#### <a id='4.3.6' href='#c4.3.6'>4.3.6　提交</a>

**NOTE:根据作者的意思，使用git commit-tree提交与git commit提交效果应该是一样的，
然而当我这样做以后，使用git status查看，发现文件未被提交：**
```text
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.MD

no changes added to commit (use "git add" and/or "git commit -a")
```

* 原文

讨论的下一主题是提交（commit）。现在hello.txt 已经通过git add命令添加了，树对象也通过git write-tree命令生成了，
可以像这样用底层命令那样创建提交对象。

```text
# echo -n 不换行输出
$ echo -n "Commit a file that says hello\n" | git commit-tree 492413269336d21fac079d4a4672e55d5d2147ac
3ede4622cc241bcb09683af36360e7413b9ddf6c
```
结果如下所示。
```text
$ git cat-file -p 3ede462
tree 492413269336d21fac079d4a4672e55d5d2147ac
author Jon Loeliger <jdl@example.com> 1220233277 -0500
committer Jon Loeliger <jdl@example.com> 1220233277 -0500

Commit a file that says hello
```
如果你在计算机上按步骤操作，你可能会发现你生成的提交对象跟书上的名字不一样。如果你已经理解了目前为止的一切内容，那原因就很明显了：
这是不同的提交。提交包含你的名字和创建提交的时间，尽管这区别很微小，但依然是不同的。另一方面，你的提交确实有相同的树。
这就是提交对象与它们的树对象分开的原因：不同的提交经常指向同一棵树。当这种情况发生时，Git能足够聪明地只传输新的提交对象，这是非常小的，
而不是很可能很大的树和blob对象。

在实际生活中，你可以（并且应该）跳过底层的git write-tree和git commit-tree步骤，并只使用git commit命令。成为一个完全快乐的Git用户，
你不需要记住那些底层命令。

一个基本的提交对象是相当简单的，这是成为一个真正的RCS需要的最后组成部分。提交对象可能是最简单的一个，包含：

标识关联文件的树对象的名称；
创作新版本的人（作者）的名字和创作的时间；
把新版本放到版本库的人（提交者）的名字和提交的时间；
对本次修订原因的说明（提交消息）。
默认情况下，作者和提交者是同一个人，也有一些情况下，他们是不同的。
```text
提示

可以使用git show --pretty=fuller命令来查看给定提交的其他细节。
```


尽管提交对象跟树对象用的结构是完全不同的，但是它也存储在图结构中。当你做一个新提交时，你可以给它一个或多个父提交。通过继承链来回溯，
可以查看项目历史。

第6章会给出关于提交和提交图的更详细描述。


#### <a id='4.3.7' href='#c4.3.7'>4.3.7　标签</a>

* 原文

最后，Git还管理的一个对象就是标签。尽管Git只实现了一种标签对象，但是有两种基本的标签类型，通常称为轻量级的（lightweight）
和带附注的（annotated）。

轻量级标签只是一个提交对象的引用，通常被版本库视为是私有的。这些标签并不在版本库里创建永久对象。带标注的标签则更加充实，并且会创建一个对象。
它包含你提供的一条消息，并且可以根据RFC 4880来使用GnuPG密钥进行数字签名。

Git在命名一个提交的时候对轻量级的标签和带标注的标签同等对待。不过，默认情况下，很多Git命令只对带标注的标签起作用，
因为它们被认为是“永久”的对象。

可以通过git tag命令来创建一个带有提交信息、带附注且未签名的标签：

```text
# 给3ede462这次提交命一个tag名
# 如果还记得git log，git rev-list这几个命令，我们可以使用这个命令获得提交历史
$ git tag -m "Tag version 1.0" V1.0 3ede462

```

可以通过git cat-file -p命令来查看标签对象，但是标签对象的SHA1值是什么呢？为了找到它，使用4.3.2节的提示。

```text
$ git rev-parse V1.0
6b608c1093943939ae78348117dd18b1ba151c6a

$ git cat-file -p 6b608c
object 3ede4622cc241bcb09683af36360e7413b9ddf6c
type commit
tag V1.0
tagger Jon Loeliger <jdl@example.com> Sun Oct 26 17:07:15 2008 -0500

Tag version 1.0
```


除了日志消息和作者信息之外，标签指向提交对象3ede462。通常情况下，Git通过某些分支来给特定的提交命名标签。请注意，
这种行为跟其他VCS有明显的不同。

Git通常给指向树对象的提交对象打标签，这个树对象包含版本库中文件和目录的整个层次结构的总状态。

回想一下图4-1，V1.0标签指向提交1492——依次指向跨越多个文件的树（8675309）。因此，这个标签同时适用于该树的所有文件。

这跟CVS不同，例如，对每个单独的文件应用标签，然后依赖所有打过标签的文件来重建一个完整的标记修订。并且CVS允许你移动单独文件的标签，
而Git则需要在标签移动到的地方做一个新的提交，囊括该文件的状态变化。

① 　Monotone、Mercurial、OpenCMS和Venti是一些值得注意的例外。——原注

② 　《应用密码学》的作者、美国密码学学者、信息安全专家与作家。——译者注

③ 　对这个数据结构更详细的描述见6.3.2节。——原注

### <a id='after4' href='#cafter4'>第4章个人总结</a>

* 用git write-tree可以从索引中写出一颗树，这棵树其实是根目录的SHA1值，至于索引是什么，下章会介绍；

* find .git/objects可以查看到所有git库中的bolb对象的散列值;

* 提交其实就是提交树和一些作者信息，因为树可以包含树，如果树包含的内容的散列值未变化，git可以依据此值不改变blob对象;

* 使用SHA1值区分不同的文件版本，是一个非常不错的策略，思考一下如果不使用这个策略，让我们自己设计git，我们会如何做?

* 对标签的简单理解就是：给某次提交命一个名，并且同时生成一个tag对象；

* 一些重要命令和选项：git ls-files -s,find,git cat-file -p


## <a id='5' href='#c5'>第5章 文件索引和管理</a>

**NOTE:在<a href="#4.1.3">4.1.3</a>中我们知道索引用来描述整个目录结构。**

* 原文

如果你的项目处于版本控制系统的管理下，你就可以在工作目录里编辑，然后把修改提交给版本库来保管。Git的工作原理与之类似，
但是它在工作目录和版本库之间加设了一层索引（index），用来暂存（stage）、收集或者修改。当你使用Git来管理代码时，你会在工作目录下编辑，
在索引中积累修改，然后把索引中累积的修改作为一次性的变更来进行提交。

你可以把Git的索引看作一组打算的或预期的修改。这就意味着，可以在最终提交前添加、删除、移动或者重复编辑文件，
只有在提交后才会在版本库里实现积累的变更。而大多数重要的工作其实是在提交步骤之前完成的。

* 提示

**请记住，一次提交其实是个两步的过程：暂存变更和提交变更。** 在工作目录下而不在索引中的变更是没暂存的，因此也不会提交。


为方便起见，当添加或更改文件的时候，Git允许把两步合并成一步：
```text
$ git commit index.html
```
但是，如果要移动或者删除文件，就没那么简单了。这两步必须分开做：
```text
$ git rm index.html

$ git commit

```

本章将要介绍如何管理索引和文件。描述如何在版本库中添加和删除文件，如何重命名文件，以及如何登记索引文件的状态。
本章最后将介绍如何让Git忽略临时文件和其他不需要被版本控制追踪的无关文件。

### <a id='5.1' href='#c5.1'>5.1 关于索引的一切</a>

* 原文

Linus Torvalds在Git邮件列表里曾说如果不先了解索引的目的，你就不能完全领会Git的强大之处。

Git的索引不包含任何文件内容，它仅仅追踪你想要提交的那些内容。当执行git commit命令的时候，Git会通过检查索引而不是工作目录来找到提交的内容
（提交将在第6章具体介绍）。

虽然许多Git的“porcelain”（高层）命令对你隐藏了索引的细节而让你的工作更容易，但记住索引和它的状态还是很重要的。

在任何时候都可通过git status命令来查询索引的状态。它会明确展示出哪些文件Git看来是暂存的。也可以通过一些底层命令来窥视Git的内部状态，
例如git ls-files。

在暂存过程中，你会发现git diff命令是十分有用的（第8章将深入讨论diff）。这条命令可以显示两组不同的差异：
git diff显示仍留在工作目录中且未暂存的变更；git diff --cached显示已经暂存并且因此要有助于下次提交的变更。

可以用git diff的这两种形式引导你完成暂存变更的过程。最初，git diff显示所有修改的大集合，--cached则是空的。而当暂存时，前者的集合会收缩，
后者会增大。如果所有修改都暂存了并准备提交，--cached将是满的，而git diff则什么都不显示。

### <a id='5.2' href='#c5.2'>5.2 Git中的文件分类</a>

Git将所有文件分成3类：已追踪的、被忽略的以及未追踪的。

* 已追踪的（Tracked）
已追踪的文件是指已经在版本库中的文件，或者是已暂存到索引中的文件。如果想将新文件somefile 添加为已追踪的文件，执行git add somefile 。

* 被忽略的（Ignored）
被忽略的文件必须在版本库中被明确声明为不可见或被忽略，即使它可能会在你的工作目录中出现。一个软件项目通常都会有很多被忽略的文件。
普通被忽略的文件包括临时文件、个人笔记、编译器输出文件以及构建过程中自动生成的大多数文件等。Git维护一个默认忽略文件列表，
也可以配置版本库来识别其他文件。被忽略的文件将会在本章后面详细讨论（见5.8节）。

* 未追踪的（Untracked）
未追踪的文件是指那些不在前两类中的文件。Git把工作目录下的所有文件当成一个集合，减去已追踪的文件和被忽略的文件，剩下的部分作为未追踪的文件。

让我们通过创建一个全新的工作目录和版本库并处理一些文件来探讨这些不同类别的文件。

```text

$ cd /tmp/my_stuff

$ git init

$ git status

# On branch master
#
# Initial commit
#
nothing to commit (create/copy files and use "git add" to track)

$ echo "New data" > data

$ git status
# On branch master
#
# Initial commit
#
# Untracked files:
#　 (use "git add <file>..." to include in what will be committed)
#
#　　　data
nothing added to commit but untracked files present (use "git add" to track)

```



最初，目录里没有文件，已追踪的文件和被忽略的文件都是空的，因此未追踪的文件也是空的。
一旦创建了一个data 文件，git status就会报告一个未追踪的文件。

编辑器和构建环境常常会在源码文件周围遗留一些临时文件。在版本库中这些文件通常是不应被当作源文件追踪的。而为了让Git忽略目录中的文件，
只需要将该文件名添加到一个特殊的文件.gitignore 中就可以了。
```text

# 手动创建一个垃圾文件
$ touch main.o

$ git status

# On branch master
#
# Initial commit
#
# Untracked files:
#　 (use "git add <file>..." to include in what will be committed)
#
#　　　 data
#　　　 main.o

$ echo main.o > .gitignore

$ git status
# On branch master
#
# Initial commit
#
# Untracked files:
#　 (use "git add <file>..." to include in what will be committed)
#
#　　　.gitignore
#　　　data
```


这样main.o 已经被忽略了，但是git status现在显示一个新的未追踪的文件.gitignore 。
虽然.gitignore 文件对Git有特殊的意义，但是它和版本库中任何其他普通文件都是同样管理的。
除非把.gitignore 添加到索引中，否则Git仍会把它当成未追踪的文件。

接下来的几节展示不同的方式来改变文件的追踪状态，以及如何添加或从索引中删除它。

### <a href='#c5.3' id='5.3'>5.3 使用git add</a>

git add命令将**暂存**一个文件。就Git文件分类而言，如果一个文件是未追踪的，那么git add就会将文件的状态转化成已追踪的。
如果git add作用于一个目录名，那么该目录下的文件和子目录都会递归暂存起来。

```text
NOTE:关于暂存,这里停顿思考一下。根据前面介绍，当commit的时候，其实是做了两个动作，先暂存再提交。那么，暂存到底是干了什么呢？
当我们修改了一个文件，不使用add直接commit的时候，git会告诉我们Changes not staged for commit，
所以我暂且认为暂存是将工作区的内容和git仓库某个临时的地方同步，然后commit是把这个临时地方的内容和版本库正式内容同步。

```

让我们继续上一节的例子。

```text
$ git status

# On branch master
#
# Initial commit
#
# Untracked files:
#　 (use "git add <file>..." to include in what will be committed)
#
#　　 .gitignore
#　　 data

# Track both new files.

$ git add data .gitignore

$ git status

# On branch master
#
# Initial commit
#
# Changes to be committed:
#　 (use "git rm --cached <file>..." to unstage)
#
#　　 new file: .gitignore
#　　 new file: data
#
```

第一条git status命令显示有两个未追踪的文件，并提醒你要追踪一个文件，只需要使用git add就可以了。
使用git add之后，暂存和追踪data和.gitignore文件，并准备在下次提交的时候加到版本库中。

在Git的对象模型方面，在发出git add命令时每个文件的全部内容都将被复制到对象库中，并且按文件的SHA1名来索引。
暂存一个文件也称作缓存（caching）一个文件 ② ，或者叫“把文件放进索引”。

```text
NOTE:前面我所说的"某个临时的地方",其实就是对象库中的objects，并给了一个SHA1名。我们知道一个SHA1值的背后代表一个blob对象，
就是这个暂存的文件。所以，暂存就是把我们工作区的各个文件计算SHA1并保存进git仓库，但并未放到最终要放的地方，而commit则会把
暂存的文件放到最终的地方。我期待在学习commit的时候知晓这个最终的地方是哪里。
```

可以使用git ls-files命令查看隐藏在对象模型下的东西，并且可以找到那些暂存文件的SHA1值。

```text
$ git ls-files --stage
100644 0487f44090ad950f61955271cf0a2d6c6a83ad9a 0　　　 .gitignore
100644 534469f67ae5ce72a7a274faf30dee3c2ea1746d 0　　　 data
```
**NOTE:当你多次提交，比如git commit --all 以后，再使用git ls-files --stage查看，发现暂存过的文件都能查看得到，
它们都保留在暂存区(不知道有没有暂存区这个概念，如果没有就当是我发明的概念)里。**

版本库中大多数的日常变化可能只是简单的编辑。在任何编辑之后，提交变更之前，请执行git add命令，用最新版本的文件去更新索引。
如果不这么做，你将会得到两个不同版本的文件：一个是在对象库里被捕获并被索引引用的，另一个则在你的工作目录下。

**NOTE:到目前为止，其实我还是不知道"索引"到底是个什么具体的东西。根据前面的知识，可以根据索引生成树(git write-tree),
然后，如果文件改变了，可以使用git add更新索引，是不是可以认为索引是记录最新版本的一个东西呢？**

继续上面的例子，让我们改变data文件，使之有别于索引中的那个文件，然后使用一条神秘的命令**git hash-object file** （你几乎不会直接调用它）
来直接计算和输出这个新版本的SHA1散列值。

```text
$ git ls-files --stage
100644 0487f44090ad950f61955271cf0a2d6c6a83ad9a 0　　　 .gitignore
100644 534469f67ae5ce72a7a274faf30dee3c2ea1746d 0　　　 data

# 编辑"data"来包含...
$ cat data
New data
And some more data now

$ git hash-object data
e476983f39f6e4f453f0fe4a859410f63b58b500

```


在略做修改之后就会发现，保存在对象库和索引中的那个文件的上一个版本的SHA1值是534469f67ae5ce72a7a274faf30dee3c2ea1746d。然而，
文件更新之后版本的SHA1值则是e476983f39f6e4f453f0fe4a859410f63b58b500。接下来，更新索引，使之包含文件的最新版本。

```text
$ git add data

$ git ls-files --stage
100644 0487f44090ad950f61955271cf0a2d6c6a83ad9a 0　　　 .gitignore
100644 e476983f39f6e4f453f0fe4a859410f63b58b500 0　　　 data
```



现在索引有了更新后的文件版本。也就是说，“文件已经暂存了”，或者简单来说，“data文件在索引中”。后一种说法不是很准确，
因为实际上文件存储在对象库中，索引只是指向它而已。

看似无用地处理SHA1散列值和索引却带来一个关键点：与其把git add看成“添加这个文件”，不如看作“添加这个内容”。

在任何情况下，最重要的事是要记住工作目录下的文件版本和索引中暂存的文件版本可能是不同步的。当提交的时候，Git会使用索引中的文件版本。

**NOTE:作者上面这句话有点含混不清，"当提交的时候，Git会使用索引中的文件版本",我已经知道，commit的时候会强制你先add,add以后工作目录和索引
便同步了。**

```text
提示

对于git add或git commit而言，--interactive选项都会是探索哪个文件将为提交而暂存很有用的方式。
```

### <a href='#c5.4' id='5.4'>5.4 使用git commit的一些注意事项</a>


#### <a href='#c5.4.1' id='5.4.1'>5.4.1 使用git commit --all</a>

git commit的-a或者-all选项会导致执行提交之前自动暂存所有未暂存的和未追踪的文件变化，包括从工作副本中删除已追踪的文件。

下面通过创建一些有不同暂存特征的文件来看看它是怎么工作的。
```text

# 建立测试版本库
$ mkdir /tmp/commit-all-example




$ cd /tmp/commit-all-example




$ git init




Initialized empty Git repository in /tmp/commit-all-example/.git/

$ echo something >> ready




$ echo somthing else >> notyet




$ git add ready notyet




$ git commit -m "Setup"




[master (root-commit) 71774a1] Setup
 2 files changed, 2 insertions(+), 0 deletions(-)
 create mode 100644 notyet
 create mode 100644 ready

# 修改ready文件并用"git add"把它添加到索引中
# 编辑ready
$ git add ready





# 修改notyet文件，保持它是未暂存的
# 编辑notyet

# 在一个子目录里添加一个新文件，但不要对它执行add命令
$ mkdir subdir




$ echo Nope >> subdir/new

```

使用git status命令来看看一个常规提交（不带命令行参数）会做什么事情。

```text
$ git status
# On branch master
# Changes to be committed:
#　 (use "git reset HEAD <file>..." to unstage)
#
#　　　modified: ready
#
# Changed but not updated:
#　 (use "git add <file>..." to update what will be committed)
#
#　　　modified: notyet
#
# Untracked files:
#　 (use "git add <file>..." to include in what will be committed)
#
#　　　subdir/

```




这里，索引准备提交ready 文件，因为只有它暂存了。

但是，如果执行git commit --all命令，Git会递归遍历整个版本库，暂存所有已知的和修改的文件，然后提交它们。在这种情况下，
当编辑器展示出提交消息模板的时候，它应该指明被修改的和已知的notyet 文件事实上也会提交。

```text
# Please enter the commit message for your changes.
# (Comment lines starting with '#' will not be included)
# On branch master
# Changes to be committed:
#　 (use "git reset HEAD <file>..." to unstage)
#
#　　　modified: notyet
#　　　modified: ready
#
# Untracked files:
#　 (use "git add <file>..." to include in what will be committed)
#
#　　　subdir/
```

最后，由于subdir /是一个全新的目录，而且该目录下没有任何文件名或路径是已追踪的，所以，即使是-all选项也不能将其提交。
```text

Created commit db7de5f: Some --all thing.
 2 files changed, 2 insertions(+), 0 deletions(-)
```



虽然Git会递归遍历整个版本库，查找修改的和删除的文件，但是全新的文件目录subdir /及其中所有文件还是不会成为提交的一部分 ③ 。

**NOTE:简单说就是：git commit --all会暂存和提交所有已追踪的文件，未追踪的不管。**

#### <a href='#c5.4.2' id='5.4.2'>5.4.2 编写提交日志消息</a>

如果不通过命令行直接提供日志消息，Git会启动编辑器，并提示你写一个。编辑器的选取根据配置文件中的设定，具体描述请见3.3节。

如果你是在编辑器中编写提交日志消息，并出于某种原因，决定中止此次操作，只要不保存退出编辑器即可；这将导致一条空日志消息。
如果那太迟了，因为你已经保存了，那只要删除整条日志消息，然后重新保存就可以了。Git不会处理空（无文本）提交。

### <a href='#c5.5' id='5.5'>5.5 使用git rm</a>

git rm命令自然是与git add相反的命令。它会在版本库和工作目录中同时删除文件。然而，由于删除文件比添加文件问题更多（如果出现错误），
Git对移除文件更多一点关注。

Git可以从索引或者同时从索引和工作目录中删除一个文件。Git不会只从工作目录中删除一个文件，普通的rm命令可用于这一目的。

从工作目录和索引中删除一个文件，并不会删除该文件在版本库中的历史记录。文件的任何版本，只要是提交到版本库的历史记录的一部分，
就会留在对象库里并保存历史记录。

继续这个例子，引进一个不应该暂存的“意外”文件，看看怎么将其删除。

```text

$ echo "Random stuff" > oops





# 无法对Git认为是"other"的文件执行 "git rm"
# 应该只使用 "rm oops"
$ git rm oops




fatal: pathspec 'oops' did not match any files


```


因为git rm也是一条对索引进行操作的命令，所以它对没有添加到版本库或索引中的文件是不起作用的；Git必须先认识到文件才行。
所以下面偶然地暂存oops 文件。
```text

# 意外暂存"oops"文件
$ git add oops





$ git status




# On branch master
#
# Initial commit
#
# Changes to be committed:
#　 (use "git rm --cached <file>..." to unstage)
#
#　　　new file: .gitignore
#　　　new file: data
#　　　new file: oops
#


```


**另外，要将一个文件由已暂存的转化成未暂存的，可以使用git rm --cached命令。**

```text

$ git ls-files --stage
100644 0487f44090ad950f61955271cf0a2d6c6a83ad9a 0　　　.gitignore
100644 e476983f39f6e4f453f0fe4a859410f63b58b500 0　　　data
100644 fcd87b055f261557434fa9956e6ce29433a5cd1c 0　　　oops

$ git rm --cached oops
rm 'oops'

$ git ls-files --stage
100644 0487f44090ad950f61955271cf0a2d6c6a83ad9a 0　　　.gitignore
100644 e476983f39f6e4f453f0fe4a859410f63b58b500 0　　　data

```

**git rm --cached会删除索引中的文件并把它保留工作目录中，而git rm则会将文件从索引和工作目录中都删除。**

```text
警告

使用git rm --cached会把文件标记为未追踪的，却在工作目录下仍留有一份副本，这是很危险的。因为你也许会忘记这个文件是不再被追踪的。
Git要检查工作文件的内容是最新的，使用这种方法则无视了这个检查。所以要谨慎使用。
```


如果想要移除一个已提交的文件，通过简单的git rm filename 命令来暂存这一请求。

```text

$ git commit -m "Add some files"




Created initial commit 5b22108: Add some files
 2 files changed, 3 insertions(+), 0 deletions(-)
 create mode 100644 .gitignore
 create mode 100644 data

$ git rm data




rm 'data'

$ git status




# On branch master
# Changes to be committed:
#　 (use "git reset HEAD <file>..." to unstage)
#
#　　　deleted: data
#
```

Git在删除一个文件之前，它会先进行检查以确保工作目录下该文件的版本与当前分支中的最新版本（Git命令调用HEAD的版本）是匹配的。
这个验证会防止文件的修改（由于你的编辑）意外丢失。

**NOTE:怎么理解前面这句话？大概是这样子的：我修改了一个文件b.txt，然后觉得应该删除它，我使用git rm b.txt删除:**
```text
$ git rm b.txt
error: the following file has local modifications:
    b.txt
(use --cached to keep the file, or -f to force removal)
```
喔，错误！文件被修改！它给出了两个方法：use --cached to keep the file, or -f to force removal.
```text
git rm b.txt --cached
rm 'b.txt'
```
文件还在工作区，但变成了未追踪状态。重新add它，然后编辑一下，再如下操作：
```text
$ git rm b.txt -f
rm 'b.txt'

```
现在b.txt已经从工作区也消失了。

```text

提示

还可以使用git rm -f来强制删除文件。强制就是明确授权，即使从上次提交以来你已经修改了该文件，还是会删除它。
```

万一你真的想保留那个不小心删除的文件，只要再把它添加回来就行了。
**NOTE:前面这句话指的是使用--cached选项删除，如果使用-f删除是不能恢复了,因为它从工作区消失了。**

```text

$ git add data
fatal: pathspec 'data' did not match any files

```


Git把工作目录下的文件也删除了。不过不用担心。版本控制系统擅长恢复文件的旧版本。

```text

$ git checkout HEAD -- data

$ cat data
New data
And some more data now

$ git status

# On branch master
nothing to commit (working directory clean)

```
**NOTE:我自己的测试：**
```text
$ git checkout HEAD -- b.txt
```
文件真的恢复了，在我前面的操作中，我在b.txt里面新加了一些文字，然后使用git rm -f删除了它，恢复后它变成了我编辑前的样子，添加的文字没有出现，
也就是说git rm -f执行的时候是不会给新内容建立索引的。

**NOTE:到现在为止，虽然我也像作者一样使用"索引"这个词，但我还是不知道索引具体是什么。**

### <a href='#c5.6' id='5.6'>5.6 使用git mv</a>

假设你需要移动或者重命名文件。可以对旧文件使用git rm命令，然后用git add命令添加新文件，或者可以直接使用git mv命令。给定一个版本库，
其中有一个stuff 文件，你想要将它重命名为newstuff 。下面的一系列命令就是等价的Git操作。

```text
$ mv stuff newstuff
$ git rm stuff
$ git add newstuff
```
和
```text
$ git mv stuff newstuff
```

无论哪种情况，Git都会在索引中删除stuff 的路径名，并添加newstuff 的路径名，至于stuff 的原始内容，则仍保存在对象库中，
然后才会将它与newstuff 重新关联。

在示例版本库中找回了data这个文件，下面重命名它，然后提交变更。
```text
$ git mv data mydata

$ git status
# On branch master
# Changes to be committed:
#　 (use "git reset HEAD <file>..." to unstage)
#
#　　　renamed: data -> mydata
#

$ git commit -m "Moved data to mydata"
Created commit ec7d888: Moved data to mydata
 1 files changed, 0 insertions(+), 0 deletions(-)
 rename data => mydata (100%)
```


如果你碰巧检查这个文件的历史记录，你可能会不安地看到Git很明显丢失了原始data 文件的历史记录，只记得它从data 重命名为当前文件名。

```text
$ git log mydata
commit ec7d888b6492370a8ef43f56162a2a4686aea3b4
Author: Jon Loeliger <jdl@example.com>
Date:　 Sun Nov 2 19:01:20 2008 -0600

Moved data to mydata

```

Git其实是记得全部历史记录的，但是显示要限制于在命令中指定的文件名。--follow选项会让Git在日志中回溯并找到内容相关联的整个历史记录。

```text
$ git log --follow mydata
commit ec7d888b6492370a8ef43f56162a2a4686aea3b4
Author: Jon Loeliger <jdl@example.com>
Date:　 Sun Nov 2 19:01:20 2008 -0600

Moved data to mydata

commit 5b22108820b6638a86bf57145a136f3a7ab71818
Author: Jon Loeliger <jdl@example.com>
Date:　 Sun Nov 2 18:38:28 2008 -0600

Add some files
```
**NOTE:git log不带选项的话，是显示提交历史列表。这里展示了git log另外的用法，可以带上文件名,还可以带上--follow选项。**

VCS的经典问题之一就是文件重命名会导致它们丢失对文件历史记录的追踪。而Git即使经历过重命名，也仍然能保留此信息。

### <a href='#c5.7' id='5.7'>5.7 追踪重命名注解</a>
下面详细讨论关于Git是如何追踪文件重命名。

作为传统版本控制系统的典型，SVN对文件重命名和移动做了很多追踪工作。为什么呢？这是由于它只追踪文件之间的差异才导致的。例如，如果移动一个文件，
这本质上就相当于从旧文件中删除所有行，然后把它们添加到新的文件中。但是任何时侯，你哪怕就做一个简单的重命名，
也需要再次传输和存储文件的全部内容，这将变得非常低效；想象一下重命名一个拥有数以千记的文件的子目录，那该是多可怕的事情。

为缓解这种情况，SVN显式追踪每一次重命名。如果你想将hello.txt 重命名为subdir/hello.txt ，你必须对文件使用svn mv，
而不能使用svn rm和svn add。否则，SVN将不能识别出这是一个重命名，只能像刚才描述的那样进行低效的删除/添加步骤。

接着，要有追踪重命名这个特殊功能，SVN服务器需要一个特殊协议来告诉它的客户端，“请将hello.txt 移动到subdir/hello.txt ”。此外，
每一个SVN客户端必须确保该操作（相对罕见）执行的正确性。

另一方面，Git则不追踪重命名。可以将hello.txt 移动或复制到任何地方，这么做只会影响树对象而已（但请记住，树对象保存内容间的关系，
而内容本身保存在blob中）。查看两棵树间的差异，我们可以很容易发现叫3b18e5...的blob已经移动到一个新地方。而且即使你没有明确检查差异，
系统中的每个部分都知道它已经有了那个blob，不再需要它的另一个副本了。

在这种情况下，像在很多其他地方一样，Git基于散列的简单存储系统简化了许多其他RCS被难倒的或者选择回避的事情。
```text
重命名追踪的困难

版本控制系统的开发人员间常年争论追踪文件重命名问题。

一次简单的重命名也足以产生一次争吵。当文件名改变之后，内容也改变了，这时大家的争论更加白热化了。
然后这个情景的讨论就由实用上升到哲学层面：“新”文件单纯只是一次重命名，还是它与旧文件仅仅相似而已？
在把它们定义为相同的文件之前，新文件和原来文件到底有多相似？如果你应用某人的补丁，删除一个文件，
然后在其他地方再创建一个相似的文件，这又是如何管理的呢？如果在不同分支中对同一个文件进行不同方式的重命名，会发生什么呢？
在这种情况下，是选择像Git一样自动检测重命名发生的错误少，还是像SVN那样要求用户显式标识重命名的错误少呢？

在现实生活的使用中，似乎Git的系统处理文件重命名的方式更优越一点，因为有太多的方式去重命名一个文件，
而人类的聪明程度不够以确保让SVN知道所有情况。但是还没有能完美处理文件重命名的系统。
```
### <a href='#c5.8' id='5.8'>5.8 .gitignore文件</a>

在本章前面，你已经看到如何通过.gitignore 文件来忽略不相干的main.o 文件。在那个例子里，可以忽略任何文件，
只要将想要忽略的文件的文件名加到同一目录下的.gitignore 中即可。此外，可以通过将文件名添加到该版本库顶层目录下的.gitignore 文件中来忽略它。

但是Git还支持一种更为丰富的机制。一个.gitignore 文件下可以包含一个文件名模式列表，指定哪些文件要忽略。.gitignore 文件的格式如下。

* 空行会被忽略，而以井号（#）开头的行可以用于注释。然而，如果#跟在其他文本后面，它就不表示注释了。
* 一个简单的字面置文件名匹配任何目录中的同名文件。
* 目录名由末尾的反斜线（/）标记。这能匹配同名的目录和子目录，但不匹配文件或符号链接。
* 包含shell通配符，如星号（*），这种模式可扩展为shell通配模式。正如标准shell通配符一样，因为不能跨目录匹配，
所以一个星号只能匹配一个文件或目录名。但对于那些通过斜线来指定目录名的模式（例如，debug/32bit/­*.o ），星号仍可以成为其中一部分。
* 起始的感叹号（!）会对该行其余部分的模式进行取反。此外，被之前模式排除但被取反规则匹配的文件是要包含的。取反模式会覆盖低优先级的规则。

此外，Git允许在版本库中任何目录下有.gitignore 文件。每个文件都只影响该目录及其所有子目录。.gitignore 的规则也是级联的：
可以覆盖高层目录中的规则，只要在其子目录包含一个取反模式（使用起始的“!”）。

为了解决带多个.gitignore 目录的层次结构问题，也为了允许命令行对忽略文件列表的增编，Git按照下列从高到低的优先顺序：

* 在命令行上指定的模式；
* 从相同目录的.gitignore 文件中读取的模式；
* 上层目录中的模式，向上进行。因此，当前目录的模式能推翻上层目录的模式，而最接近当前目录的上层目录的模式优先于更上层的目录的模式；
* 来自.git/info/exclude 文件的模式；
* 来自配置变量core.excludedfile指定的文件中的模式。

因为在版本库中.gitignore 文件被视为普通文件，所以在复制操作过程中它会被复制，并适用于你的版本库的所有副本。一般情况下，
只有当模式普遍适用于所有派生的版本库时，才应该把条目放进版本控制下的.gitignore 文件中。

如果排除模式某种程度上特定于你的版本库，并且不应该（或可能不）适用于其他人复制的版本库，那么这个模式应该放到.git/info/exclude 文件里，
因为它在复制操作期间不会传播。它的模式的格式和适用对象与.gitignore 文件是一样的。

下面是另一种情景，排除.o 文件（编译器从源码生成的）是很典型的。为了忽略.o 文件，要将*.o 添加到顶层的.gitignore 文件中。但是，
如果有一个特定的*.o 文件是由其他人提供的，你不能自己生成一个替代，那该怎么办？你很可能会想明确追踪那个特定的文件。然后，你就可能要这样的配置。

```text

$ cd my_package

$ cat .gitignore
*.o

$ cd my_package/vendor_files
$ cat .gitignore
!driver.o

```



这种规则的组合意味着Git会忽略版本库中所有.o 文件，但是会追踪一个例外，即在vendor_files 子目录下的driver.o 文件。

### <a href='#c5.9' id='5.9'>5.9 Git中对象模型和文件的详细视图</a>

到现在为止，你应该已经具备管理文件的基本能力。尽管如此，在哪里跟踪什么文件——在工作目录、索引还是版本库中——还是挺令人困惑的。
让我们跟随该系列的4幅图来可视化一个叫file1 的文件从编辑到在索引中暂存，再到最终提交的整个过程，加深我们对文件管理的理解。
下面的每一幅图都会同时显示你的工作目录、索引以及对象库。为了简单起见，让我们只看master分支。

初始状态如图5-1所示。在这里，工作目录包含file1 和file2 两个文件，分别包含内容“foo”和“bar,”。
![](https://github.com/YuxingXie/git_study/raw/master/assets/image/05-09-01.jpg) 
图5-1　初始文件和对象

除了工作目录下的file1 和file2 之外，master分支还有一个提交，它记录了跟file1和file2内容完全一样的“foo”和“bar,”的树。此外，
该索引记录两个SHA1值a23bf和9d3a2，与那两个文件分别对应。工作目录、索引以及对象库都是同步和一致的。没有什么是脏的。

图5-2显示了在工作目录中对file1 编辑后的变化，现在它的内容包含“quux.”。索引和对象库中没有变化，但是工作目录现在是脏的。
![](https://github.com/YuxingXie/git_study/raw/master/assets/image/05-09-02.jpg) 

图5-2　编辑file1之后

当使用git add file1来暂存file1 的编辑时，一些有趣的变化发生了。

如图5-3所示，Git首先取出工作目录中file1 的版本，为它的内容计算一个SHA1的散列ID（bd71363），然后把那个ID保存在对象库中。接下来，
Git就会记录在**索引中的file1路径名**已更新为新的bd71363的SHA1值。


![](https://github.com/YuxingXie/git_study/raw/master/assets/image/05-09-03.jpg) 

图5-3　在git add之后

由于file2 的内容未发生改变而且没有任何git add来暂存file2 ，因此索引继续指向原始blob对象。

此时，你已经在索引中暂存了file1 文件，而且工作目录和索引是一致的。不过，就HEAD而言，索引是脏的，
因为索引中的树跟在master分支的HEAD提交的树在对象库里是不一样的 ④ 。

最后，当所有变更都暂存到索引中后，一个提交将它们应用到版本库中。git commit的作用如图5-4所示。

![](https://github.com/YuxingXie/git_study/raw/master/assets/image/05-09-04.jpg) 
图5-4　在git commit之后

如图5-4所示，提交启动了三个步骤。首先，虚拟树对象（即索引）在转换成一个真实的树对象后，会以SHA1命名，然后放到对象库中。其次，
用你的日志消息创建一个新的提交对象。新的提交将会指向新创建的树对象以及前一个或父提交。最后，
master分支的引用从最近一次提交移动到新创建的提交对象，成为新的master HEAD。

一个有趣的细节是，工作目录、索引和对象库（由master分支的HEAD表示）再次同步，变得一致了，就如同它们在图5-1中一样。

**NOTE:这一节内容看着不多，但是包含超多信息。现在可以理解"索引"是什么了，从add到commit发生了什么。另外，还引入了"分支"的概念，
以及熟悉的HEAD master一些分支相关的词汇，它们都是和commit密切相关的概念。**


*① 　我有确实可靠的证据证明，本章实际的标题应该是“Bart Massey讨厌Git的地方”。——原注*

*② 　你肯定在git status命令的输出里看到--cached了，对吧？——原注*

*③ 　要包括subdir及其中所有文件，可以先执行git add.，然后执行commit-a。——译者注*

*④ 　无论工作目录的状态，都可以在其他方向上得到脏的索引。将一个非HEAD提交从对象库中读取出来并放进索引中，但不把相应的文件检出到工作目录中，
那么你就制造出这样一种情况：索引和工作目录不一致，就HEAD而言，索引仍是脏的。——原注*

## <a id='6' href='#c6'>第6章 提交</a>

在Git中，提交（commit）是用来记录版本库的变更的。

从表面看来，Git的提索引中的file1 路径名交和其他VCS的提交或检入没什么不同。但Git是在背后以一种独特的方式来执行提交的。

当提交时，Git会记录索引的快照并把快照放进对象库（为提交准备索引在第5章讲述）。这个快照不包含该索引中任何文件或目录的副本，
因为这样的策略会需要巨大的存储空间。Git会将当前索引的状态与之前的快照做一个比较，并派生出一个受影响的文件和目录列表。
Git会为任何有变化的文件创建新blob对象，对有变化的目录创建新的树对象，对于未改动的文件和目录则会沿用之前的blob与树对象。

提交的快照是串联在一起的，每张新的快照指向它的先驱。随着时间的推移，一系列变更就表示为一系列提交。

**NOTE:虽然现在还不知道索引长什么样，但是我们可以知道，根据索引可以知道现在暂存的文件是哪些版本，并可以根据git write-tree还原出来。
也就是作者前面刚刚说的，索引是一些提交列快照中最新的那一个。**

看起来将整个索引与之前某个状态的索引相比较的开销是比较大的，但整个过程是非常快的，因为每个Git对象都有一个SHA1散列值。
如果两个对象甚至两棵子树拥有相同的SHA1散列值，那么它们就是相同的。Git可以通过修剪有相同内容的子树来避免大量的递归比较。

**NOTE:比较两棵树的所有枝节，根据每个枝节(一个枝节也是一个树)的SHA1值，如果相同就可以不用再继续比较，如果不同就继续比较，直到找出所有的
不同点，这在逻辑上没问题。**

版本库中的变更和提交之间是一一对应的关系：**提交是将变更引入版本库的唯一方法**，任何版本库中的变更都必须由一个提交引入。此项授权提供了问责制。
任何情况下都不会出现版本库有数据变动而没有记录！试想一下，如果主版本库中的内容不知何故发生了变化，又没有任何记录记载这一切是如何发生的、
谁干的，甚至是什么原因，那将是多么混乱啊。

**NOTE:既然提交是将变更引入版本库的唯一方法,那么add就并没有将变更引入版本库，add只是暂存，虽然它改变了当前的索引，但分支的内容没有变化。
所以要理解作者口中的版本库，它依赖于分支。**

虽然最常见的提交情况是由开发人员引入的，但是Git自身也会引入提交。正如你将会在第9章看到的那样，**除了用户在合并之前做的提交外，
合并操作自身会导致在版本库中多出一个提交**。



你选择何时提交更多取决于你的喜好或开发风格。一般来说，你应该在明确的时间点提交，也就是当你的开发处于静态阶段时，比如一个测试套件通过时，
每天回家的时候，或者任何其他时间点。

但是，对于提交不要有任何负担！Git非常适合频繁的提交，并且它还提供了丰富的命令集来操作这些提交。接下来，
你将看到几个提交——包含清晰且定义良好的变更——也可以导致更好的组织变化和更易操作的补丁集。

**NOTE:基于经验，多提交会避免很多冲突产生，所以我经常鼓励我们公司的程序员多提交，然而不知道什么原因，或者是我的说服力不够，
大家对提交似乎有某种心理障碍。**

### <a href='#c6.1' id='6.1'>6.1 原子变更集</a>

每一个Git提交都代表一个相对于之前的状态的单个原子变更集。对于一个提交中所有做过的改动 ① ，
无论多少目录、文件、行、字节的改变，**要么全部应用，要么全部拒绝**。

在底层对象模型方面，原子性是有意义的：一张提交快照代表所有文件和目录的变更，它代表一棵树的状态，
而两张提交快照之间的变更集就代表一个完整的树到树的转换（你可以阅读第8章中有关提交之间的衍生差异来了解更多细节）。

考虑把一个函数从一个文件移动到另一个文件的流程。假设你在第一次提交中删除了某函数，并在紧接着的提交中把该函数加回来(note:并提交?)。
那么在函数被删除期间版本库的这段历史记录中，就会出现一个小小的语义鸿沟（semantic gap）。调换这两次提交的顺序也是有问题的。在这两种情况下，
第一次提交之前和第二次提交之后，代码在语义上都是一致的，而在第一次提交过后的代码则是错误的。

然而，使用原子提交同时添加和删除该函数，就不会有语义鸿沟出现在历史记录中。可以在第10章中学习到如何更好地构建和组织提交。

**NOTE:作者意思是不要让错误代码commit到版本库吗？**

Git不关心文件为什么变化。即变更的内容并不重要。作为开发人员，可以将一个函数从这里移动到那里，并期望这算一次移动。
但是也可以先提交删除再提交添加。Git对此并不关心，因为它丝毫不在乎文件的语义。

但这揭示了Git实现原子性操作的关键原因之一：它允许你根据一些最佳实践建议来设计你的提交。

最后，你可以放心Git一直没有把你的版本库置于两次提交之间的过渡状态
(**note**:因为你的版本库，即分支，它一定指向某次提交,无论怎么修改，甚至add都不会改变，直到再次commit)。

### <a href='#c6.2' id='6.2'>6.2 识别提交</a>

无论你是独自编码还是在团队中工作，识别个人的提交都是一个很重要的任务。例如，**当创建新分支时，必须要选择某个提交来作为分支点**；
当比较代码差异时，必须要指定两个提交；当编辑提交历史记录时，必须提供一个提交集。在Git中，可以通过显示或隐式引用来指代每一个提交。

你应该已经见过了一些显示引用和隐式引用。唯一的40位十六进制SHA1提交ID是显式引用。而**始终指向最新提交的HEAD则是隐式引用**。
尽管有时两种引用都不方便，但是幸运的是，Git提供了许多不同的机制来为提交命名，这些机制有各自的优势，需要根据上下文来选择。

**NOTE:HEAD可以认为是一系列提交快照中最新的那一个。**

例如，**在分布式环境中，当你要与同事讨论相同数据的提交时，最好使用两个版本库中相同的提交名**。另一方面，如果你在自己的版本库上工作，
当你需要查找一个分支几次提交之前的状态时，有一个简单相关的名字足矣。

**NOTE:有的时候，确实会出现两个人都改了同一个地方并且做相同修改的情况。**

#### <a href='#c6.2.1' id='6.2.1'>6.2.1 绝对提交名</a>

对提交来说，最严谨的名字应该是它的散列标识符。**散列ID是个绝对名**，这意味着它只能表示唯一确定的一个提交。无论提交处于版本库历史中的任何位置，
哈希ID都对应相同的提交。

每一个提交的散列ID都是全局唯一的，不仅仅是对某个版本库，而且是对任意和所有版本库都是唯一的。例如，
如果一个开发人员在他的版本库有一个特定的提交ID，并且你在自己的版本库中发现了相同的提交ID，那么你就可以确定你们有包含相同内容的相同提交。
此外，因为导致相同提交ID的数据包含整个版本库树的状态和之前提交的状态，所以通过归纳论证，可以得出一个更强的推论：
你可以确定你们讨论的是之前完全相同的开发线，包括提交也是相同的。

由于输入一个40位十六进制的SHA1数字是一项繁琐且容易出错的工作，因此Git允许你使用版本库的对象库中唯一的前缀来缩短这个数字。
下面是来自Git自己的版本库中的一个例子。

```text
$ git log -1 --pretty=oneline HEAD
1fbb58b4153e90eda08c2b022ee32d90729582e6 Merge git://repo.or.cz/git-gui

$ git log -1 --pretty=oneline 1fbb
error: short SHA1 1fbb is ambiguous.
fatal: ambiguous argument '1fbb': unknown revision or path
　　not in the working tree.
Use '--' to separate paths from revisions

$ git log -1 --pretty=oneline 1fbb58
1fbb58b4153e90eda08c2b022ee32d90729582e6 Merge git://repo.or.cz/git-gui
```
虽然标签名并不是全局唯一的，但它会明确的指向一个唯一的提交，这种指向是不会随着时间而改变的（当然，除非你明确地修改它）。

**NOTE:到目前所学为止，我们是不能给自己的提交命个别名什么的，但是可以给个tag。给tag实际产生了一个tag对象，并明确的指向一次提交。**

**NOTE:自己试试,"HEAD -> master"以及"origin/master"表示还不知道表示什么。**
```text
$ git log -5 --pretty=oneline HEAD
6b9e4ad0f6c447011006c6f54b1a29c53ae3e04f (HEAD -> master) clear
f432c3130c595c22792b356836b8d3b718c21cd2 (origin/master) clear
751b1be8abe23ce95b74e264da7f36ac156c930b clear
af64db73cb2fe437b39141a1d3aee5f2fdf6a7cd clear
70d1384fea52a62654dbe842117a7a7082422205 clear

$ git log V1.0 -1
commit 9168c3dbd65dc2b32dfcbcdc87c4b5a8a1f6e63e (tag: V1.0)
Author: yuxingxie <185246042@qq.com>
Date:   Mon Nov 23 14:07:23 2020 +0800

    clear


```

#### <a href='#cafter6.2.2' id='after6.2.2'>补充内容:master,head,origin等概念</a>

**NOTE:作者高估了我的git基础知识，我并不那么理解诸如"origin/master"、"HEAD -> master"等一些符号的含义。
所以我决定新开章节自行研究一下。**

好在stackoverflow上，有人给出了解释，可点击
<a href='https://stackoverflow.com/questions/8196544/what-are-the-git-concepts-of-head-master-origin'
 target='_blank'>这里</a>查看。
 
简书上也有一篇不错的文章，可点<a href='https://www.jianshu.com/p/4219b6f62ce3' target='_blank'>这里</a>查看。

另外我还从中文网络寻找了一些有用的资料，总结如下：

***

1. HEAD:一次提交
 
你的仓库所处的当前提交。大多数时候，HEAD指向你的当前分支的最后一次提交，但事实并非如此。HEAD真正意思是"我的版本库当前(分支)指向的东西"。

一个提交指向的不是任何分支的顶端时，称为“分离头(detached head)”。

HEAD不是最新版本，而是当前版本。通常，它是当前分支的最新修订，但不必如此。

一个版本库是否只有一个HEAD?我猜**应该**是的!并不是每个分支都有自己的HEAD,切换分支以后HEAD换成当前分支的最新提交，
所以HEAD是个相对概念(**NOTE:关于这个结论我并不100%确定**)。

***

2. master: 一个分支名

第一次创建repo时git为您创建的默认分支的名称。在大多数情况下，“master”的意思是“主分支”。
大多数shops(商店?)都要求每个人都使用master, master被认为是版本库的权威视图。
但是发布(release)分支从master中创建来进行发布也是很常见的。本地存储库有自己的主分支，它几乎总是在远程存储库的主分支之后。

master通常是给主分支的一个名称，但是它可以被称为任何其他名称(或者没有主分支)。

***

3. origin: 一个远程仓库

git为主远程存储库提供的默认名称。您的机器有它自己的存储库，您很可能将其推到您和所有同事推到的某个远程git库。
这个远程git库几乎总是称为origin，但也不必如此。

origin通常是主远程仓库的名称,是另一个您可以从其中提取和推入的git库，比如github这样的服务器上的git库。

HEAD是git中的一个正式概念。HEAD总是有明确的含义。master和origin通常是在git中使用的常见的名字，但不必如此。

***

4. origin master:两个概念

代表着两个概念，前面的 origin 代表远程名，后面的 master 代表远程分支名。

***

5. origin/master:远程仓库的master分支

只代表一个概念，即远程分支名，是从远程拉取代码后在本地建立的一份拷贝（因此也有人把它叫作本地分支）。

在下面"HEAD -> master"的研究时可以看到git log master命令会打印"origin/master"。

***

6. origin/HEAD:远程版本库的HEAD(不确定)

是代表origin版本库当前分支的HEAD提交吗？

***

7. HEAD -> master:分支及状态表示法?(不确定)

我在网上找了很久都没找到"HEAD -> master"的含义。根据一些蛛丝马迹，我暂时认为它代表master分支，并且HEAD在master上。

这些证据是这样获得的：
```text
# git log命令实际上可以接上分支名，打印该分支的所有提交
$ git log master
commit 8026f37b7bdf55c5673d0d931a213450d6e2879a (HEAD -> master, origin/master)
...
...
```
根据上面命令的打印，我猜测"HEAD -> master"是想告诉我们，8026f37b7bdf55c5673d0d931a213450d6e2879a这次提交是master分支的HEAD。

在这里"分支"和"提交"两个概念有点含混不清了，期待后面获得清晰的概念。

#### <a href='#c6.2.2' id='6.2.2'>6.2.2 引用和符号引用</a>

引用（ref）是一个SHA1散列值，指向Git对象库中的对象。虽然一个引用可以指向任何Git对象，但是它通常指向提交对象。
符号引用（symbolic reference），或称为symref，间接指向Git对象。它仍然只是一个引用。

本地特性分支名称、远程跟踪分支名称和标签名都是引用。

每一个符号引用都有一个以ref/开始的明确全称，并且都分层存储在版本库的.git/refs/ 目录中。目录中基本上有三种不同的命名空间代表不同的引用：
refs/heads/ref 代表本地分支，refs/remotes/ref 代表远程跟踪分支，refs/tags/ref代表标签（分支会在第7章和第12章进行更详细的讲解）。

例如，一个叫做dev的本地特性分支就是refs/heads/dev的缩写。因为远程追踪分支在refs/remotes/命名空间中，
所以origin/master实际上是refs/remotes/origin/master。最后，标签v2.6.23就是refs/tags/v2.6.23的缩写。

可以使用引用全称或其缩写，但是如果你有一个分支和一个标签使用相同的名字，Git会应用消除二义性的启发式算法，
根据git rev-parse手册上的列表选取第一个匹配项。

```text
.git/ref
.git/refs/ref
.git/refs/tags/ref
.git/refs/heads/ref
.git/refs/remotes/ref
.git/refs/remotes/ref/HEAD
```
第一条规则通常只适用随后讲到的几个引用：HEAD、ORIG_HEAD、FETCH_HEAD、CHERRY_PICK_HEAD和MERGE_HEAD。

**NOTE:根据前面我自己的研究知道，HEAD表示当前分支的最新提交，它虽然有个ID，但用HEAD指代它。
这些常用的对象都可以用叫做"符号引用"的东西来指代它们。**

**NOTE:用本项目试一试。可以看到有点不一样，
我猜应该是git版本差异，因为像.git/refs/ref、.git/refs/heads/ref这种目录结构似乎有点啰嗦，所以git新版本(我的2.23.0)去掉里层的ref目录。**


```text
$ find .git/refs
.git/refs
.git/refs/heads
.git/refs/heads/master
.git/refs/tags
.git/refs/tags/V1.0
.git/refs/remotes
.git/refs/remotes/origin
.git/refs/remotes/origin/master
```
**NOTE:.git/refs目录下有heads、remotes、tags三个目录，可以合理推测一下：**
* heads:存放本地git库的所有分支的HEAD提交的引用
* tags:存放本地git库的所有tag的引用
* remotes：存放远程git库的分支的引用
```text
提示

从技术角度来说，Git的目录名.git这个名字是可以改变的。因此，Git的内部文档都使用变量$GIT_DIR，而不是字面量.git。
```

Git自动维护几个用于特定目的的特殊**符号引用**。这些引用可以在使用提交的任何地方使用。
***
* HEAD

HEAD始终指向当前分支的最近提交。当切换分支时，HEAD会更新为指向新分支的最近提交。
***
* ORIG_HEAD

某些操作，例如合并（merge）和复位（reset），会把调整为新值之前的先前版本的HEAD记录到ORIG_HEAD中。
可以使用ORIG_HEAD来恢复或回滚到之前的状态或者做一个比较。
***
* FETCH_HEAD

**当使用远程库时，git fetch命令将所有抓取分支的头记录到.git/FETCH_HEAD 中**。FETCH_HEAD是最近抓取（fetch）的分支HEAD的简写，
并且仅在刚刚抓取操作之后才有效。使用这个符号引用，哪怕是一个对没有指定分支名的匿名抓取操作，都可以也在git fetch时找到提交的HEAD。
抓取操作将在第12章详细讲到。
***
* MERGE_HEAD

当一个合并操作正在进行时，其他分支的头暂时记录在MERGE_HEAD中。换言之，MERGE_HEAD是正在合并进HEAD的提交。
***
所有这些符号引用都可以用底层命令git symbolic-ref进行管理。


```text
警告

虽然可以使用这些特殊的名字（例如HEAD）来创建你自己的分支，但这不是个好主意。
```

**Git中有一个特殊符号集来指代引用名。两个最常见的符号“^”和符号“～”将会在下一节中讲述。在转向另一个引用时，
冒号“:”可以用来指向一个产生合并冲突的文件的替代版本**。第9章介绍这一过程。

**NOTE:这些符号引用对我们有什么用？怎么用？这里作者并未提及。下一小节里面有一个git show HEAD~2**

#### <a href='#c6.2.3' id='6.2.3'>6.2.3 相对提交名</a>

Git还提供一种机制来确定相对于另一个引用的提交，通常是分支的头。

你应该已经见过了一些这样的例子，比如，master和master^，其中master^始终指的是在master分支中的倒数第二个提交。还有一些其他的方法，
例如master^^、master～2，甚至像master～10^2～2^2这样复杂的名字。

除了第一个根提交之外 ② ，每一个提交都来自至少一个比它更早的提交，这其中的直接祖先称作该提交的父提交。**若某一提交存在多个父提交，
那么它必定是由合并操作产生的**。其结果是，每个分支都有一个父提交贡献给合并提交。

在同一代提交中，插入符号^是用来选择不同的父提交的。给定一个提交C，C^1是其第一个父提交，C^2是其第二个父提交，C^3是其第三个父提交，
等等，如图6-1所示。

![](https://github.com/YuxingXie/git_study/raw/master/assets/image/06-02-03-01.jpg) 
图6-1　多个父提交名

波浪线～用于返回父提交之前并选择上一代提交。同样，给定一个提交C，C～1是其第一个父提交，C～2是其第一个祖父提交，C～3是第一个曾祖父提交。
当在同一代中存在多个父提交时，紧跟其后的是第一个父提交的第一个父提交。你可能会注意到，C^1和C～1都指的是C的第一个父提交，两个名字都是对的，
如图6-2所示。

![](https://github.com/YuxingXie/git_study/raw/master/assets/image/06-02-03-02.jpg) 
图6-2　多个父提交名

Git也支持其他形式的简写和组合。如C^和C～两种简写形式分别等同于C^1和C～1。另外，C^^与C^1^1相同，因为这代表提交C的第一父提交的第一父提交，
它也可以写做C～2。

通过把引用与“^”和“～”组合，就可以从引用的提交历史图中选出任意提交。不过要注意，这些名字都相对于引用的当前值。如果当前引用指向一个新提交，
那么提交历史图将变为“新版本”，所有父提交“辈分”都会上升一层。

下面这个例子来自Git自身的历史，那是当Git的master分支处于提交1fbb58b4153e90 eda08c2b022ee32d90729582e6的时候。使用命令：

```text
git show-branch --more=35
```


并限制输出最后10行，可以检查提交历史图并研究一个复杂的分支合并结构。

```text
$ git rev-parse master
1fbb58b4153e90eda08c2b022ee32d90729582e6

$ git show-branch --more=35 | tail -10
-- [master~15] Merge branch 'maint'
-- [master~3^2^] Merge branch 'maint-1.5.4' into maint
+* [master~3^2^2^] wt-status.h: declare global variables as extern
-- [master~3^2~2] Merge branch 'maint-1.5.4' into maint
-- [master~16] Merge branch 'lt/core-optim'
+* [master~16^2] Optimize symlink/directory detection
+* [master~17] rev-parse --verify: do not output anything on error
+* [master~18] rev-parse: fix using "--default" with "--verify"
+* [master~19] rev-parse: add test script for "--verify"
+* [master~20] Add svn-compatible "blame" output format to git-svn

$ git rev-parse master~3^2^2^
32efcd91c6505ae28f87c0e9a3e2b3c0115017d8

```


在master～15到master～16之间，进行了一次合并操作，该合并引入了一些其他的合并操作，像名为master～3^2^2^的简单提交。
这恰好是提交32efcd91c6505ae28f87c0e9a 3e2b3c0115017d8。

git rev-parse命令最终决定把任何形式的提交名——标签、相对名、简写或绝对名称——转换成对象库中实际的、绝对的提交散列ID。

**NOTE:没怎么看懂，先略过，希望不影响后续学习。**

### <a href='#c6.3' id='6.3'>6.3 提交历史记录</a>
#### <a href='#c6.3.1' id='6.3.1'>6.3.1 查看旧提交</a>

**显示提交历史记录的主要命令是git log**。比起ls，它有更多的选项、参数、着色器、选择器、格式化器、铃铛口哨和其他小玩意等 ③ 。不过不用担心，
就像使用ls一样，你不需要了解所有的细节。

在参数形式上，git log跟git log HEAD是一样的，输出每一个可从HEAD找到的历史记录中的提交日志消息。变更从HEAD提交开始显示，并从提交图中回溯。
它们大致按照时间逆序显示，但是要注意当回溯历史记录的时候，Git是依附于提交图的，而不是时间。

如果你提供一个提交名（如git log commit），那么这个日志将从该提交开始回溯输出。这种形式的命令对于查看某个分支的历史记当是非常有用的。

**NOTE:这里git log master分明提供的是一个分支名。。。所以git log也可以查看分支的提交。**
```text
$ git log master
commit 1fbb58b4153e90eda08c2b022ee32d90729582e6
Merge: 58949bb... 76bb40c...
Author: Junio C Hamano <gitster@pobox.com>
Date: Thu May 15 01:31:15 2008 -0700

Merge git://repo.or.cz/git-gui

* git://repo.or.cz/git-gui:
　git-gui: Delete branches with 'git branch -D' to clear config
　git-gui: Setup branch.remote,merge for shorthand git-pull
　git-gui: Update German translation
　git-gui: Don't use '$$cr master' with aspell earlier than 0.60
　git-gui: Report less precise object estimates for database compression

commit 58949bb18a1610d109e64e997c41696e0dfe97c3
Author: Chris Frey <cdfrey@foursquare.net>
Date:　 Wed May 14 19:22:18 2008 -0400

Documentation/git-prune.txt: document unpacked logic

Clarifies the git-prune manpage, documenting that it only
prunes unpacked objects.

Signed-off-by: Chris Frey <cdfrey@foursquare.net>
Signed-off-by: Junio C Hamano <gitster@pobox.com>

commit c7ea453618e41e05a06f05e3ab63d555d0ddd7d9

...
```

日志记录是权威的，但是在版本库的整个提交历史记录中进行回滚是不切实际且没有意义的。通常情况下，一个有限的历史记录往往记录了更多的信息。
限制历史记录的一种技术是使用since..until这样的形式来指定提交的范围。给定一个范围，git log将会把在since到until之间的所有提交显示出来。
下面给出一个例子。

```text
$ git log --pretty=short --abbrev-commit master~12..master~10
commit 6d9878c...
Author: Jeff King <peff@peff.net>

clone: bsd shell portability fix

commit 30684df...
Author: Jeff King <peff@peff.net>

t5000: tar portability fix

```

这里，git log显示了在master～12到master～10之间的所有提交，换言之，是主分支上之前10次和第11次的提交。6.3.3节会更详细地讲述范围。

前面的例子还引入了两个格式选项--pretty=short和--abbrev-commit。前者调整了每个提交的信息数量，并且还有其他的几个选项，
包括oneline、short和full。后者只是简单地请求缩写散列ID。

使用-p选项来输出提交引进的补丁或变更。

```text
$ git log -1 -p 4fe86488
commit 4fe86488e1a550aa058c081c7e67644dd0f7c98e
Author: Jon Loeliger <jdl@freescale.com>
Date: Wed Apr 23 16:14:30 2008 -0500

Add otherwise missing --strict option to unpack-objects summary.

Signed-off-by: Jon Loeliger <jdl@freescale.com>
Signed-off-by: Junio C Hamano <gitster@pobox.com>

diff --git a/Documentation/git-unpack-objects.txt b/Documentation/git-unpack-objects.txt
index 3697896..50947c5 100644
--- a/Documentation/git-unpack-objects.txt
+++ b/Documentation/git-unpack-objects.txt
@@ -8,7 +8,7 @@ git-unpack-objects - Unpack objects from a packed archive

 SYNOPSIS
 --------
-'git-unpack-objects' [-n] [-q] [-r] <pack-file
+'git-unpack-objects' [-n] [-q] [-r] [--strict] <pack-file
```

值得注意的是，-1也是一个很不错的选择，它会将输出限制为一个提交。也可以使用-n来将输出限制为最多n个提交。

--stat选项列举了提交中所更改的文件以及每个更改的文件中有多少行做了改动。

```text

$ git log --pretty=short --stat master~12..master~10
commit 6d9878cc60ba97fc99aa92f40535644938cad907
Author: Jeff King <peff@peff.net>

clone: bsd shell portability fix

 git-clone.sh | 3 +--
 1 files changed, 1 insertions(+), 2 deletions(-)

commit 30684dfaf8cf96e5afc01668acc01acc0ade59db
Author: Jeff King <peff@peff.net>

t5000: tar portability fix

 t/t5000-tar-tree.sh | 8 ++++----
 1 files changed, 4 insertions(+), 4 deletions(-)

```


```text
提示

比较git log --stat和git diff --stat的输出，其根本区别在于两者的现实。前者为指定范围中每个单独提交产生一个摘要，
而后者输出命令行中指定的两个版本库状态差异的汇总。
```

另一个查看对象库中对象信息的命令是git show。可以使用它来查看某个提交。

```text
$ git show HEAD~2
```

或者查看某个特定的blob对象信息。

```text
$ git show origin/master:Makefile
```
后者显示的是origin/master分支的Makefile blob。

#### <a href='#c6.3.2' id='6.3.2'>6.3.2 提交图</a>

4.2节介绍了一些可视化布局和Git数据模型中对象的连通性。这些图像十分简明形象，特别是对于Git新手来说。
但是，即使对一个仅仅拥有几个提交、合并和补丁的小版本库来说，需要展示相同细节的图像也是非常难以实现的。
例如，图6-3显示了一幅更完整但仍稍显简单的提交图。试想一下，如果所有提交和数据结构都展现出来会是什么样子？


![](https://github.com/YuxingXie/git_study/raw/master/assets/image/06-03-02-01.jpg) 

图6-3　完整的提交图

然而对提交的约定可以极大地简化蓝图：每个提交都引入一个树对象来表示整个版本库。因此一个提交可以只画成一个名字。

图6-4与图6-3展示了同样的一幅提交图，但是略去了树对象和blob对象。为了便于讨论或引用，通常在提交图中还会显示分支名。
![](https://github.com/YuxingXie/git_study/raw/master/assets/image/06-03-02-02.jpg) 

图6-4　简化的提交图

在计算机科学领域，图（graph）表示的是一组节点和节点之间的一组边。根据不同的属性将图分为几种类型。Git使用其中的一种——有向无环图（DAG）。
顾名思义，DAG具有两个重要的属性。首先，图中的每条边都从一个节点指向另一个节点（称为有向）。其次，从图中的任意一节点开始，沿着有向边走，
不存在可以回起始点的路径（称为无环）。

Git通过DAG来实现版本库的提交历史记录。在提交图中，每个节点代表一个单独的提交，所有边都从子节点指向父节点，形成祖先关系。
你在图6-3和图6-4中看到的图都属于DAG。当谈及提交历史和讨论提交图中提交的关系时，单独的提交节点通常标记为如图6-5所示。
![](https://github.com/YuxingXie/git_study/raw/master/assets/image/06-03-02-03.jpg) 

图6-5　标记的提交图

在这些图中，时间轴都从左到右。A是初始提交，因为它没有父提交，B发生在A之后。E和C发生在B之后，但是对于C和E之间的相对时间关系则没有明确声明；
谁都有可能发生在另一个之前。事实上，Git并不关心提交的时间（无论是绝对时间还是相对时间）。提交的实际“挂钟”时间可能会产生误导，
因为计算机的时间设置可能不正确或不一致。在分布式开发环境中，这样的问题将更加严重。时间戳是不可信的。那么什么是一定的呢？如果提交Y指向父提交X，
那么X就捕获了版本库在Y提交之前的状态，而不用管提交中的时间戳。

提交E和C拥有共同的父提交B。因此，B是一个分支的源头。主分支从提交A、B、C和D开始。同时，提交序列A、B、E、F和G形成名为pr-17的分支。
分支pr-17指向提交G（你可以在第7章阅读到更多有关分支的内容）。

提交H是一个合并提交（merge commit），在此处pr-17分支已经合并到了master分支。因为它是合并操作，所以H有多个父提交，即G和D。这次提交后，
master将指向新提交H，而pr-17仍继续指向提交G（第9章将就合并操作进行更详细的讨论）。

在现实中，插入提交的支根末节是不重要的。此外，提交指向它的父提交的实现细节也经常被忽略，如在图6-6给出的例子。

![](https://github.com/YuxingXie/git_study/raw/master/assets/image/06-03-02-04.jpg) 

图6-6　无箭头的提交图

时间轴还是从左到右，图6-6中有两个分支和一个命名为H的合并提交，并且有向边都简化为线段了，因为这些都是约定俗成的。

这种提交图经常用来讨论一些Git命令的操作和每个操作是如何修改提交历史的。图是比较抽象的表示方法，与此相反，
一些工具（如gitk和git show-branch）则可以将提交历史记录图形象地表现出来。但是在使用这些工具时，时间轴通常自下向上，从最古老的到最近的。
然而，从概念上来说，它们都是同样的信息。

#### <a href='#c6.3.3' id='6.3.3'>6.3.3 提交范围</a>
### <a href='#c6.4' id='6.4'>6.4 查找提交</a>
#### <a href='#c6.4.1' id='6.4.1'>6.4.1 使用git bisect</a>
#### <a href='#c6.4.2' id='6.4.2'>6.4.2 使用git blame</a>
#### <a href='#c6.4.3' id='6.4.3'>6.4.3 使用Pickaxe</a>

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

