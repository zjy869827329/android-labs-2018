第二次实验
-
实验要求
-
在Issues中创建自己的选题：https://github.com/hzuapps/android-labs-2018/issues ；
根据自选题目，编写一个或多个Activity（所有均带上学号前缀，放到自己的Java包下）；
将标题设置为自己的学号+对应的功能或题目；
根据自己选择的题目实现Activity中导航、调用等功能（选做）。
实验步骤
-
1. 阅读实验要求：https://github.com/hzuapps/android-labs-2018/labels/Lab   
2. 在电脑上Android Studio编写代码  
3. 使用Git将代码提交到自己的库中：https://github.com/YOUR_NAME/android-labs-2018   
$ git pull
$ git add 学号目录/*  (git rm 学号目录/*)
$ git commit "#12345678 "
$ git push

4. 在自己的GitHub库上创建和发送Pull Request（注意查看Changed files）  
5. 在GitHub中使用Markdown文件编写实验报告（report1.md, report2.md）  

实验提示
-
根据MVC、MVP设计模式或其他Android App设计模式设计Java类；
先设计表示业务数据的Java类，如表示订单、图书、商品、车辆、音乐、笔记等的类；
再考虑设计一些业务服务类，如网络连接等类；
上传代码时，代码放到自己的学号里面，同时保留Studio的目录结果，如：

app
- src
-- main
--- AndroidManifest.xml (第1个文件)
--- java
---- edu / hzuapps / androidlabs / Soft学号 / Soft学号Activity.java (第2个文件)
--- res 
---- layout
----- soft_学号_activity.xml (第3个文件)
---- values
----- strings.xml (第4个文件)

.实验结果
-
![在Android SDK Manager中选择6.0库](https://github.com/Zhengmianjie/android-labs-2018/blob/master/soft1614080902314/2%E8%BF%90%E8%A1%8C%E6%88%AA%E5%9B%BE.png?raw=true"配置教育网下载代理")

.实验体会
-
