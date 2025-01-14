
## 项目简介 / Project Introduction

中文：
本项目是一个基于 SpringBoot 和 Vue.js 开发的现代化房屋租赁管理系统。系统提供房源管理、租赁合同管理、租金收付、维修管理等功能，旨在为房东和租客提供便捷的租赁服务平台。

English:
This project is a modern house rental management system developed using SpringBoot and Vue.js. The system provides features such as property management, lease contract management, rent payment processing, and maintenance management, aiming to provide a convenient rental service platform for landlords and tenants.

## 开发环境 / Development Environment

### 服务器环境 / Server Environment
- Debian Linux 
- Nginx 1.24.1
- MySQL 8.x/MariaDB 10.11.x
- JDK 

### 开发工具 / Development Tools
- 后端 / Backend：
  - Spring Boot
  - Maven
  - MySQL/MariaDB
  
- 前端 / Frontend：
  - Vue.js
  - Node.js
  - npm

## 系统配置 / System Configuration

- SSH: 22
- Nginx: 80
- MySQL: 3306
- Cockpit: 9090

## 部署指南 / Deployment Guide

### 前端部署 / Frontend Deployment

中文：
1. 安装 Node.js 环境
2. 进入前端项目目录
3. 安装项目依赖：`npm install`
4. 构建生产环境代码：`npm run build`
5. 将 dist 目录下的文件部署到 Nginx

English:
1. Install Node.js environment
2. Navigate to frontend project directory
3. Install dependencies: `npm install`
4. Build for production: `npm run build`
5. Deploy dist directory files to Nginx

### 后端部署 / Backend Deployment

中文：
1. 安装 JDK 
2. 安装并配置 MySQL/MariaDB
3. 修改数据库连接配置
4. 编译项目：`mvn clean install`
5. 运行 JAR 文件：`java -jar target/xxx.jar`

English:
1. Install JDK 17
2. Install and configure MySQL/MariaDB
3. Modify database connection settings
4. Build project: `mvn clean install`
5. Run JAR file: `java -jar target/xxx.jar`

## 使用说明 / Usage Guide

中文：
1. 通过浏览器访问系统地址
2. 默认使用 80 端口访问
3. 如使用其他端口，需要在地址后添加端口号

English:
1. Access system through web browser
2. Default access through port 80
3. If using different port, add port number to address

## 作者 / Author

Matrix0523

## 许可证 / License

MIT License

Copyright (c) 2024 Matrix0523

[MIT License 完整内容请参见项目根目录的 LICENSE 文件 / For the full MIT License text, please see the LICENSE file in the project root directory]