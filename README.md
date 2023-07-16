# 数据库课程设计——企业人事管理系统（详细内容见报告）
数据库课程设计
### 业务流程图
![image](https://github.com/thisisbaiy/-Enterprise_Personnel_Management_System/assets/96861449/2a37ae48-d1a8-4921-99b4-aa74c91decd6)

报告目录

[1 设计目的与要求... 3](#_Toc139471062)

[1.1 设计目的... 3](#_Toc139471063)

[1.2 设计要求... 3](#_Toc139471064)

[2 设计内容... 4](#_Toc139471065)

[3 需求分析... 4](#_Toc139471066)

[3.1 用户需求... 4](#_Toc139471067)

[3.2 功能模块分析... 6](#_Toc139471068)

[3.3 功能模块划分... 7](#_Toc139471069)

[3.4 数据流图... 7](#_Toc139471070)

[4 概念结构设计... 12](#_Toc139471071)

[4.1 涉及的实体... 12](#_Toc139471072)

[4.2 实体之间的关系... 12](#_Toc139471073)

[4.3 实体应该具有的属性... 13](#_Toc139471074)

[4.4 ER图绘制... 15](#_Toc139471075)

[5 逻辑结构设计与物理结构设计... 16](#_Toc139471076)

[5.1 关系模型设计... 16](#_Toc139471077)

[5.2 关系模式规范化... 17](#_Toc139471078)

[5.3 外模式(视图)设计... 17](#_Toc139471079)

[5.4 权限控制... 18](#_Toc139471080)

[5.5 数据完整性的考虑... 19](#_Toc139471081)

[6 代码编写与具体实现... 20](#_Toc139471082)

[6.1 实现环境... 20](#_Toc139471083)

[6.2 主要的业务流程... 22](#_Toc139471084)

[6.3 安全性的考虑... 22](#_Toc139471085)

[6.4 后端代码的性能考量... 24](#_Toc139471086)

[6.5 前端页面使用的框架... 26](#_Toc139471087)

[6.6 测试工作... 27](#_Toc139471088)

[7 实际运行效果展示... 28](#_Toc139471089)

[7.1 前端页面模块展示... 28](#_Toc139471090)

[7.2 部分功能展示... 33](#_Toc139471091)

[8 遇到的问题与解决办法... 39](#_Toc139471092)

[8.1 问题一——MySQL DROP表卡死... 39](#_Toc139471093)

[8.2 问题二——事务提交... 40](#_Toc139471094)

[8.3 问题三——删除一周钱的考勤记录问题... 43](#_Toc139471095)

[总结... 44](#_Toc139471096)


---- 
### 设计要求：
完成一个基本的人事管理系统，该管理系统需要涉及：员工基本信息、岗位系统、员工岗位变动、员工考勤信息、部门信息、学历信息、员工薪资及变动信息、员工培训信息等相关实体。同时从以下几个方面着重考虑：

[1]      需求分析（课题组成员通力合作，力求需求分析的全面、有效！）

[2]      数据库设计（数据涵盖系统的数据需求，关系模式均达到3NF，性能优化自己思考）

[3]      数据完整性（分析关键表中的关键数据，制定自己的完整性约束规则！）

[4]      安全性（必须具有基本的用户及其权限的控制手段！）

[5]      视图（从操作的方便性、数据的安全性、数据的逻辑独立性等方面综合考虑！）

[6]      触发器（根据对应用的理解，是否采用触发器？带来的好处？）

[7]      存储过程（在充分理解系统业务处理的前提下，作出自己的判断，要运用得当！）

[8]      索引（需结合数据量的估算、应用的特点等，做出合理的设计）

[9]      系统功能（在需求分析的基础上尽可能全面一些！）

[10]  用户界面友好性（多从用户的角度考虑！）
### 实际开发环境
Tomcat8.0.50
Intellij IDEA2020.2


### 大致功能模块划分
![image](https://github.com/thisisbaiy/-Enterprise_Personnel_Management_System/assets/96861449/f95753fe-f4ef-49fa-b671-c27feb3b393d)

### 部分数据流图(详细内容见报告)
![image](https://github.com/thisisbaiy/-Enterprise_Personnel_Management_System/assets/96861449/77e6b028-f0cc-4ad1-b485-44ab41a84b4d)

### ER图绘制
![image](https://github.com/thisisbaiy/-Enterprise_Personnel_Management_System/assets/96861449/b4a71300-af38-4390-8faf-9f7df7933e05)

### 管理员界面
![image](https://github.com/thisisbaiy/-Enterprise_Personnel_Management_System/assets/96861449/329e5999-b60b-4886-9636-993d0347ee5a)

### 普通员工界面
![image](https://github.com/thisisbaiy/-Enterprise_Personnel_Management_System/assets/96861449/2630efad-329c-4063-97eb-c55fdad7e4a3)


