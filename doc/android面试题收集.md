# Android面试题收集

## Java

### 基础

1. Java中为什么把String设计为一个常量，把StringBuilder和StringBuffer设置为变量 ？
2. final关键字如何使用的？
3. 线程之间如何同步？
4. ArrayList、LinkedList、Hashtable、HashMap、ConcurrentHashMap、HashSet的底层实现
5. 常用的线程池，这几种线程池之间有什么区别和联系，线程池的实现原理[^1]
6. Atomic、volatile、synchronized区别[^2]
7. Object类中的方法以及每个方法的作用
8. 假如有Thread1、Thread2、Thread3、Thread4四条线程分别统计C、D、E、F四个盘的大小，所有线程都统计完毕交给Thread5线程去做汇总，应当如何实现？
9. ArrayList和Vector的区别
10. 什么是多线程安全？
11. String、StringBuilder、StringBuffer、CharSequence 区别
12. 抽象类与接口的区别


### 进阶

1. Reader Thread怎么工作的
2. 注解原理
3. 反射原理
4. AOP实现
5. 写一个支持优先级的线程池
6. Threadlocal作用
7. ConcurrentHashMap，锁分段技术，迭代器是强一致性的迭代器还是弱一致性的迭代器，读是否要加锁

### JVM

1. Java虚拟机的内存布局
2. GC算法及几种垃圾收集器
3. 类加载机制，也就是双亲委派模型
4. Java内存模型
5. happens-before规则
6. volatile关键字使用规则
7. java编译过程



## Android

### 基础

1. Handler的设计初衷，原理，非主线程间如何使用Handler通信
2. 什么是序列化？ Serializable 和 Parcelable 区别是什么？ 为什么会有Parcelable存在？Android里面为什么要设计出Bundle而不是直接用Map结构
3. 能否new一个activity并启动它
4. view生命周期是什么5. 
5. 自定义动画里面的Matrix怎么控制
6. 各种launchermode使用场景
7. 动画原理，属性动画与之前动画有何不同，能否取代
8. android app的生命周期
9. content provider的生命周期
10. touch事件分发，能否用代码模拟一组touch事件（比如自动点击广告，自动滚动）
11. ART模式与Dalvk有何不同
12. 软引用虚引用弱引用区别，什么场景下使用它们
13. anr的三种类型
14. 纯代码实现res中资源功能，缩放点9图
15. 对activity/view/window的理解
16. view绘制流程
17. touch事件机制
18. binder的理解
19. Arraymap，Sparry与Hashmap关系，为什么建议用
20. applink实现原理
21. 防被杀，进程保活
22. 签名原理
23. AIDL是什么
24. [增量更新原理](http://blog.csdn.net/hmg25/article/details/8100896)
25. Scroll原理
26. Intentservice，Handlerthread，Atomfile
27. 推送心跳包是TCP包还是UDP包或者HTTP包 [^3]，具体实现 [^4]
28. ARGB_8888占用内存大小[^5]
29. 进程间通信（IPC）有哪些
30. JNI使用，[官方文档](https://developer.android.com/training/articles/perf-jni.html)
31. 如何做屏幕适配，有没有什么注意事项？
32. 继承viewGroup后必须实现哪些方法，这些方法有谁调用
33. 请介绍下ContentProvider是如何实现数据共享的
34. 介绍下AsyncTask的内部实现
35. Android开发中XML解析方式的比较及优缺点
36. 如何在不失真的条件下显示一张超高清的图片或者长图
37. 声明ViewHolder内部类时，为什么建议使用static关键字
38. AIDL设计体现了那些设计思想
39. android fragment和activity的区别
40. mipmap文件夹和drawable文件夹的区别
41. 怎么得到手机的唯一标识
42. View ViewRoot如何更新绘制界面的？


### 常用类库

开源项目解析[参考](http://www.codekk.com/)

1. Volley磁盘缓存,缓存命中率,缓存文件名的计算
2. ImageLoader
3. Fresco
4. EventBus
5. 你应用中的网络层是怎么设计的？


### 优化

参考google官方出的视频及国内[翻译教程](http://hukai.me/)。

1. 内存优化
2. 启动速度优化
3. layout优化
4. 卡顿优化
5. 体积优化
6. [sqlite优化](http://www.cnblogs.com/devinzhang/archive/2012/01/16/2323949.html)
7. listView的优化方式
8. 耗电量优化
9. [内存泄露的一些场景](http://jiajixin.cn/2015/01/06/memory_leak/)


### 框架层

1. 打包apk过程
2. 安装apk过程
3. 启动apk过程
4. android系统开机启动过程
5. activity视图层次是什么，打开一个对话框它是如何添加到视图上的
6. Dialog、PopupWindwo、WindowManager加载视图区别
7. ServiceManger ActiviyManager XXManager 是干什么的
8. [binder的理解](http://blog.csdn.net/luoshengyang/article/details/6618363)，除了binder外还能怎么跟service交互
9. root原理是什么，系统怎么管理app的权限
10. 谈谈你对Android中Context的理解 [^6]
11. Android中进程间通信有哪些实现方式？Intent，Binder（AIDL），Messenger，BroadcastReceiver


### 新技术

1. DexLoader
2. MVC，MVP，MVVM [^7]
3. React Native
4. RxJava
5. 插件原理
6. 热更新原理
7. fresco为什么省内存
8. data bindding
9. 65535问题与分包实践
10. 换肤原理
11. android开发中何时使用多进程，如何使用，如何通信
12. Recycleview、百分比布局、Gridlayout、Toolbar等MetrialDesign控件
13. 架构的定义

### 安全

1. 官方文档 https://developer.android.com/training/articles/security-tips.html?hl=zh-cn
2. 对称加密和非对称加密
3. Android Webview安全交互
4. [BroadCastReceiver安全](http://blog.csdn.net/yuanzeyao/article/details/38948863)



## 项目

1. 项目中遇到最大的困难时什么，怎么解决的
2. 觉得自己在哪方面的技术比较厉害

## 计算机基础

1. https的s是指什么
2. spdy使用过么
3. 数据库中事务是什么，union和union all，各种join，几种索引及其区别



## 数据结构算法

算法资料[1](http://blog.csdn.net/v_JULY_v),[2](https://github.com/pedrovgs/Algorithms)


1. 计算N的阶乘后面位数的个数及算法复杂度
2. 二分查找算法
3. 你知道索引使用的是哪种数据结构实现吗？为什么要用这种数据结构
4. Collections.sort方法使用的是哪种排序方法
5. 二叉查找树
6. 什么是平衡树，AVL树和红黑树的区别
7. 请用任意语言实现数据结构中的栈（可以包装一个LinkedList来实现）



## 设计模式

[常见设计模式的java实现](https://github.com/iluwatar/java-design-patterns)


1. 工作中常用的设计模式有哪些？如何使用的？该设计模式优缺点，画出该设计模式的UML图
2. 

## 逻辑题

[75道逻辑题](http://tieba.baidu.com/p/957651817)


## 其它

1. 为什么离开现在的公司
2. 你的技术优势是什么
3. 开发中遇到最难的问题是什么
4. 业余会做什么，有没发布过app，有没有参与过开源项目
5. 当前公司薪资待遇
6. 个人未来的发展方向
7. [自我介绍](http://www.zhihu.com/question/19603341)



[^1]:[40个Java多线程问题总结](http://www.cnblogs.com/xrq730/p/5060921.html)
[^2]:[并发编程之ThreadLocal、Volatile、synchronized、Atomic关键字扫盲](http://blog.csdn.net/u010687392/article/details/50549236)
[^3]:[Android推送技术研究](http://www.jianshu.com/p/584707554ed7)
[^4]: [android心跳包的分析](http://blog.csdn.net/wangliang198901/article/details/16542567)
[^5]: [你的 Bitmap 究竟占多大内存](http://bugly.qq.com/bbs/forum.php?mod=viewthread&tid=498)
[^6]:[你所不知道的Context](http://blog.csdn.net/qinjuning/article/details/7310620)
[^7]:[MVC，MVP 和 MVVM 的图示](http://www.ruanyifeng.com/blog/2015/02/mvcmvp_mvvm.html)





