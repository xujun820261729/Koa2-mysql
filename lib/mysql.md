#### mysql 模块封装
1. [基础知识](https://www.runoob.com/nodejs/nodejs-mysql.html)
2. posts(存储文章)，users(存储用户)，comment(存储评论)，create table if not exists users()表示如果users表不存在则创建该表
3. mysqladmin -uroot -proot processlist 查看当前的mysql连接数
4. 封装的query()使用的是node.js的连接池
5. 强调使用sql不能使用拼接等，会造成sql注入