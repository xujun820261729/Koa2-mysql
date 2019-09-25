#### ejs
1. [基础](https://ejs.bootcss.com/)


#### 标签含义
- <% '脚本' 标签，用于流程控制，无输出。
- <%_ 删除其前面的空格符
- <%= 输出数据到模板（输出是转义 HTML 标签）
- <%- 输出非转义的数据到模板
- <%# 注释标签，不执行、不输出内容
- <%% 输出字符串 '<%'
- %> 一般结束标签
- -%> 删除紧随其后的换行符
- _%> 将结束标签后面的空格符删除


#### 包含
<%- include('user/show'); %>: 中间为引入的地址

####  自定义修饰符
```
var ejs = require('ejs'),
    users = ['geddy', 'neil', 'alex'];

// 单个模板文件
ejs.render('<?= users.join(" | "); ?>', {users: users},
    {delimiter: '?'});
// => 'geddy | neil | alex'

// 全局
ejs.delimiter = '$';
ejs.render('<$= users.join(" | "); $>', {users: users});
// => 'geddy | neil | alex'
```