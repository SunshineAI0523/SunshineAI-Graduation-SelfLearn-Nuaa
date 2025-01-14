---
time: 2023-12-30 13:00:00
category: 项目 
tag:
    - 南京航空航天大学
    - 毕业设计
---
# Project Name - 项目名称
南京航空航天大学继续教育学院自学考试本科阶段毕业设计    
## Description - 描述
南京航空航天大学自学考试本科阶段毕业设计 
## Introduction - 介绍
创建南京航空航天大学继续教育学院自学考试本科阶段毕业设计这个项目是希望可以记录一下自己论文撰写和软件编程学习的过程，同时作为毕业设计相关文件夹的一个备份。
## Requirements - 必要条件（环境，对所有项目，和所有子模块和库的描述。）
Rocky Linux 9.x；
Nginx 1.24.1；
MySQL 8.x/MariaDB 10.11.x；
jdk 17；
## Configuration - 配置（配置信息。2）
SSH Port 22;
Nginx Port 80;
MySQL Port 3306;
Cockpit Port 9090;
## Installation - 安装（如何安装。）
前端：
1. 安装Node.js；
2. 进入项目目录；
3. 执行npm install；
4. 执行npm run build；
5. 将前端项目根目录中的dist文件夹中的内容拷贝至nginx网站根目录；
后端：
1. 安装MySQL；
2. 安装jdk；
3. 修改数据库配置文件；
4. 修改后端项目配置文件；
5. 执行mvn clean install；
6. 执行java -jar target/xxx.jar；
7. 访问后端项目接口；
## Usage - 用法（用法。）
使用浏览器直接登录服务器IP即可
如使用特殊端口，则需要使用IP:端口进行访问
## Changelog - 更新日志（一个简短的历史记录（更改，替换或者其他）。）

## FAQ - 常见问题（常见问题。）

## Support - 支持

### Dos - 文档（更多文档。）

## Authors and acknowledgment - 贡献者和感谢（作者列表和鸣谢。）
Author: Matrix0523
## License - 版权信息（版权和许可信息（或阅读许可证）、法律声明。）
MIT License

Copyright (c) 2023 Matrix0523

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.