#### QA
1. Q:ctx.render is not a function  报这个错?
- A： 造成这个bug的原因是因为中间件的执行是有顺序的，路由在前，然后模板引擎在后的话，当执行到ctx.render的时候，模板引擎相关的中间件还未执行，render方法还未绑定到ctx上，所以就会报ctx.render is not a function

2. Q: 为什么我启动时候报错sql的client 需要更新?
- A: 这个原因是由于,sql8.0后更换 修改密码的方式更换下密码即可

3. Q : 这个已经封装好的koa2架子如何使用?
- A : 其实很简单，学习下每个模块的使用在DOCS里,学习下文件的路由即可

4. Q: 如何使用 koa-session2 ioredis 来管理用户的 session?
- A ：详情看DOCS中的 koa-mysql-session 介绍