#### QA
1. Q:ctx.render is not a function  报这个错?
- A： 造成这个bug的原因是因为中间件的执行是有顺序的，路由在前，然后模板引擎在后的话，当执行到ctx.render的时候，模板引擎相关的中间件还未执行，render方法还未绑定到ctx上，所以就会报ctx.render is not a function

