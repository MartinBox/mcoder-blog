---
title: Java常用命令
date: 2019-05-08 17:13:10
tags:
---

### 监测垃圾回收情况
`jstat -gcutil -h10 <pid> 3s 1000`

### 启动并查看日志
`bin/startup.sh ; tail -f logs/catalina.out`

### 关闭匹配关键字的进程
`kill -9 $(ps aux |grep online | grep java | awk '{print $2}') `
