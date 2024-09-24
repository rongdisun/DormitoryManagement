# 基于Python的Django框架实现的学生宿舍管理系统

## 1、技术栈

- python==3.10
- django==4.2.6
- sqlite
- bootstrap4
- jquery3

## 2、系统概述

本系统使用pycharm进行开发，开发过程中使用了一些好用的插件，表单插件crispy_forms，该插件可以帮我们快速的生成表单，不用在一个个写前端form，极大的提高开发效率。在数据库选择方面使用了sqlite3，该数据库方便项目迁移，如果项目改成mysql只需要更改项目配置即可，其他都不需要动。

角色分为三种：管理员、宿管、学生。管理员主要功能是用户管理、宿舍楼管理、分配管理、公告管理等；宿管主要功能：宿舍检查、来访者登记、晚归学生登记、维修管理；学生功能：申请报修。

在删除的过程中，使用弹窗的技术，让操作者进一步确认。

## 3、功能简介

### 用户管理

**使用inlineformset_factory来实现**

![image-20240923230425818](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923230425818.png)

**用户列表，实现分页和搜索**

![image-20240923230734713](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923230734713.png)

### 楼宇管理

**添加楼宇**

![image-20240923230839984](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923230839984.png)

**楼宇列表**

![image-20240923230909047](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923230909047.png)

**弹窗实现删除的确认**

![image-20240923230953765](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923230953765.png)

### 分配管理

**分配宿管，报错提示**

![image-20240923231059258](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923231059258.png)

**学生宿舍列表**

![image-20240923231128659](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923231128659.png)

### 公告管理

**只用当登录的用户为管理员的时候，才会显示编辑和删除按钮**

![image-20240923231216923](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923231216923.png)

### 学生离校管理

**管理员可主动添加学生离校信息**

![image-20240923231507074](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923231507074.png)

**离校纪录列表**

![image-20240923231535146](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923231535146.png)

### 宿舍检查管理

![image-20240923231635464](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923231635464.png)

### 报修管理

![image-20240923231715898](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923231715898.png)

### 添加报修

**学生端添加报修**

![image-20240923231805674](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923231805674.png)

**记录报修的记录和时间**

![image-20240923231902354](https://raw.githubusercontent.com/rongdisun/learn/main/image-20240923231902354.png)