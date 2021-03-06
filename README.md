# Talent Blog

作为一个合格的程序员，拥有一个属于自己的博客是必须的，既可以督促自己不断学习积累，也可以在回顾的时候带来不小的成就感，通过一星期零碎的时间，就可以从０基础搭建一个简单的博客,通过一个小任务来掌握一些基础知识和技能.

## 可以学到什么

- 简单的linux命令行操作
- 基本的配置环境技能
- markdown语法写作
- git分支管理
- 如何使用搜索引擎
- 如何阅读文档和手册

## 需要什么

- 利用框架快速搭建静态博客,不需要任何一门编程语言知识.
- 可以将静态博客部署到github上面,有条件可以尝试部署到服务器上面.
- 有条件可以尝试购买域名,解析到github上面,但是对github.io不嫌弃也可以不用.
- 如果打算完成上一条可以尝试给域名备案.

## 一些要求

- **每天定时push**:必须要有学习笔记的记录和思考,在每天11:30前push到github对应仓库自己的分支上.
- **独立思考**:在遇到问题不去直接问别人,尝试使用搜索引擎(**重要**),我在搭建自己的博客的时候并没有求助于他人并且最后完成了任务,这个过程可能比较坎坷,但是希望能够坚持.
- 使用框架的同时思考背后的原理并且完成相应的思考题目.

## 提示

- 在遇到问题,无论是命令行报错还是功能出问题,都试着去求助于搜索引擎,建议使用的包括但不限于[百度](https://www.baidu.com),[知乎](https://zhihu.com/),(不熟悉英文环境)[谷歌](https://www.google.com),[Stack Overflow](https://stackoverflow.com/)(想挑战自己),而且报错要筛选出有用的信息,一般来说错误码也是比较好的选择.

- 遇到配置问题不要轻易复制粘贴配置特别是CSDN上面的配置(大部分都可能有问题),尝试知乎或者找时间比较新的文章,而且配置往往随着操作系统的不同而不同,这点要注意.

- 以上两点是比较坏的选择,最好的方案当然是去阅读官方文档还有官方的Q&A,可以涵盖你可能遇到的绝大部分问题.

  

## 提供的资源

[git的学习](https://www.liaoxuefeng.com/wiki/896043488029600)

[如何用hexo搭建博客](https://zhuanlan.zhihu.com/p/35668237)

[hexo](https://hexo.io/zh-cn/)

[fluid](https://github.com/fluid-dev/hexo-theme-fluid)(一个我喜欢的博客模板,不过可以根据喜好切换)

## 学习计划以及任务(不定期更新)

## Day 1~Day 2

1. 学会一些简单的git命令,包括但不限于add commit push pull clone等等.

2. 在团队仓库内创建自己的分支,并且将自己的学习记录和每日的问题答案提交上去.

   ```bash
   #1.为什么我们需要git
   
   
   #2.当你对自己代码进行了一些更改想要提交到远程仓库需要执行哪些命令
   
   
   #3.接着上一题,在你提交完成以后想要回溯回去上一个版本应该执行什么命令
   
   
   #以上问题独立完成填写到空白处并且提交到自己的分支上去,不得询问他人,对题意理解不清可以私戳
   ```


## Day 3

学习使用markdown,可以为未来写文档和博客提供便利

1.安装typora,一款markdown编辑器(群里应该有),把你之前写的笔记改写成markdown形式(文件名字以.md结尾)

2.一些简单的应用,写一份新的文件,里面包含各级标题,超链接,代码块(写一份c语言代码上去吧),并且push到自己仓库对应的分支上去

3.学习git pull.

## Day 4~5

1. 安装ubuntu虚拟机(记得必须要用英文环境),学会基本的命令行操作
2. 配置hexo需要的基本环境([阅读官方文档](https://hexo.io/zh-cn/))
3. 试着跟着官方文档将博客运行起来
4. 基本的vim语法
5. 回答下列问题

```bash
#1.如何通过apt-get安装卸载软件(ubuntu系统)


#2.当在安装某些软件的安装过程中往往会出现失败或者环境配错等故障,如何干净得卸载这个软件以及其所有依赖


#3.基本的vim语法,如何进入insert模式,如何在编辑完成之后保存文件并退出


#4.linux下这几个命令对应含义是什么
cd 
ls 
pwd 
mkdir 
rm -rf 
#5.如何通过命令行返回上级目录
```

任务量比较大,请分批完成,并且每天记得push