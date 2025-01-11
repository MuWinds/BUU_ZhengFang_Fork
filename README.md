# BUU北京联合大学 正方教务系统自动抢课助手

正方教务系统模拟登录，爬取信息，自动抓包发包抢课

*抢课需谨慎，记得看注意事项*

> 程序仅供交流学习，请勿用作非法用途

### 环境需求
1. python环境 ：Python3.5+

### 使用步骤

#### 1. release版本

1. 下载系统对应的release版本
2. 运行main可执行程序


#### 2. 使用源码运行
1. git clone源码
2. pip install -r requirements.txt
4. 运行源码中的main.py文件
5. 第一次运行先选择设置账号密码(之后运行直接选开始抢课,之前的账号密码会保存在account.json文件中)

### 注意事项
注意正方教务系统中进行计划内选课时，如果已有该课程，再次提交同样课程不同时间段的选课申请，有可能会删除你的已选课程 ,抢课之前请一定一定一定要确认一下你要抢的课(若课程被删了，我不负责哦)

### 可能存在的bug

1. windows上运行程序的时候最开始的提示会出现乱码(有什么3m31这样的字)，但事实上那不是乱码，是python带颜色的字，但是windows的终端不支持这个。
2. Macos上可能会出现zip包中的model文件找不到，如果提示没有在xxx路径找到这个model，那就把这个model文件从解压出来的地方移动到那里吧。

### 实现原理

[zucc正方教务系统抢课脚本](https://zghy.xyz/2020/05/21/zucc正方教务系统抢课脚本/#more)

之前修改计划内选课的时候顺便写的一个文档，从最开始的页面分析GET到抢课界面，到最后发送POST数据包进行抢课