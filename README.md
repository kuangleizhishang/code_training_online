# 升华工作室程序部线上培训

虽然线下培训结束了 不过咱们的微信小程序培训还没有进行= =

微信小程序的开发逻辑与vue有些许相似，因此大家把重要精力放在小程序特有的写法上即可

**小程序前后端各有独特的写法与逻辑，请各位根据自己想研究的技术方向着重选择，本次培训结束后会进行前后端分流哈**

### 小程序前端

小程序前端采用MVVM架构，基本的写法逻辑与vue相似，请大家前往**微信开放文档**进行相关的学习

##### 任务：（大部分可以在微信开放文档中查阅到相关指引）

1. 注册小程序账号

2. 下载微信开发者工具

3. 创建小程序项目
4. 搞懂小程序的项目目录 ``.wxml .wxss .js .json``
5. 熟悉小程序的生命周期
6. 小程序js中的this指针作用域（这点不同于vue）
7. 熟悉一些常用API，比如发起请求、显示弹窗、设置页面数据之类的
8. 会使用开发者工具进行预览、调试和真机调试
9. 会查阅开放文档中的API

##### 传送门

1. [🔗微信开放文档](https://developers.weixin.qq.com/miniprogram/dev/framework/)
2. [🔗申请账号](https://developers.weixin.qq.com/miniprogram/dev/framework/quickstart/getstart.html#%E7%94%B3%E8%AF%B7%E5%B8%90%E5%8F%B7)
3. [🔗下载开发者工具](https://developers.weixin.qq.com/miniprogram/dev/framework/quickstart/getstart.html#%E5%AE%89%E8%A3%85%E5%BC%80%E5%8F%91%E5%B7%A5%E5%85%B7)

##### 附注

微信开发者工具自带的编辑器不好用（现在这个版本好像好了很多），而且对小屏笔记本极其不友好，所以可以选用vscode进行开发，下载这几个插件可以很好地进行小程序开发：

- miniapp

- wechat-snippet

- wxapp-helper


然后在vscode里写好保存之后切换到微信开发者工具编译运行即可

### 小程序后端&运维

小程序后端与普通后端区别不大，主要是在小程序进行**登录**时需要向微信的接口发起请求用code来换取session_key与用户的open_id，依旧跟着微信官方的文档来就好

另外，小程序最大的不同是后端服务器的配置，**小程序必须用HTTPS协议向一个ICP备案的域名指向的服务器发起请求**。域名问题不用担心，工作室有。SSL证书需要我们自己配置。

##### 任务：

1. 搞明白如何向微信接口发请求用code（前端请求中携带）换取session_id
2. 学习阿里云控制台的使用，学会配置安全组来开放端口等
3. 学习Nginx配置，掌握如何将发送的请求转发到后端监听的端口上
4. 学习使用certbot配置免费的SSL证书

##### 传送门：

1. [🔗服务端文档](https://developers.weixin.qq.com/miniprogram/dev/api-backend/)
2. [🔗certbot](https://certbot.eff.org/)

### 作业 :）

请各位使用小程序完成一个**TODO List**，在**12.16（周三）前**交到这个仓库来**（交项目的文件夹，别交错了）**，如果在学习与完成作业的过程中有任何疑问，请在qq*群里及时提问哈*

*ddl设置到16号是因为周末考四六级 大家别拖着 有空就学点*

TODO List功能参考：

- 待办事项与已完成事项的展示
- 标记完成一个事项或者撤回一个已经完成的事项
- 添加待办事项
- 删除一个事项

参考网站（功能上的参考）：[🔗todolist](http://www.todolist.cn/)

