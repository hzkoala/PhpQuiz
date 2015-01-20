# FrontEnd.Baicheng 笔试题
 
## 公司 & 项目
 
> 历史公司和项目, 担任的角色, 具体的工作, *离职原因*
> 开发环境(Win/Linux) & IDE
 
 
---
## 基础
 
> [A]将十进制24转化为八进制和十六进制表示
> [A]如何对小数四舍五入/向上取整/向下取整
> [L]`==`和`===`的区别
 
### I/O
> [L]get和post的区别
> [L]$_REQUEST包含哪几部分信息
> [H]HereDoc和NowDoc的区别, 哪个可以解析变量
> [H]什么是Restful? Restful中操作资源的方法
> [H]301和302重定向的区别
> [A]输出函数echo/print_r/var_dump/var_export的区别
> [A]双引号和单引号的区别? 哪个效率高?
 
### DateTime
> [L]计算当前时间+7天后的时间, 输出格式`YY-MM-DD HH:MM:SS`
> [H]计算当前时间+7天后00:00:00的时间戳
 
### String
> [A]在GBK/UTF-8下, 一个中文占据的字节数
```
$str = '中文abc';
echo strlen($str);
echo mb_strlen($str);
```
> [A]如何保证字符编码的统一(DB/PHP/HTML)
 
### Array
> [H]从一个数组中, 随机取一条数据
> [A]合并两个数组, 一组作为key, 一组作为value(元素个数相同)
 
### File & Dir
> [L]include和require区别
> [L]如何判断目录/文件存在
 
### Error & Exception
> [L]异常的抛出和捕获
> [H]如何关闭Notice级别的提醒信息
> [H]如何自定义error/exception处理方法
> [A]如何全局性地处理错误和异常
 
### Class
> [L]public/protected/private修饰符的区别
> [H]final修饰符的含义
> [H]static修饰符的含义
> [A]如何在类方法中使用全局变量
 
### Session & Cookie
> [H]Session的实现机制
> [H]Cookie的实现机制
> [A]Session和Cookie的区别
 
### 引用
> [H]执行结果?
```
$a = 'test';
$b = & $a;
unset($b);
echo $a;
```
```
$a = 'test';
$b = & $a;
unset($a);
echo $b;
```
 
### Comment
> [L]Php支持哪几种注释方法
> [H]PhpDoc方法注释包含哪几部分信息
 
### Regex
> [L]使用正则匹配`http://www.baicheng.com/dir/file.html`中的域名
> [H]使用正则匹配`http://www.baicheng.com:8080/dir/file.html`中的域名和端口号
 
### Script
> [H]Php脚本以命令行方式执行, 如何接收参数
 
### Cache & NoSQL
> [A]Memcache和Redis的区别, 使用场景
 
### Autoload
> [H]spl_autoload_regist()的用法? 如何指定全局函数/类(静态)方法
 
### 魔术方法
> [H]列举常用的魔术方法和对应的含义
 
### Safe
> [H]XSS(Cross Site Script)和CSRF(Cross Site Request Forgery)的原理, 如何避免
 
### MySQL
> [H]char和varchar的区别
> [H]事务和使用场景
> [A]如何防止SQL注入
> [A]MySQL的存储引擎种类? 各自的特点和使用场景?
> [A]MySQL较慢时的优化方法
 
### JavaScript
> [L]alert/confirm/prompt区别
> [H]$(document).ready()和window.onload的区别
 
 
---
## 疑难
 
### mkdir掩码问题
> [P]使用`mkdir($path, 0777)`函数创建目录, 但others不可写, 可能的原因
 
### mb系函数内部编码问题
> [H]文件编码UTF8, $str = "中文", `echo mb_strlen($str)`结果为6, 可能的原因
 
### md5
> [L]如何安全地存储用户密码
 
### encrypt
> [H]对称加密和非对称加密的区别? md5属于哪种?
 
 
---
## 架构
 
### Framework
> [A]使用过哪些PHP开源框架? 各自的特点?
 
### MVC
> [A]MVC的含义? Controller和Buziness层如何划分?
 
### 高并发
> [H]高并发的对应方法(用户端Web/服务端Api)
 
### 设计模式
> [P]列举常见的设计模式和使用场景
 
### SOA
> [P]SOA的含义, 优势, 关键点
 
### ORM
> [P]ORM的含义? 如何实现一个简单的ORM?
 
