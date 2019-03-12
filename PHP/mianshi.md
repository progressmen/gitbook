
<!-- toc -->

### 1.echo print print_r var_dump区别
 - echo()  
可以一次输出多个值，多个值之间用逗号分隔。echo是语言结构(language construct)，而并不是真正的函数，因此不能作为表达式的一部分使用。
 - print()  
函数print()打印一个值（它的参数），如果字符串成功显示则返回true，否则返回false。
 - print_r()  
可以把字符串和数字简单地打印出来，而数组则以括起来的键和值得列表形式显示，并以Array开头。但print_r()输出布尔值和NULL的结果没有意义，因为都是打印"\n"。因此用var_dump()函数更适合调试。
 - var_dump()  
判断一个变量的类型与长度,并输出变量的数值,如果变量有值输的是变量的值并回返数据类型。此函数显示关于一个或多个表达式的结构信息，包括表达式的类型与值。数组将递归展开值，通过缩进显示其结构。


### 2.事务的隔离级别
https://www.cnblogs.com/xrq730/p/5087378.html  
事务会产生的问题:  
脏读  : 事务A读到了事务B还没有提交的数据  
不可重复读 :在一个事务里面读取了两次某个数据，读出来的数据不一致  
幻读 :在一个事务里面的操作中发现了未被操作的数据  
隔离级别:  
1) 默认  default  
2) 读未提交  read uncommited  
3) 读已提交  read commited  
4) 重复读取   repeatable read  
5) 串行化 serlalizable  

### 3.聚簇索引
索引从数据存储方式上可以分为聚簇索引和非聚簇索引
### 4.常见的魔术方法
__clone  __call __construct  __Tostring (当字符串使用时候输出内容，必须有返回值)
### 5.Linux产看内存使用情况命令，端口占用命令，等常用命令
 top 查看cpu 内存占用
free 查看
netstat -tunlp |grep 查看端口占用




