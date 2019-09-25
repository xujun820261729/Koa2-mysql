#### koa-mysql-session koa-session-minimal
- koa2 原生功能只提供了cookie的操作，但是没有提供session操作.需要安装第三方中间件,
- koa-session-minimal 适用于koa2 的session中间件，提供存储介质的读写接口 。
- koa-mysql-session 为koa-session-minimal中间件提供MySQL数据库的session数据读写操作。将sessionId的数据存到数据库


#### Koa中Cookie和Session区别
1. cookie数据存放在客户的浏览器上，session数据放在服务器上。
2. cookie不是很安全，别人可以分析存放在本地的COOKIE并进行COOKIE欺骗
   考虑到安全应当使用session。
3. session会在一定时间内保存在服务器上。当访问增多，会比较占用你服务器的性能
   考虑到减轻服务器性能方面，应当使用COOKIE。
4. 单个cookie保存的数据不能超过4K，很多浏览器都限制一个站点最多保存20个cookie。

