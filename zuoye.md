```c
#include<stdio.h>
int main(){
    int x = 5, y = 10;

    printf("originally x  =%d and y = %d.\n", x, y);
    interchange(x, y);
    printf("Now x =%d and y = %d.\n", x, y);

    return 0;
}

void interchange(int u, int v){
    int temp;

    printf("originally u = %d and v = %d.\n", u, v);
    temp = u;
    u = v;
    v = temp;
    printf("Now u = %d and v = %d.\n", u, v);
}
	
```

1.我们为什么需要git？

答：它能为开源项目免费提供git储存。

分布式版本控制系统分布式版本控制系统根本没有“中央服务器”

每个人的电脑上都是一个完整的版本库

这样，你工作的时候，就不需要联网

因为版本库就在你自己的电脑上。

而分散式需要联网才能工作，且分散式如果中央服务器垮掉，

很多人都无法工作了

2.命令

命令mkdir (文件名)为创建文件

pwd为查看当前文件位置

git init 命令为把这个目录编程git可以管理的仓库

git commit命令，-m后面输入的是本次提交的说明

可以输入任意内容

当然最好是有意义的，这样你就能从历史记录里方便地找到改动记录

命令git reflog用来记录你的每一次命令

cat readme.txt用来查看内容

git log 用来查看版本库的状态

加上--pretty=oneline会变的简便一点

git reset --hard为回溯版本

上一个版本就是HEAD^，

上上一个版本就是HEAD^^，

当然往上100个版本写100个^比较容易数不过来，

所以写成HEAD~100

HEAD指向当前版本

Git允许我们在版本的历史之间穿梭，

使用命令git reset --hard commit_id

要重返未来，用git reflog查看命令历史

以便确定要回到未来的哪个版本。

git checkout -- file可以丢弃工作区的修改

git reset HEAD <file>可以把暂存区的修改撤销掉（unstage）

，重新放回工作区

git status为查看当前工作区与暂存区状态

ls为查看当前地址的文件

用`git push`命令，实际上是把当前分支`main`推送到远程。

由于远程库是空的，我们第一次推送`master`分支时，加上了`-u`参数，Git不但会把本地的`master`分支内容推送的远程新的`master`分支，还会把本地的`master`分支和远程的`master`分支关联起来，在以后的推送或者拉取时就可以简化命令。

```
推送成功后，只要本地做了提交，就把本地可以通过命令：git push origin 
```

把本地main分支的最新修改推送至GitHub，现在，你就拥有了真正的分布式版本库！

如果添加的时候地址写错了，或者就是想删除远程库，可以用`git remote rm <name>`命令。使用前，建议先用`git remote -v`查看远程库信息：

命令`git clone`克隆一个本地库

```
格式为: git clone git@github.com:youname/gitskills.git
```

要克隆一个仓库，首先必须知道仓库的地址，然后使用`git clone`命令克隆。

Git支持多种协议，包括`https`，但`ssh`协议速度最快。

查看分支：git branch

创建分支：git branch name(分支名)

切换分支：git checkout name(分支名)或者git switch name

创建+切换分支：git checkout -b name或者git switch name

合并某分支到当前分支：git merge name

删除分支：git branch -d name

**git pull** 命令用于从远程获取代码并合并本地的版本。

```
git pull <远程主机名> <远程分支名>:<本地分支名>
```

将远程主机 () 的 () 分支拉取过来，与本地的 () 分支合并

<video src="D:\gal\000不剧透.mp4"></video>

[bilibili]: https://www.bilibili.com/

```c
#include<stdio.h>
int recursion(int n);

void main(){

​    int n;
​    printf("输入你的数值:");
​    scanf("%d",&n);

}

int recursion(int n){
    int recur = 0;

​    if (recur < n)

​    {

​        recursion(recur + 1);

​    }
​    printf("第%d的和为%d",n, recursion(n));
}


```

```java
public class Switchdemo{
    public static void main(String args[]){
        int x = 5, y = 7;
        switch (x * y){
            case 10 :
                System.out.println("10");
                break;
            case 20 :
                System.out.println("20");
                break;
            case 30 :
                System.out.println("30");
                break;
            default :
                System.out.println("以上没有匹配的")；
        }
    }
}
```

[ASCLL对照表]: https://tool.oschina.net/commons?type=4	"这是连接"

爱你，鸥酱，mua~

```c
#include <stdio.h>
int main () {
    int var_runoob = 10;
    int *p;              // 定义指针变量   
    p = &var_runoob;   
    printf("var_runoob 变量的地址： %p\n", p);   
    return 0;
}
```

```c
#include <stdio.h>
 
enum DAY
{
      MON=1, TUE, WED, THU, FRI, SAT, SUN
};
 
int main()
{
    enum DAY day;
    day = WED;
    printf("%d",day);
    return 0;
}
```

希望鸥酱感冒早日好起来哦，鸥酱要多注意点身体，多喝点热水，多出出汗，让病毒早日排除去，我期待着鸥酱好起来，继续给我布置任务哦！

我这几天先看看指针和Linux命令，再看看怎么弄博客.

**慎用** rm

**勿试** rm -rf /* 。用 rm 删除的文件难以找回，可能会造成不可挽回的损失。在一个项目中一般是 **建立一个 delete 文件夹**，然后使用 mv 指令移走文件，**定时对 delete 进行删除**。

**rm -rf /D**：删除指定目录 D 以及其所有子目录和文件

**rm -rf \*** ：删除当前文件夹下的所有文件而保留该文件夹

**rm -rf /**：删除一整个根目录 / 有些版本的系统会提示你这很危险，但有的不会！

这会删除绝大部分的文件，只要权限足够都会删。所以有时候会发现执行完这个命令后，还有一些残余的目录和文件。但其实你的文件已经不完整了，如果在linux系统下，会导致命令丢失无效（比如cd，ls）。

**rm -rf /\***：**直接强制删除**一整个根目录 / ，数据无价，没有后悔药

① 无参 删除当前目录下的指定文件（但不能删除空目录 ）

② **rm -d** ：   -d 指 --dir，删除空目录，同 rmdir

③ **rm -f** ：    -f 指 --force，强制删除，忽略系统提示，即使该文件不存在

④ **rm -i** ：    -i 指 --interactive，顾名思义，交互式删除，系统将询问是否确认删除

⑤ **rm -r** （-R）：-r 指 --recursive， 指将当前目录和全部子目录及文件递归删除

⑥ **rm -v** ： -v 指 --verbose，显示删除的步骤信息

- Normal模式：Normal模式是最常用的模式，在该模式下，主要浏览、修改文本内容；（进入 vim filename 退出 ：:wq）
- Insert模式：在该模式下，主要添加文本内容；（i,s,o键进入  Esc键退出）
- Visual模式：在该模式下，主要选取文本内容，还可以以行或列为单位选取文本内容，有一种用鼠标选择的即视感，非常方便；（v 进入    Esc键 退出）
- Command模式：在该模式下，主要通过命令来操作文本文件，而非文件内容，如保存、退出等。（:键进入  Esc 退出）
- :w    保存当前文件.
- :wq   保存并退出.
- :q!      放弃修改，强制退出.
- :f         显示文件名称、总行.

```c
#include<stdio.h>
void miyakoCal(int, int, int, int, int, char);                                  //   声明函数
void main() {                                                                   //   主函数入口
    int x = 34, y = 65, z = 20 , l = 5 ,w = 3;
    char d = 'a';
    miyakoCal(x, y, z, l, w, d);

}
void miyakoCal(int x, int y, int z,int lenth, int width, char direct) {         //  miyakoCal：喵都计算器
    printf("输入的Minecraft坐标为：[坐标]= %d,%d,%d\n", x, y, z);
    printf("输入的展开半径为：[width]= %d\n", width);
    printf("输入的展开长度为：[length]= %d\n", lenth);
    switch (direct)
    {
        case 'a':
            printf("靠X轴正半轴展开......\n");
            break;
        case 'b':
            printf("靠X轴负半轴展开......\n");
            break;
        case 'c':
            printf("靠Z轴正半轴展开......\n");
            break;
        case 'd':
            printf("靠Z轴负半轴展开......\n");
            break;
        default:
            printf("不属于任何一种条件，程序即将退出......\n");
            break;
    }
}
```

```c
#include <stdio.h>
 
const int MAX = 3;
 
int main ()
{
   int  var[] = {10, 100, 200};
   int  i, *ptr;
 
   ptr = var;
   for ( i = 0; i < MAX; i++)
   {
 
      printf("存储地址：var[%d] = %p\n", i, ptr );
      printf("存储值：var[%d] = %d\n", i, *ptr );
 
      ptr++;
   }
   return 0;
}//提问：为啥（ptr = var）里面没有用到&呢，虽然用了之后还可以运行，"message": "assignment to 'int *' from incompatible pointer type 'int (*)
}
```

