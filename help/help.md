# 七鱼云客服使用说明

##	系统登录

###		云客服平台登录
七鱼云客服为您打造专属的后台登录地址，如http://xxxx.qiyukf.com/login 的二级域名，其中“xxxx”在企业注册时生成。登录网址、账号与密码在您申请成功后我们将以邮件的形式发给您，密码为6~16位的字母或数字，密码区分大小。
 ![七鱼登录页](./images/1.1.jpg)
您在注册时所用的邮箱是您的客服后台超级管理员账号，**请务必保管好账号及密码。**
###	目前所支持浏览器
目前七鱼客服工作台（即客服使用的后台）仅支持最新版谷歌chrome浏览器；用户访问端已兼容市面上主流浏览器。

##	渠道接入
###  PC端接入
####	Web对话窗口功能
PC端接入是指设置您企业网站的客服咨询入口，让您的访客可以及时得到客服的服务。咨询入口如下图所示：
  ![七鱼咨询入口](./images/2.1.1.png)
  
####	接入代码设置
在“设置”入口选择“网站接入”，可以查看PC端访客接入代码。详细文档可查看 [七鱼云客服 Web 开发指南](./Web_SDK_Guide.html) 。
此外，这里的“访客开关”默认为开启状态，使用户在访问您企业网站时可以看到客服咨询的入口，如您手动设置为“关闭”状态，用户则无法看到该入口。接入代码后，您可以根据您网站的视觉风格来设置对话框的样式、企业logo及访客见到的客服头像。

###	移动端接入
####	移动对话窗口功能
通过接入七鱼提供的SDK，您企业的APP上即可增加一个可自定义样式的客服咨询入口，访客点击该入口，即可直接向客服人员咨询。
  ![七鱼移动端SDK](./images/2.1.1.2.png)

#### 	接入代码设置
通过SDK设置，您可以快速地将客服咨询功能集成到您企业的APP中。您可以直接下载SDK，这里的APP Key是用于验证识别您企业APP应用的唯一标识序号。

iOS SDK接入说明，请见 [七鱼云客服 iOS 开发指南](../../sdk/_book/iOS_SDK_Guide.html)  ；

Android SDK接入说明，请见 [七鱼云客服 Android 开发指南](../../sdk/_book/Android_SDK_Guide.html)  ;

**需要注意的是，SDK包的大小会增加您企业APP的文件大小，Android接入后大概会增加不到500KB，iOS大概会增加2~3MB的大小。**

### 	微信公众号接入
#### 	微信对话窗口功能
七鱼云客服提供接入微信公众平台的功能，您企业公众号绑定授权后，访客在公众号发送的任何信息，都能直接在客服会话列表中显示出来，客服人员即可直接与访客展开会话。
<!--    ![七鱼微信接入](./images/2.2.1.jpg) -->

<img src="./images/2.2.1.jpg" style="width:200px">

####	微信接入授权
在“设置”入口选择“微信接入”，点击“去微信平台绑定授权”，登录公众号并授权给七鱼云客服。需要注意的是，您的微信公众号必须是经过认证的订阅号或服务号，否则无法正常回复访客对话。
您在微信上完成授权后，可以回到七鱼云客服的页面查看绑定结果。

## 	功能设置
### 	客服添加与管理
点击导航条上的“客服管理”，进入客服列表，页面的整体布局如下图所示：
   ![客服管理](./images/3.1.png)
点击页面右上角“新增客服”按钮即可进行添加客服的操作。完善相应的信息。**注意：1.每位客服可以设定个性化昵称；2.可以设定每个客服的最大接待人数，系统默认10人。**

角色的权限：
1.	超级管理员：企业注册开通时创建，帐号唯一，可以创建管理员和客服。
2.	管理员：由超级管理员创建，帐号不唯一，可以创建客服，同级管理员之间不可操作。
3.	普通客服：由超级管理员和管理员创建，帐号不唯一。

### 	设置欢迎语
在“设置”模块的“基础设置”中，您可以设置相应的个人信息以及设置欢迎语，欢迎语即为访客进入后自动响应的第一句话。
  ![设置欢迎语](./images/3.2.png)
  
### 	设置咨询分类
在基础设置中，您还可以进行咨询分类设置，七鱼云客服系统支持创建两级分类，后续可支持多级分类。
  ![设置咨询分类](./images/3.3.png)


##	客服工作台使用

### 	智能会话分配
七鱼云客服为您提供了智能的会话分配方案，即当某访客进行客服咨询时，会优先分配给上次接待他的客服人员，这样也能确保更快速、更到位地为访客提供服务。若该访客此前未被任何客服人员接待，则按照数量平均分配原则，随机分配给某位客服人员。

### 	设置状态
客服人员在客服工作台的页面右上角，可以进行状态设置，目前可供选择的状态为“在线”或“挂起”，后续将开放自定义状态设置。
   ![设置状态](./images/4.2.png)
客服人员需要小休，选择“挂起”状态时，将不会再接入新的访客咨询。

### 	会话咨询
当客服人员进入到“当前会话窗口”时，相关页面布局及功能如下图所示：
   ![会话咨询](./images/4.3.png)
在用户资料处显示客户信息，包括：地址信息、发起终端（pc、移动端还是微信）、发起咨询所在的页面。七鱼云客服平台开放API接口，可以接入您企业的CRM系统，若接入成功，则客服人员可以通过“更多详情”查看用户的订单、账号等信息。

在咨询分类中可以添加备注，并记录访客设备信息，通过记录设备信息把历史会话整合到同一个客户资料中。

### 	客服个人信息管理
在“设置”页面中，客服人员可以设置自己的手机号和新密码。而账号、姓名、昵称的设置权限仅开放给管理员，客服人员不具备相应权限。
说明：姓名是企业管理的员工真实姓名，昵称是客服对外接待客户的名字。






##	数据报表及业务管理

### 	实时客服在线管理
在七鱼云客服工作台主页，您可以实时监控企业当前的咨询人数、在线客服人数、访客排队情况以及各个时段的会话数接待情况。
    ![实时监控坐席及当前排队情况](./images/5.1.png)

您还可以实时监控客服人员的工作情况，了解当日考勤及使用时间。
<!--     ![今日客服活动](./images/5.1.1.png) -->

<img src="./images/5.1.1.png" style="width:500px">

### 	企业整体工作报表
七鱼提供了丰富的报表项目，可以查看企业某个时段的接待咨询数、未接待咨询数以及接待咨询总数，并可将相关数据导出到本地电脑上查看。
   	![会话报表](./images/5.1.2.png)
您还可以看到某个时段内，客服发出的消息数以及访客发出的消息数，从而获悉客服人员与客户的沟通状态。**注意：会话与消息的定义标准不同，一次会话可能包含多条客服和客户之间的消息。
此外，您可以通过以下数据了解企业的整体服务水平：**
   	![会话报表统计](./images/5.1.3.png)
也可以了解访客咨询问题的分类和占比信息。
    ![咨询分类](./images/5.1.4.png)

### 	单个客服工作报表
在“工作报表”的“客服”界面，您可以查看到每位客服人员的会话数、总消息数、响应时间等信息。
     ![客服报表](./images/5.3.png)
     
### 	历史会话记录查询
在“历史会话”界面中，可以直观地看到每次会话的详细信息，并可以通过各类筛选来查看列表会话的信息。点击进入某个会话，即可查看会话的历史详情。
    ![历史会话](./images/5.4.png)

##  工单中心
### 	工单中心介绍
七鱼1.1版本新增加工单中心功能，解决企业内部之间的工作协作问题。当企业客服无法立即解决用户的问题时，可以通过发起一个工单来请求企业内部的其他人员或部门（支持组）来协助解决完成。

七鱼1.1版本的工单中心需要通过申请或后续的付费购买来使用。

### 	工单客服及分组的设置

工单客服是新增的一个帐号角色，该角色只可对工单进行相关的操作，不可在线咨询接待访客。

分组主要是便于对企业的员工角色进行管理，可以是对客服部门内部进行分组管理，也可以针对企业内部进行分组管理。应用到工单中心场景，主要是创建工单时可以指定哪个分组来处理工单。

工单客服及分组可以通过管理后台的左侧导航“客服管理”进入后进行创建、修改。

#### 	创建工单客服
![创建工单客服](./images/6.2.1创建工单客服.jpg)

#### 	分组设置管理

![分组设置管理](./images/6.2.2分组设置管理.jpg)

### 	工单分类设置
工单分类主要是用来设置工单的问题分类，可以通过管理后台设置里进行创建工单分类

![6.3工单分类设置](./images/6.3工单分类设置.jpg)

### 	工单列表

进入工单中心会看到四个tab标签列表，分别为我受理的、我提交的、历史工单以及组内工单

* 我受理的工单：其他人创建并直接指派受理人为我的工单，或是我在组内工单中主动申领的工单

* 我提交的工单：我主动发起创建的工单

* 历史工单：我受理的工单被转交的、我受理的工单被完结的

* 组内工单：我所在的客服组接收到的工单

![6.4工单列表](./images/6.4工单列表.jpg)

### 	新建工单

如果帐号角色是工单客服，则可以进入工单中心里面进行新建工单；

如帐号角色是普通客服，则既可以在工单中心里创建也可以在当前会话页面的右侧用户信息页面点击新建工单。

新建工单需要填写工单标题、工单内容、工单分类、工单的受理组/人等信息。

创建成功后可以进入到“我提交的”tab标签列表中查看工单的状态。

![6.5新建工单](./images/6.5新建工单.jpg)

### 	申领工单

当帐号角色被加入到某个分组时，此时可以去组内工单池申领对应的工单进行处理。


![6.6申领工单](./images/6.6申领工单.jpg)

### 	处理工单

进入我受理的工单列表处理需要我跟进处理的工单；

进入我提及的工单列表查看工单问题的回复处理结果，并对回复处理结果进行跟进处理。

* 回复工单：工单受理人在接到需要处理的工单时，根据工单的问题描述进行协助查询解决，并给与反馈结果。

* 转交工单：工单受理人认为此工单的问题需要其他人来协作完成时，可以通过转交工单来进行操作。

* 完结工单：工单创建者在收到工单问题的处理结果时，如确认此问题已解决，可以对工单进行完结操作，表示此工单已解决。


![6.7处理工单](./images/6.7处理工单.jpg)

### 	搜索工单
七鱼的工单服务提供工单编号、工单标题、工单发起人、工单受理人、工单分类、工单创建时间等多维度的搜索条件进行查询工单。

![6.8搜索工单](./images/6.8搜索工单.jpg)

### 	工单规则说明
#### 	工单状态

我们的工单流转过程中的状态包含未申领、受理中、已完结三个状态；

工单创建者创建工单时选择受理组创建成功后，此工单状态为未申领，当所在的受理组有人申领工单后，此工单状态为受理中；

工单创建者创建工单时选择受理人创建成功后，此工单状态为受理中，受理中的工单在未完结时，始终处于受理中状态。

工单被标记为已完结时，此时工单状态为已完结，已完结的工单只可查看，不可进行回复、转交和完结等操作。

#### 	工单转交说明

工单处于受理中时，工单创建者认为此工单需要其他组/人处理，此时可以对工单进行转交操作。

工单处于受理中时，工单受理人认为此工单需要其他组/人协助处理，也可以将工单进行转交操作，同时当前受理人将不可再对工单进行回复、完结、转交操作。

##	客户留言  
### 	留言介绍
当企业没有一个客服在线时，客户可以通过留言的方式与企业保持联系，客户的留言将被收录进留言模块。

* 通过移动app或微信公众号留言的客户，客服可直接回复留言。回复内容将发送到客户移动app或微信中。

* 通过web留言的留言内容，客户可自行通过邮件或电话的方式回复客户。

<!-- ![7.1](./images/7.1.png) -->
<img src="./images/7.1.png" style="width:500px">

### 	留言设置
登录管理后台，在设置页面可以针对留言的引导文案以及留言需要填写的内容的信息进行设置。
![7.2](./images/7.2.png)

### 	留言列表
切换为客服工作台模式后，在当前会话列表下面增加留言列表，包含新留言以及历史留言信息。可对留言进行查看，来自移动端的留言可以直接回复用户。
![7.3](./images/7.3.png)

### 	留言统计
切换为客服工作台模式后，在当前会话列表下面增加留言列表，包含新留言以及历史留言信息。可对留言进行查看，来自移动端的留言可以直接回复用户。
![7.4.1](./images/7.4.1.png)
![7.4.2](./images/7.4.2.png)



##	会话邀请
### 	会话邀请功能介绍
七鱼1.1版本增加了会话邀请功能，当用户在访问你的企业网站时可以自动发出会话邀请，让你的企业不错过任何一个商机，七鱼1.1版本会话邀请服务主要为系统自动发送会话。

    
### 	设置会话邀请

* 入口：管理员登录到管理后台在设置页面，点击会话邀请标签，

* 开关设置：我们的会话邀请支持灵活的开关设置，即如你不需要使用时也可以进行关闭会话邀请功能

* 时间设置：通过时间设置可以灵活配置一个访客在访问你的企业网站多少秒后自动发送会话邀请

* 再次发送会话邀请设置：通过这里可以设置当访客拒绝邀请后再次自动发送会话设置的间隔时间

* 系统样式：可以设置会话邀请的文字，并可以根据自己配置的文字进行预览样式

![8.2设置会话邀请](./images/8.2设置会话邀请.jpg)

##	智能机器人

### 	智能机器人介绍
智能问答机器人是由网易自主研发、运用顶尖语义分析技术开发而成的服务于企业用户的一套智能问答系统，功能涵盖针对用户咨询问题进行智能回复、未知问题学习、机器人问答统计等功能。目前智能机器人支持网站接入、App接入及微信公众号接入。通过智能机器人能够极大的降低企业人力成本、提升服务效率。

### 	开启智能机器人
#### 	入口设置

* 如果企业想要使用智能问答机器人，需要先在七鱼客服平台管理模式中的设置—机器人选项中开启。

* 智能机器人支持网站接入、App接入及微信接入。企业可以根据自己的需求选择需要开启智能机器人的渠道。

<!-- ![9.2.1](./images/9.2.1.png) -->
<img src="./images/9.2.1.png" style="width:450px">

#### 	模式设置

开启智能机器人后，我们还提供使用人工客服和机器人模式及只开启机器人模式。

* 使用人工客服和机器人模式时，当遇到机器人无法回答的问题，访客可以从智能机器人无缝转接到人工客服

* 使用只开启机器人模式时，访客将始终和智能机器人对话，无法转接至人工客服

#### 	常驻人工客服设置

设置常驻人工客服入口

* 当开启后，访客可以在界面中直接转接至人工客服。

* 如果关闭则不出现转为人工按钮，但是访客仍然可以根据机器人的引导转接至人工客服。

![9.2.3](./images/9.2.3.png)

### 	机器人知识库
机器人知识库是智能机器人的大脑，如果想要机器人能够帮助你解决绝大多数访客问题，则需要在知识库中将访客可能会问的问题都添加进去。

![9.3](./images/9.3.png)

#### 	添加知识库问题
在知识库界面右上角点击“添加新问题”就可以给机器人知识库添加问题。

在使用之前，我们需要认识到机器人能够识别的问题范围与机器人知识库息息相关，机器人无法一开始就知道你的公司的业务问题，所以如果想让机器人能够解决访客的大多数问题，那么你需要将访客可能会问到的问题尽可能多的添加进机器人知识库。

下面将介绍知识库的使用方法及注意事项：

你可以在“知识库”面板下，点击右上角的“添加新问题”，系统功能界面如下图所示。

![9.3.1.1](./images/9.3.1.1.png)

用户可以添加一个问题的标准问法，如：“包邮吗”，并在标准答案中加入相应答案，如：“本店满299元以上全国包邮，满99元以上江浙沪包邮”。

答案中可进行超链接编辑。添加好问题后，选择问题的相应分类，点击“提交”，就完成了基本问题的创建。需要注意的是，问题的分类信息对于问题的管理以及日后的信息统计尤为重要，因此创建问题时，最好为每一个问题选择正确的分类。

![9.3.1.2](./images/9.3.1.2.png)

另外，针对同一个标准答案，客户的问法可能千差万别。比如在询问“包邮条件”问题时，客户实际问的可能是“满多少可以包邮”，也有可能是“怎样才能包邮”。这两种问法对应的都是“包邮条件”的标准答案。机器人存在学习过程，所以在添加完标准问题后，建议再输入几个相似问法，让机器人更快的学习，变得更智能。添加方法只需要在界面中间的相似问题框中输入相似问法，点击“添加相似问题”即可。

注意，问题的设置可遵循以下几个原则：

**标准问题应当采用意思完整、表述规范、简单的问句**，尽量设置为用户最可能的问法，且不要包含与问题无关的内容。

**例如：**

**例子1：**将修改密码的标准问题设置成“用户如何修改密码”，问句“改密码”意思不够完整，问句“密码怎么改”太过口语化、“修改密码的流程是什么”不够高频，另外，问句中尽量不要包含“你好”这类与问题无关的内容。

**例子2：**设置问题“亚马逊支持哪些支付方式”

正确例子：“亚马逊有哪些可用的支付方式”

错误例子：“支付方式”、“我该怎么支付”、“用户的支付方法”

**例子3：**设置问题“分期付款该如何操作”

正确例子：“分期付款的操作流程”

错误例子：“分期付款”、“怎么分期付款”

**例子4：**设置问题“满多少可以包邮”

正确例子：“包邮的条件”

错误例子：“包邮”、“怎样才能包邮”

**例子5：**设置问题“如何给账户充值”

正确例子：“账户充值如何办理”

错误例子：“充值”、“怎么充值”

**相似问题尽量包含多种语态，每个相似问题设置成差异化较大的表达。**注意，推荐将标准问题的核心关键词加入相似问题中。

**例如：**

（1）“退货如何办理”可以设置相似问题 “退货”、“退货流程”、“想退货怎么操作”等，其中“退货”是该问题的核心关键词，字面一样只是字的顺序不一样的问题，如“货怎么退”则不用加入相似问题，因为系统默认可以匹配；

（2）“数据安全如何保证”可以设置相似问题“数据安全”、“数据安全的策略”“泄露风险有多大”等；

（3）“如何给账户充值”可以设置相似问题“账户充值”、“账户充值怎么办理”、“账户余额不足怎么办”等；

（4）“如何查询账单查询”可以设置相似问题“账单查询”、“怎么查账单”、“想查账单怎么操作”；

（5）“发货时间”可以设置相似问题“多久可以发货”、“发货要多长时间”、“什么时候发货”。

#### 	问题学习

当遇到机器人无法回答的问题时，这些问题将会被收集到知识库中的问题学习模块中。 

管理员可以将这些问题作为新的问题快速添加到知识库中或者将问题作为相似问题关联到知识库的标准问题中。

如果遇到无意义的问题时，还可以将此问题忽略，忽略后此问题将不再出现在问题学习中（即使之后还有访客问此问题）。

![9.3.2](./images/9.3.2.png)

##	DemoApp使用指南

### 	DemoApp简介
七鱼DemoApp是七鱼云客服提供给用户及开发者的一个体验App，主要包含移动端客服界面和开发定制功能体验模块。用户在完成AppKey绑定后，可以通过Demo与对应企业七鱼云客服平台发起会话，完整体验七鱼移动SDK提供的多媒体消息收发、用户排队、离线留言、满意度评价等功能。同时支持轻量CRM接入、接口CRM接入、聊天窗口素材替换等开发者定制功能的体验。

### 	DemoApp下载

用户可以在七鱼官网演示Demo[下载页面](http://qiyukf.com/download#id=1)中，下载到最新版本的Android和iOS访客端DemoApp。

需注意的是，iOS9.0以上的系统，需要在“设置-通用-设备管理”中完成“七鱼客服Demo”信任操作。

开发者可以在 [七鱼云客服SDK开发指南](../../sdk/_book/index.html) 中下载到DemoApp的源码，便于在接入过程中参考。

### 	DemoApp使用说明
#### 	绑定企业Appkey
DemoApp本身自带了默认Demo企业的AppKey，可以直接与默认企业发起会话，体验七鱼云客服移动SDK所提供的功能。如果用户希望与自己企业的七鱼云客服平台建立会话，可以在DemoApp中完成与自己企业AppKey绑定，其中

（1）可以在“七鱼云客服平台管理端-设置-App接入”中找到企业对应的AppKey及二维码：
![AppKey二维码](./images/二维码.png)

（2）DemoApp支持扫码和手动输入两种方式完成AppKey绑定：
![AppKey绑定](./images/绑定AppKey.png)

#### 	体验发起会话
DemoApp模拟了一个互联网金融类App的界面，用户可以在首页、产品介绍页和设置页发起客服咨询：

![发起会话](./images/发起会话.png)

会话建立后，用户可以完整体验文字、语音、图片等多媒体消息的收发，以及用户排队、离线留言、满意度评价等功能。

#### 	个人信息上报
DemoApp在“设置-个人信息”中支持切换匿名与非匿名用户，非匿名状态下发起的会话，客服可以在当前会话右侧看到由应用上报的用户信息。企业可以根据需要将访客的姓名、手机号、最近订单号、收货地址等常用信息上报，客服在会话接入时即可对访客基本信息有所了解，减少了询问常用信息的时间，能够提升客服工作效率和访客的满意度。

<!-- **这是一张非匿名用户发起会话的截图** -->

七鱼云客服支持轻量级接入和接口接入两种个人信息接入方式，详细的接入文档和使用说明可以查看 [七鱼云客服企业信息对接开发指南](../../sdk/_book/qiyu_crm_interface.html) 。

#### 	切换窗口样式
七鱼云客服支持开发者自定义聊天窗口样式，其中包括窗口背景、字体颜色、气泡样式、通知banner样式、客服访客头像等素材的自定义，在DemoApp设置中选择切换窗口样式，可以查看自定义后的窗口样式。

![切换聊天窗口风格](./images/切换聊天窗口风格.png)