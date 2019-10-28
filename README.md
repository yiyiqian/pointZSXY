一点知识学院后台管理系统
==

扫码关注加微信，备注 一点知识学院，进群讨论。

![image](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/cxzc.jpg)

一点知识学院 是一个在线课程资料的管理系统（是对app手机端的支撑），项目采用SpringBoot +JPA+easyui开发。
项目地址：Github项目地址

https://github.com/ProceduralZC/pointZSXY.git
        
本来计划把项目跑起来放到网上供小伙伴们查看预览的，但是服务器有其他几个项目在运行，内存空间已经不足以起起来该项目了，因此小伙伴们只能看一下下面的截图了，本文结尾会有部署教程，部署到本地也可以查看完整效果。（如有需要：联系我，或者后续我录制部署启动视频）

前言
==
整个项目功能比较多，也比较复杂，因此分多期开发，目前基本功能已经全部做完，部分功能有待优化，其他模块还在规划当中。考虑到目前功能已经可以使用，同时里面的权限管理，菜单管理，用户管理，可以用于任何需求的项目中，权限管理又是许多同学的痛点，因此将本项目提前开源供小伙伴们研究。<br/> 

提供App端接口已经完成，app端的开发进行中。。。<br/> 

需要注意的是，因为考虑到用户权限模板是一个很独立的模板，所以单独分离出来，作为一个项目库来使用，所以有两个项目包，其中 system-core-college 作为库文件引入到 onepoint_college中使用。<br/> 

有需要的小伙伴可以拿来直接学习和使用，有任何问题可以查看说明。

那么适合什么人群使用和学习呢？
=
1，Java初学者，这个是一个很好的学习框架，让你学会整体流程<br/> 
2，Java有一定经验（大牛除外），但是之前做的工作一直是打下手，这个框架就比较适合了，可以让自己对框架更深的了解，也可以一直升级和优化<br/> 
3，大学生，还没有毕业就想了解一下Java 和通过一个项目更深入的了解Java的神奇，跑起来该项目，一定很有成就感。<br/> 
4，其他语言转Java语言的，直接拿来使用就好<br/> 

另外，本项目也在不断的更新中，小伙伴们可以通过关注公众号   程序职场  了解最新更新记录查看最新完成的功能。

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/cxzc.jpg)


邀请函
==
该项目还有一些功能需要完善，新的需求也在规划中，欢迎小伙伴们提出来好的建议，我会作为框架的升级项，会将大家所提的好建议展示在README中！


整体效果
==

1、系统菜单
--
（1）首先，不同的用户在登录成功之后，根据不同的角色，配置不同的菜单项，会看到不同的系统菜单，完整菜单如下：

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片1.jpg)

不同用户登录之后，看到的菜单项不同。

2、用户管理
--
（1）展示后台管理员信息，可以新增，删除，编辑 管理员信息，对不需要的用户可以：禁用，还可以做：启用，重置密码操作等


![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片2.jpg)

新增后台管理员用户，可以选择不同权限级别：超级管理员，一级管理员，二级管理员

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片3.jpg)

编辑管理员信息

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片4.jpg)


3、数据编辑
--
（1）用于维护项目中 固定数据 的展示和编辑，可以通过头部菜单：新增，编辑，删除

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片5.jpg)

4、版本升级
--
（1）为app端开发的 android端 版本的升级 ，可以新增，编辑和删除

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片6.jpg)

5、权限管理
--
（1）配置用户级别权限，可以给不同级别权限用户配置不同菜单，目前有：超级管理员，一级管理员，二级管理员

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片7.jpg)

6、菜单管理
--
（1）产品的项目菜单数据管理，可以根据不同项目的需求 新增，删除，编辑等

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片8.jpg)


7、知识类型
--
（1）app端的课程资源分类，目前规定四个主分类，知识课件，知识路径，精品系列知识，热门知识。可以新增，删除，编辑

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片9.jpg)

8、知识课件
--
（1）课程知识的知识课件分类，可以新增，编辑，删除 分类，同时可以添加子课时

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片10.jpg)

9、知识路径
--
（1）课程知识的知识路径分类，可以新增，编辑，删除 分类，同时可以添加子课时

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片11.jpg)

10、精品系列知识
--
（1）课程知识的精品系列知识分类，可以新增，编辑，删除 分类，同时可以添加子课时

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片12.jpg)

11、热门知识
--
（1）课程知识的热门知识分类，可以新增，编辑，删除 分类

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片13.jpg)

12、精选课程
--
（1）精选课程是最专业和最具代表意义的课程资源，可以添加子课时，功能包括，新增，删除，编辑。

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片14.jpg)

13、消息动态
--
（1）展示系统发布的一些系统消息，或者资源新增和变更消息等，用户app端展示，功能包括，新增，删除，修改。

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片15.jpg)

14、首页动态
--
（1）展示系统发布的一些系统消息，或者推荐视频，最好视频资源等，用户app端展示，功能包括，新增，删除，修改。

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片16.jpg)

15、意见反馈
--
（1）用来收集客户在app端使用中遇到的优化意见和反馈帮助意见等等。

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/图片17.jpg)

技术栈
==

后端技术栈
--
1.SpringBoot
2.jpa
3.MySQL

前端技术栈
--
1.easyui

还有其他一些琐碎的技术就不一一列举了，会以知识点的形式详细讲解。

项目部署
==

1.克隆(clone) 项目到本地: 克隆Github地址    https://github.com/ProceduralZC/pointZSXY.git <br/> 
2.数据库脚本放在onepoint_college 项目的src / main / webapp / file目录下，在MySQL中执行数据库脚本或者直接导入即可<br/> 
3.数据库配置在onepoint_college项目的resources目录下的application.properties文件中<br/> 
4.在eclipse中运行onepoint_college项目<br/> 
OK，到这里，服务端就启动成功了，此时我们直接在浏览器地址栏输入<br/> http://localhost:8080/onepoint_college/manager/home/login.html <br/> 
即可访问项目，如果要做二次开发，直接在基础上作调整就行，不受任何影响。

注意，注意，注意  对应的前端还在更新中，后面会陆续 开源 app，小程序，flutter等移动端源码。

文档
==
文档是对项目开发过程中遇到的一些问题的详细记录，主要是为了帮助没有基础的小伙伴快速理解这个项目。
该项目框架虽然已经基本完成，但是，但是，但是，开发中一些问题整理还欠缺，迫不及待的想要分享给大家，提前开源给大家使用，如果有疑问  添加公众号    程序职场    进群。

其他资料
==

关注公众号 程序职场 ，专注于 前端框架（flutter）app移动端，小程序， Spring Boot+微服务，定期文章分享，后续定期更新视频，关注后回复   Java资料  ，领取为你精心准备的干货！
一个执着的职场程序员

![Alt text](https://github.com/ProceduralZC/pointZSXY/raw/master/onepoint_college/image/cxzc.jpg)

[项目部署视频地址](https://github.com/ProceduralZC/pointZSXY.git)  
