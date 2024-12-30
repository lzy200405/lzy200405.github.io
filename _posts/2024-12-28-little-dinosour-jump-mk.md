---
layout: post
title: 小恐龙快跑
subtitle: C#程序
gh-repo: lzy200405/little_dinosaur_jump
gh-badge: [star, fork, follow]
tags: [C#]
comments: true
mathjax: true
author: Bill Smith
---
# 小恐龙快跑
这是一个基于经典 Chrome 离线小游戏“恐龙快跑”的 Windows 应用程序。该项目是为 Windows 程序设计课程的期末作业而开发，采用三层架构设计，并使用结构化数据库进行数据存储。

## 软件架构
小恐龙快跑采用三层架构，包括：

表示层（Presentation Layer）：负责用户界面的显示和用户交互。

业务逻辑层（Business Logic Layer）：处理应用程序的核心功能和业务逻辑。

数据访问层（Data Access Layer）：负责与数据库的交互，进行数据的存取操作。

这种架构提高了系统的可扩展性、可维护性和可重用性，使开发、测试和维护更加方便。

## 数据库设计
该项目使用结构化数据库来管理用户登录、注册、游戏得分和商店等功能。数据库包含三个数据表，分别用于存储不同类型的数据。项目中已提供表的创建 SQL 文件（little_dinosaur.sql）。

## 开发工具
项目开发使用的工具和框架包括：

集成开发环境（IDE）：Microsoft Visual Studio 2022

数据库管理系统：Microsoft SQL Server

实体框架（Entity Framework）：用于对象关系映射（ORM），所用版本如下：

Microsoft.EntityFrameworkCore.SqlServer：版本 8.0.5

Microsoft.EntityFrameworkCore.Design：版本 8.0.5

Microsoft.EntityFrameworkCore.Tools：版本 8.0.5

这些工具和框架的结合使用，提高了开发效率和应用程序的性能。

## 项目结构
项目的主要文件和文件夹包括：

Common/：通用功能模块

Model/：数据模型定义

lib/：外部库文件

little_dinosaur_jump.BLL/：业务逻辑层实现

little_dinosaur_jump.DAL/：数据访问层实现

little_dinosaur_jump/：表示层和主程序

.gitattributes：Git 属性配置文件

.gitignore：Git 忽略文件配置

README.md：项目说明文档

_config.yml：配置文件

little_dinosaur.sql：数据库表创建脚本

little_dinosaur_jump.sln：Visual Studio 解决方案文件

这种结构清晰地组织了项目的各个部分，便于开发和维护。

## 运行项目
要运行此项目，请按照以下步骤操作：

克隆仓库：使用以下命令将仓库克隆到本地：

bash
复制代码
git clone https://github.com/lzy200405/little_dinosaur_jump.git
设置数据库：

在 SQL Server 中执行 little_dinosaur.sql 脚本，以创建所需的数据库和表。

确保数据库连接字符串在项目的配置文件中正确设置，以便应用程序能够连接到数据库。

打开解决方案：使用 Visual Studio 2022 打开 little_dinosaur_jump.sln 解决方案文件。

还原 NuGet 包：在 Visual Studio 中，使用“还原 NuGet 包”功能，确保所需的依赖项已安装。

编译项目：在 Visual Studio 中构建解决方案，确保项目没有错误。

运行应用程序：在 Visual Studio 中运行调试或启动应用程序，即可开始体验小恐龙快跑游戏。

请确保您的开发环境满足上述工具和框架的要求，以顺利运行该项目。

如需更多信息，请访问项目的 GitHub 页面：

在此页面，您可以找到项目的源代码、文档和其他相关资源。
