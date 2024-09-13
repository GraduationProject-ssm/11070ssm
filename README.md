# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# 11070ssm疫情防控物业管理系统文件

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1Kp48e9EtU?p=112)


# 系统概述
进过系统的分析后，就开始记性系统的设计，系统设计包含总体设计和详细设计。总体设计只是一个大体的设计，经过了总体设计，我们能够划分出系统的一些东西，例如文件、文档、数据等。而且我们通过总体设计，大致可以划分出了程序的模块，以及功能。但是只是一个初步的分类，并没有真正的实现。

整体设计，只是一个初步设计，而且，对于一个项目，我们可以进行多个整体设计，通过对比，包括性能的对比、成本的对比、效益的对比，来最终确定一个最优的设计方案，选择优秀的整体设计可以降低开发成本，增加公司效益，从这一点来讲，整体设计还是非常重要的。

` `疫情防控物业管理系统 工作原理图如图4-1所示：

![](/md/blog.012.png)

图4-1 系统工作原理图
## 4.2 系统结构设计
系统架构图属于系统设计阶段，系统架构图只是这个阶段一个产物，系统的总体架构决定了整个系统的模式，是系统的基础。 疫情防控物业管理系统 的整体结构设计如图4-2所示。

![](/md/blog.013.png)

图4-2 系统结构图
## 4.3数据库设计
数据库是计算机信息系统的基础。目前，电脑系统的关键与核心部分就是数据库。数据库开发的优劣对整个系统的质量和速度有着直接影响。

[4.3.1数据库设计](#_Toc273815984)

[4.3.2数据库简介](#_Toc273815985)

数据库是信息系统的基础和核心。数据库设计的好坏直接影响到信息系统开发的成败。创建数据库表首先确定实体的属性和实体之间的关系。根据关系创建一个数据表。

[4.3.2数据库设计](#_Toc273815986)

(1)系统的E-R图

概念模型是数据库设计的强大工具。数据库概念模型设计可以通过E-R图描述现实世界的概念模型。系统的E-R图显示了系统中实体之间的链接。 

(2)实体属性图

费用信息的实体图如图4-3。

![](/md/blog.014.png)

图4-3费用信息实体图

车位信息实体图如图4-4。

![](/md/blog.015.png)

图4-4车位信息实体图

报告信息实体图如图4-5。

![](/md/blog.016.png)

图4-5报告信息实体图
### 4.3.3 数据库表设计
数据库的表信息属于设计的一部分，下面介绍数据库中的各个表的详细信息。

表4-1 allusers表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|username|varchar|50|` `default NULL|
|pwd|varchar|50|` `default NULL|
|cx|varchar|50|` `default NULL|

表4-2：baogaoxinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|` `int|11|NOT NULL |
|addtime|varchar|50|default NULL|
|mingcheng|varchar|50|default NULL|
|riqi|varchar|50|default NULL|
|baogaoneirong|varchar|50|default NULL|
|yonghuming|varchar|50|default NULL|
|xingming|varchar|50|default NULL|
|sfsh|varchar|50|default NULL|
|shhf|varchar|50|default NULL|
表4-3：cheweixinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|ID|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|mingcheng|varchar|50|default NULL|
|yuancheweihao|varchar|50|default NULL|
|chepai|varchar|50|default NULL|
|yonghuming|varchar|50|default NULL|
|xingming|varchar|50|default NULL|
|huancheweihao|varchar|50|default NULL|
|sfsh|varchar|50|default NULL|
|shhf|varchar|50|default NULL|
表4-4：fangkedengji表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|mingcheng|varchar|2|default NULL|
|riqi|varchar|50|default NULL|
|fangkexingming|varchar|50|default NULL|
|xingbie|varchar|50|default NULL|
|nianling|varchar|255|default NULL|
|zhiye|varchar|255|default NULL|
|zhuzhi|varchar|255|default NULL|
|wendu|varchar|255|default NULL|
表4-5：feiyongxinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|mingcheng|varchar|255|default NULL|
|riqi|varchar|50|default NULL|
|shuifei|varchar|50|default NULL|
|dianfei|varchar|50|default NULL|
|wuyefei|varchar|50|default NULL|
|cheweifei|varchar|50|default NULL|
|qitafeiyong|varchar|50|default NULL|
|zongfeiyong|varchar|50|default NULL|
|yonghuming|varchar|50|default NULL|
|xingming|varchar|50|default NULL|
表4-6：gonggaoxinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|biaoti|varchar|50|default NULL|
|gonggaoneirong|varchar|50|default NULL|
|riqi|varchar|50|default NULL|
表4-7：tousuxinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|mingcheng|varchar|50|default NULL|
|riqi|varchar|50|default NULL|
|tousuneirong|varchar|50|default NULL|
|yonghuming|varchar|50|default NULL|
|xingming|varchar|50|default NULL|
|sfsh|varchar|10|default NULL|
|shhf|varchar|200|default NULL|
# `      `5系统界面实现
## 5.1管理员功能模块
管理员登录，管理员通过输入用户名，密码，权限，等信息进入疫情防控物业管理系统，如图5-1所示。

![](/md/blog.017.png)

图5-1管理员登录界面图

管理员登录进入疫情防控物业管理系统可以查看首页、个人中心、业主管理、车位信息管理、费用信息管理 、报告信息管理 、核酸检测管理、访客登记管理、投诉信息管理、公告信息管理、公告回复管理等内容，如图5-2所示。

![](/md/blog.018.png)

图5-2管理员功能界面图

业主管理，在业主管理页面可以查看用户名、密码、姓名、性别、头像、身份证等内容，并可根据需要进行修改，删除或查看详细内容等操作，如图5-3所示。

![](/md/blog.019.png)图5-3业主管理界面图

费用信息管理，在费用信息管理页面可以查看名称、日期、水费、电费、物业费、车位费等内容，并可根据需要对费用信息管理进行修改，删除或查看详细内容等操作，如图5-4所示。

![](/md/blog.020.png)图5-4费用信息管理界面图

报告信息管理，在报告信息管理页面可以查看名称、日期、报告内容、用户名等内容，并可根据需要对报告信息管理信息进行修改，删除或查看详细内容等操作，如图5-5所示。

![](/md/blog.021.png)

图5-5报告信息管理界面图

核酸检测管理，在核酸检测管理页面可以查看名称、检测日期、检测情况、检测程度等内容，并可根据需要对核酸检测管理信息进行修改，删除或查看详细内容等操作，如图5-6所示。

![](/md/blog.022.png)

图5-6核酸检测管理界面图

投诉信息管理，在投诉信息管理页面可以查看名称、日期、投诉内容、用户名、姓名等内容，并可根据需要对投诉信息管理信息进行修改，删除或查看详细内容等操作，如图5-7所示。

![](/md/blog.023.png)

图5-7投诉信息管理界面图

公告回复管理，在公告回复管理页面可以查看标题、发布内容、发布日期等内容，并可根据需要对公告回复管理信息进行修改，删除或查看详细内容等操作，如图5-8所示。

![](/md/blog.024.png)

图5-8公告回复管理界面图

访客登记管理，在访客登记管理页面可以查看名称、日期、访客姓名、性别、年龄、职业等内容，并可根据需要对访客登记管理信息进行修改，删除或查看详细内容等操作，如图5-9所示。

![](/md/blog.025.png)

图5-9访客登记管理界面图





## 5.2业主功能模块
业主登录，业主通过输入用户名，密码，权限，等信息进入疫情防控物业管理系统，如图5-10所示。

![](/md/blog.026.png)

图5-10业主登录界面图

业主登录进入疫情防控物业管理系统可以查看首页、个人中心、车位信息管理、费用信息管理 、报告信息管理 、核酸检测管理、投诉信息管理、公告信息管理、公告回复管理、隔离状态管理等功能。如图5-11所示。

![](/md/blog.027.png)图5-11业主功能界面图

车位信息管理，在车位信息管理页面可以通过填写名称、换车位号、车牌、用户名、姓名等详细的车位信息管理等内容进行查看等操作，如图5-12所示。

![](/md/blog.028.png)图5-12车位信息管理界面图




`    `报告信息管理，在报告信息管理可以查看名称、日期、报告内容、用户名、姓名等内容，并可根据需要对报告信息管理查看详细内容等操作，如图5-13所示。

![](/md/blog.029.png)

图5-13报告信息管理界面图

核酸检测管理，在核酸检测管理页面可以查看名称、检测日期、检测情况、检测报告等详细核酸检测管理，如图5-14所示。

![](/md/blog.030.png)

图5-14核酸检测管理界面图

投诉信息管理，在投诉信息管理页面可以查看名称、日期、投诉内容、用户名、姓名等详细投诉信息管理，如图5-15所示。

![](/md/blog.031.png)

图5-15投诉信息管理界面图

公告信息管理，在公告信息管理页面可以查看标题、公告内容、日期等详细公告信息管理，如图5-16所示。

![](/md/blog.032.png)

图5-16公告信息管理界面图














