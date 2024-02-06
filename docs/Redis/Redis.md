### 第01章 Redis十大数据类型

#### String  
String是redis最基本的类型，一个key对应一个value。  
String类型是二进制安全的，意思是redis的string可以包含任何数据，比如jpg图片或者序列化的对象 。  
String类型是Redis最基本的数据类型，一个redis中字符串value最多可以是512M  



### Redis事务：   

#### 常用命令： 

MULTI、EXEC、DISCARD、WATCH、UNWATCH  

#### Redis事务三特性： 

单独的隔离操作、没有隔离级别的概念、不保证原子性   

#### 事务中的错误处理： 

组队阶段，如果某个命令出现了报告错误，执行时整个的所有队列会都会被取消。  
执行阶段，如果某个命令报出了错误，则只有报错的命令不会被执行，而其他的命令都会执行，不会回滚。