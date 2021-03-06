# VueMovieWebsite
使用 Vue + Node.js + Express + MongoDB + iView 实现的一个电影社区网站。由于时间有限，一些细节可能不够完善。

更多相关内容可参考我的博客：[Vue.js学习笔记](https://blog.csdn.net/weixin_42762089/article/details/91492148#Vue.js%E7%94%B5%E5%BD%B1%E7%BD%91%E7%AB%99%E9%A1%B9%E7%9B%AE)

## 安装

此项目分为服务端和前端，服务端代码在 `book_service` 文件夹中，前端代码在 `book_view` 文件夹中，数据库文件在 `database` 文件夹中（分为 json 和 sql 两种格式）

1. 先下载源代码，并且安装 `Node.js`

2. 安装模块：命令行环境进入`book_service` 文件夹，执行 `npm instll`，同样进入`book_view` 文件夹，执行 `npm instll`

3. 启动服务：命令行环境进入`book_service` 文件夹，执行 `npm start`，同样进入`book_view` 文件夹，执行 `npm start`

4. 在浏览器中打开网址即可： http://localhost:8080 

## 1.技术选择

数据库：[MongoDB](https://www.mongodb.com/)（一个介于关系数据库和非关系数据库之间的产品）

服务器端：[JavaScript](https://www.liaoxuefeng.com/wiki/1022910821149312) + [Node.js](http://nodejs.cn/) + [Express框架](http://www.expressjs.com.cn/)

前端：[Vue.js框架](https://cn.vuejs.org/index.html)

UI库：[iView](https://www.iviewui.com/)

## 2.开发环境

IDE：WebStorm

MongoDB可视化界面软件：Studio 3T

服务器测试：Postman客户端

## 3.主要功能

* 前台   

1. 用户的注册、登录、忘记密码、个人资料显示

2. 主页显示电影推荐及影评推荐

3. 电影详细信息页面：显示电影名称、上映日期、预告片地址、观看次数、点赞次数、观看地址、已审核的用户评论

4. 影评详细信息页面：显示影评标题、发布日期、影评内容、已审核的用户评论

5. 用户对电影的浏览、评论、点赞、跳转到观看网址

6. 用户对影评的浏览、评论

* 后台

1. 电影管理: 查询所有电影、添加电影、删除电影、修改电影信息、更新主页的推荐电影
   
2. 影评管理：查询所有影评、添加影评、删除影评、修改影评信息、更新主页的推荐影评
    
3. 评论管理：查询所有用户评论、删除用户评论、审核用户评论
     
4. 用户管理：查询所有用户、删除用户、封停/解封用户、修改用户身份（用户/管理员）、修改用户权限（0-普通用户，1-普通管理员，2-超级管理员，数字越大权限越高）

## 4.数据库描述

数据库主要有6张表：

1. articles 影评表

2. comments 用户评论表

3. movies 电影表

4. recommends 主页显示大图的电影表

5. users 用户表

6. mails 站内信表（时间有限，此功能前台部分未实现）

## 5.项目截图

![首页](screenshot/1.首页.png)

![注册页面](screenshot/2.注册页面.png)

![登录页面](screenshot/3.登录页面.png)

![电影列表页面](screenshot/4.电影列表页面.png)

![影评列表页面](screenshot/5.影评列表页面.png)

![电影详情页面](screenshot/6.电影详情页面.png)

![影评详情页面](screenshot/7.影评详情页面.png)

![后台管理主页面](screenshot/8.后台管理主页面.png)

![电影管理页面](screenshot/9.电影管理页面.png)

![添加电影页面](screenshot/10.添加电影页面.png)

![影评管理页面](screenshot/11.影评管理页面.png)

![添加影评页面](screenshot/12.添加影评页面.png)

![评论管理页面](screenshot/13.评论管理页面.png)

![用户管理页面](screenshot/14.用户管理页面.png)
