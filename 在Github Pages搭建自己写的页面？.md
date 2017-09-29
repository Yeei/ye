# 在Github Pages搭建自己写的页面？

------

本人的博客就是在Github上搭建的。下面来分享一下方法。
首先在搭建博客之前，需要做到如下：

> * 自己已经写好的网页文件
> * 注册Github
> * 下载安装git


### [接下来开始搭建：](https://www.zybuluo.com/cmd/)



------


### 步骤一：登录到Github上，新建一个repo，命名成你想要的网页名（这里用test），勾选 initialize this repository with a README，点击create repository。

### 步骤二：打开settings，有一个Github Pages 的设置，点击 source 中的本来的 None ，使其变成 master 分支，也就是作为部署github pages 的分支，然后点击 save。


###步骤三：页面刷新之后，再看 github pages 设置框处，多了一行网址，就是你的 github pages 的网址了。
比如我的就是：

>* https://yeei.github.io/ye/

现在我们就拥有了自己的网址啦！有了自己的网址，没页面啊！

至此以上，github上要处理的操作告一段落，该上Git了！


### 步骤四 ：打开我的电脑，选择一个盘，比如 f 盘，右键空白处点击 git bash here。


###步骤五：输入如下命令，用来在 f 盘创建 test 文件放你的github上的test仓库，克隆test仓库到 test 文件中。
```git
mkdir test 
cd test
git clone test仓库的地址 (点击test仓库中的Clone or download 即可看见)
```
mkdir test：创建一个test文件

### 步骤六： 将自己的网页文件复制粘贴至 f 盘的 test 文件中 
### 步骤七：执行如下命令

```git
cd test
git status
git add .
git status
```
解释一下：
git status 可以让我们时刻掌握仓库当前的状态，列出当前目录所有还没有被git管理的文件和被git管理且被修改但还未提交的文件，也就是所有改动文件，在界面中会红色字体标出。

然后输入 git add .  (有个点) 表示添加当前目录下的所有文件和子目录，

然后 再输入一次 git status 如果看见文件都变绿了 ，那么就代表 它们已经准备好了被提交（git commit）。
```
git commit -m "blog"
```
git commit命令，-m后面输入的是本次提交的说明，可以输入任意内容，当然最好是有意义的，这样你就能从历史记录里方便地找到改动记录。
```
git push
```
git push用于将本地分支的更新,推送到远程主机。
### 8. 最后

打开浏览器输入你的网址。
锵锵锵！！！
完成啦！~

