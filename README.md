# community-forum-By-SpringBoot

基于SpringBoot+MyBatis实现，并集成了MySQL,Redis，Kafka，Elasticsearch等。实现了账号注册，会话管理，文章发表，富文本编写显示，生成验证码，文章搜索，账号管理，过滤敏感词，评论私信点赞，事务管理等功能。



## 工具（tools）

JDK1.8；

IDEA：IntelliJ IDEA 2020.1.1 x64



## 界面

#### 首页

显示前十个文章，通过分页显示全部文章，默认按发表时间逆序，热度排行按公式排。并可以显示置顶加精贴。

![image-20201102175505880](https://github.com/Wenbin94/community-forum-By-SpringBoot/edit/master/img/image-20201102175505880.png)

#### 帖子文章详情

文章详情，通过Spring Security 权限控制并实现了点赞，评论回复，并使用Kafka构建异步消息系统。

![image-20201102182726622](img\image-20201102182726622.png)

![image-20201102182731536](img\image-20201102182731536.png)

#### 登录界面

验证账号密码及验证码，成功时生成凭证发给客户端，服务器通过Redis存储登录凭证。失败时跳回登录页。

![image-20201102183351103](img\image-20201102183351103.png)



#### 私信通知列表

使用Redis处理点赞，关注等功能

![image-20201102183445951](img\image-20201102183445951.png)

#### 文章发帖界面

集成markdown富文本编辑器。

![image-20201102183546721](img\\image-20201102183546721.png)
