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
> cat pj/C++/hello.cpp | grep "cout" #只显示含有cout的行
> ```

### cal

> ```shell
> cal #显示这个月的日历
> cal 2022 #显示2022年每个月的日历
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

## D

### date

> ```shell
> date #显示当前时间
> date "+%Y" #显示当前年份
> date "+%Y-%m-%d-%H-%M-%S" #显示年-月-日-时-分-秒
> date -s "2022-2-14 15:02:10" #设置系统时间
> ```

## E

### echo

> ```shell
> echo $PATH #输出环境变量
> echo $HOSTNAME #输出主机名
> echo "Hello Linux" #输出Hello Linux
> ```

## F

### find

> ```shell
> find -name hello.cpp #在当前目录下查找hello.cpp文件
> find -user zane #在当前目录下查找zane用户的文件
> find C++/ -size -500k #在C++/目录下查找小于500k的文件（+500大于，500等于，k,M,G）
> ```

## G

### grep

> ```shell
> grep "cout<<" pj/C++/hello.cpp #查找并显示含有cout的行
> grep -n "cout<<" pj/C++/hello.cpp #查找并显示含有cout的行，并显示行号
> grep -i "cout<<" pj/C++/hello.cpp #查找并显示含有cout的行，忽略大小写
> cat pj/C++/hello.cpp | grep "cout" #只显示含有cout的行
> cat pj/C++/hello.cpp | grep -n "cout" #只显示含有cout的行，并显示行号
> ```

### gzip

> ```shell
> gzip text.txt #压缩为后缀为gz格式的压缩包
> gunzip text.txt.gz #解压
> ```
>
> 



## H

```shell
halt #关机
```

### head

> ```shell
> head Project/C++/hello.cpp #显示文件的头部内容，默认前10行
> head -n5 Project/C++/hello.cpp #显示文件前5行
> ```

### history

> ```shell
> history #显示所有的历史命令
> history 10 #显示最近使用过的10个命令
> !10 #再次执行在history里编号为10的命令
> ```

## I

## J

## K

## L

### less

> ```shell
> less Project/C++/hello.cpp #查看文件
> ```
>
> | 操作     | 功能说明                                           |
> | -------- | -------------------------------------------------- |
> | Space    | 向下翻动一页                                       |
> | PageDown | 向下翻动一页                                       |
> | PageUp   | 向上翻动一页                                       |
> | /字符    | 向下搜寻『字串』的功能；n：向下查找；N：向上查找； |
> | ?字符    | 向上搜寻『字串』的功能；n：向上查找；N：向下查找； |
> | q        | 退出less                                           |

### ln

> ```shell
> ln -s Project/ pj #在当前目录创建软链接，pj相当于Project的快捷方式，可cd pj
> ```

### locate

> ```shell
> updatedb #先执行完这个再执行locate
> locate hello.cpp #直接查找hello.cpp文件
> ```

### ls

> ```shell
> ls -a #显示当前目录所在的文件和目录，包括隐藏的
> ls -l #以列表的方式显示信息
> ls -lh #显示当前目录下的文件大小
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

### tail

> ```shell
> tail Project/C++/hello.cpp #显示文件尾部内容，默认是最后10行
> tail -n 5  Project/C++/hello.cpp #显示文件最后5行、
> tail -f Project/C++/hello.cpp #实时监控文件最后
> ```

### tar

> ```shell
> tar -zcvf text.tar text.txt #压缩当前目录下的text.txt文件
> tar -zcvf text.tar.gz text.txt #同上
> tar -zxvf text.tar #将text.tar解压到当前目录
> tar -zxvf text.tar -C temp/ #将text.tar解压到temp/目录
> ```
>
> | 选项 | 功能               |
> | ---- | ------------------ |
> | -c   | 产生.tar打包文件   |
> | -v   | 显示详细信忠       |
> | -f   | 指定压缩后的文件名 |
> | -z   | 打包同时压缩       |
> | -x   | 解包.tar文件       |
>
> 
>

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
  > ```shell
  >  :q	#退出
  >  :q!	#强制退出，不保存
  >  :wq	#保持退出
  >  ```
  >   

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

### zip

> ```shell
> zip -r Project.zip Project/ #把Project目录压缩名为Project.zip的压缩包
> unzip -d temp/ Project.zip #把Project.zip解压到temp/目录下
> ```

## >/>>

### >

> ```shell
> echo "#include<iostream>" > C++/hello.cpp #将#include<iostream>重定向输入到hello.cpp中，并将原内容覆盖
> ```
>
> ```shell
> ls -l /home > /home/info.txt #将home/信息输入到其目录下的info.txt文件下
> ```
>

### >>

> ```shell
> echo "//input" >> C++/hello.cpp #将//input重定向追加输入到hello.cpp的最后一行
> ```
>
> ```shell
> cal >> /home/mycal.txt #将这个月的日历追加到mycal.txt中
> ```
