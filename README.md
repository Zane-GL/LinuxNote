# Linux Command Set

## A

---



## B

## C

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

>less
>

## M

### man

功能：获取帮助信息

```shell
man ls #获取ls命令的帮助信息
```

### mkdir

> ```shell
> mkdir Project #在当前目录下创建Project目录
> ```

## N

## O

## P

## Q

## R

```shell
reboot #现在重新启动计算机
```

-----

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
