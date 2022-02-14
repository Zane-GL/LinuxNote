# Linux Command Set

## A

---



## B

## C

### cat

> ```shell
> cat hello.cpp #查看当前目录下的hello.cpp文件的内容
> cat -n hello.cpp  #查看当前目录下的hello.cpp文件的内容，并加上行号
> cat -n hello.cpp | more  #查看当前目录下的hello.cpp文件的内容，并加上行号，more是用来翻页的
> ```

### cd

> ```shell
> cd ~  #回到当前用户的目录主目录
> cd .. #返回当前目录的上一级目录；同理，cd../.. 返回上上级目录
> ```

### cp

>```shell
>cp TEXT/temp.txt text/ #拷贝TEXT目录下的temp.txt文件到text/目录下
>cp -r text/ TEXT/ #递归拷贝text/目录到TEXT/目录下
>\cp -r text/ TEXT/ #递归拷贝 text/目录 并强制覆盖到TEXT/目录下
>```
>
>

## D

## E

## F

## G

## H

```shell
halt #关机
```

## I

## J

## K

## L

### ls

> ```shell
> ls -a #显示当前目录所在的文件和目录，包括隐藏的
> ls -l #以列表的方式显示信息
> ```



## M

```shell
man ls #获取ls命令的帮助信息
```

### mkdir

> ```shell
> mkdir Project #在当前目录下创建Project目录
> mkdir -p Project/C++ #创建多级目录
> ```

### more

> ```shell
> more hello.cpp #查看文件
> ```
>
> | 操作   | 功能说明                        |
> | ------ | ------------------------------- |
> | space  | 向下翻一页                      |
> | Enter  | 向下翻一行                      |
> | q      | 立刻离开more,不再显示该文件内容 |
> | Ctrl+F | 向下滚动一屏                    |
> | Ctrl+B | 返回上一屏                      |
> | =      | 输出当前行的行号                |
> | :f     | 输出文件名和当前行的行号        |

### mv

>```shell
>mv text text0 #重命名当前目录下的text/目录
>mv text0/ TEXT/ #移动目录
>```
>

## N

## O

## P

```shell
pwd #显示当前的工作目录的绝对路径
```



## Q



## R

```shell
reboot #现在重新启动计算机
```

### rmdir

>```shell
>rmdir project/ #删除project目录（空）
>rmdir -p TEXT/text/ #删除多级目录 前提text是空目录
>```

### rm

> ```shell
> rm hello.cpp #删除当前目录下的文件
> rm -r TEXT/text/ #删除TEXT/下的text/目录
> rm -f TEXT/text.txt #强制删除TEXT/目录下的text.txt文件，不会有提示
> rm -rf TEXT/ #递归强制删除TEXT目录，其下级目录也跟着删除
> ```



## S

### shutdown

> ```shell
> shutdown-h now #立该进行关机
> shudown-h 1 #1分钟后关机
> shutdown-r now #现在重新启动计算机
> ```

```shell
sync #把内存的数据同步到磁盘
```



## T

### touch

```shell
touch text.txt #当前目录下创建txt文件
touch text/text.txt #在已有的目录text/下创建txt文件
```



## U

## V

### vi / vim

**vi** 文本编辑命令

**vim** vi的增强版，具有较强的程序编辑能力

- 正常模式 

  > 按下 esc 后的模式
  >
  > 以vim打开一个档案就直接进入一般模式了(这是默认的模式)。在这个模式中,你可以使用『上下
  > 左右』按键来移动光标,你可以使用『除字符』就『删除整行』来处理档案内容,也可以使用
  > 『复制、粘贴』来处理你的文件数据

- 插入模式 

  > 按下 i 后的模式
  >
  > 按下i,IO,O,a,A,r,R等任何一个宇母之后オ会进入编損模式一般来说用 i 即可

- 命令行模式

  > 按下 esc 再按下 : 后的模式
  >
  > 在这个模式当中,可以提供你相关指令,完成读取、存盘、替换、离开vim、显示行号等的动作
  > 则是在此模式中达成的!
  >
  > **指令** 
  >
  > - ```shell
  >   :q	#退出
  >   ```
  >
  > - ```shell
  >   :q!	#强制退出，不保存
  >   ```
  >
  > - ```shell
  >   :wq	#保持退出
  >   ```

**快捷键**

- yy 拷贝当前行,拷贝当前行向下的5行5yy,并粘贴(输入p)。
- dd 删除当前行 ，5dd 删除当前行向下的5行 
- u 撤销上一次的 行输入
- /关键字 在文件中查找，输入n就是查找下ー个
- : set nu 设置文件的行号   
- : set nonu 取消文件的行号
- 行号 + shift + g 将光标移动到相应行
- gg 定位到首行
- G 定位到末尾行

**实例: **在终端输出 Hello Linux!

```shell
vim hello.cpp #用vim创建hello.cpp文件并进入
```

```c++
#include <iostream> 
using namespace std;

int main (){
    cout<<"Hello Linux!"<<endl;
    return 0;
}
```

```shell
g++ hello.cpp -o hello #编译
./hello	#运行
```



## W

## X

## Y

## Z
