# 学习方法建议及Java基础阶段内容

## 1、学习方法

**思考+练习**

### 1.1 思考：学而不思则罔

>  5w + 1h
>
> what：是什么？           why：为什么？
>
> who：什么人，角色    where：什么地方（可以用）？
>
>  when：什么时候（可以用）
>
> ​      how：怎么做

### 1.2 练习 ：欲速则不达；不谋全局者，不足以谋一域

* **欲速则不达**

> 1. 代码出问题要自己思考哪里有问题
> 2. 写代码先梳理思路，写注释，然后再写代码
> 3. 然后把代码删掉，重写一遍

* **不谋全局者，不足以谋一域**

> 1. 整体——>局部
> 2. 注释把整体先写出来。实现（用任何方法）一些难一点的代码，出现问题时，要知道自己要攻克的难关

## 2、Java基础阶段学习

程序就是有序的指令集合。

### 2.1 Java的语言特点

* 面向对象（贴近人类思维模式，模拟现实世界，解决现实问题）
* 安全性（自动内存管理，不易造成内存溢出）
* 跨平台（操作系统，服务器等）

#### Java的执行机制

* 先编译、再解释：
  * 将源文件编译成字节码文件（平台中立文件.class），再将字节码文件进行解释执行

![image-20240716171300676](C:/Users/cxl11/AppData/Roaming/Typora/typora-user-images/image-20240716171300676.png)

### 2.2 DOS命令操作

> 即windows 下的cmd
>
> * 更换盘符：d:
> * 查看当前目录下的文件及文件夹：dir
> * 进入文件夹：cd + 文件夹的名字
> * 返回上级目录：cd ..
> * 创建文件夹：mkdir +  文件夹的名字
> * 删除文件夹：rd +  文件夹的名字
> * 清屏：cls
> * 退出：exit

### 2.3 第一个Java应用程序

* Java程序的开发步骤
  * 编写      .java        记事本
  * 编译      .class       javac命令
  * 运行       java命令

~~~java
public class HelloWorld{
	public static void main(String[] args){
            System.out.print("hello world");
    }
}
~~~

### 2.4 注释

Java三类注释：

​		单行注释：//

​		多行注释：/*   */

​		文档注释：/**    */
​               能够自动生成帮助文档即代码使用说明

~~~java
package demo1;

/**
 * 这是围殴的第一个Java类文件
 * 是我学习的起步
 */
public class day001 {
    /*这里直接输入psvm可直接生成
    这是程序的入口
     */
    /**
     *这是主方法上的文档注释
     * 这是程序入口方法
     */
    public static void main(String[] args) {
        //soup，这是一个输出语句
        System.out.print("hello world！");
    }
}

~~~

#### 如何生成帮助文档

在cmd里输入：javadoc -encoding utf-8 文件名

![image-20240716194103228](C:\Users\cxl11\AppData\Roaming\Typora\typora-user-images\image-20240716194103228.png)

若将生成的帮助文档存入指定文件夹可用

javadoc -d 文件夹名 -encoding utf-8 文件名