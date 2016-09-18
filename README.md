# asLockApp

安卓应用锁

### 开发配置
本应用是在Android Studio 2.1.3上面开发的。

使用的JDK版本是 jdk1.8.0_51。

安卓版本：
最低要求是：minSdkVersion 14
目标版本为：targetSdkVersion 23

关于各个分支的介绍：目前有三个分支，

1、master只实现了最核心的锁定功能。没有设置，只能选择程序锁定。

2、ActionBar大家不用看，是我想实现一个侧滑栏，不过完成度不高，后面没有继续跟进

3、framelayout这个版本，名字没取好，反而是这个版本实现了ActionBar的基本框架。设置界面的框架也搭出来了。

同时这个版本采用的Broadcast唤醒LockService服务。只需稍作改动就能完成开机自启动等其他重要功能。

### 2016.1.25 更新

加入了更改密码以及绑定邮箱等功能。
同时，对这个项目的机构有了更深入的认识，有了一些重构代码的想法。预计在后面的一个礼拜进行代码的重构。

### 截止2016.9.11 更新
根据《APP研发录》的一些设计重构了部分代码，将一些全局性的变量放到Application类里面。
修复了遇到的所有的bug，算是一个稳定能用的版本。欢迎大家发现bug，一起改进。

### 截止2016.9.18 更新
尝试使用MVP模式对项目进行重构，当前只完成了主界面的重构，算是实现了面向接口编程。
使得项目各模块之间的耦合度降低。方便后期进行模块的更新

### 后续工作

后续工作应该放在优化界面，增加界面美观度上面。想要增加账号系统和换肤功能。


### 参考资料
关于应用锁的实现可以参考我的博客：

[安卓开发之应用锁](http://blog.csdn.net/include_u/article/details/49889791)

[应用锁之获取栈顶Activity](http://blog.csdn.net/include_u/article/details/50558130)