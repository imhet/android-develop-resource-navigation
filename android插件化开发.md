# android插件化开发资源


## 类库

### 插件化


|  类库       |    功能  | 说明 |
| ------------- | :-----:| :---- | 
|[DroidPlugin](https://github.com/Qihoo360/DroidPlugin)|插件|360，无安装情况下运行第三方APK|
|[dynamic-load-apk](https://github.com/singwhatiwanna/dynamic-load-apk)| 插件|百度，代理activity |
|[Direct-Load-apk](https://github.com/melbcat/Direct-Load-apk)|插件| 对dynamic-load-apk进行了改进，很久没更新|
|[Small](https://github.com/wequick/Small)| 插件| 跨平台 |
|[android-pluginmgr](https://github.com/houkx/android-pluginmgr)| 插件| 更新勤，貌似成熟 |
|[Android-Plugin-Framework](https://github.com/limpoxe/Android-Plugin-Framework)|插件| 说明很详细，近期有更新 |
|[ACDD](https://github.com/bunnyblue/ACDD)| 插件| 淘宝Atlas开源版，基于OSGI，近期有更新 |
|[DynamicAPK](https://github.com/CtripMobile/DynamicAPK) |插件|携程，支持hotfix，apk形式，不支持so|
|[AndroidDynamicLoader](https://github.com/mmin18/AndroidDynamicLoader)| 插件| 大众点评，基于Fragment+Scheme |


### 热修复

|  类库       |   功能  | 说明 |
| ------------- | :-----:| :----| 
| [dexposed](https://github.com/alibaba/dexposed) |热修复|阿里出品，基于[Xposed](https://github.com/rovo89/Xposed) AOP，补丁麻烦|
| [AndFix](https://github.com/alibaba/AndFix)|热修复| 阿里出品，支持2.3到6.0，无需重启  |
| [Nuwa](https://github.com/jasonross/Nuwa)|热修复| 基于MultipleDex，纯java，2.3-6.0，需重启  |
| [HotFix](https://github.com/dodola/HotFix)|热修复|基于MultipleDex，javassist动态注入，2.3-6.0，需重启  |
| [DroidFix](https://github.com/bunnyblue/DroidFix)|热修复 |基于MultipleDex，2.3-6.0，需重启  |
| [XLog](https://github.com/promeG/XLog)|   基于注解的log |   基于dexposed  |
| [hugo](https://github.com/JakeWharton/hugo)|  基于注解的log |     |


## 文章


### 插件化


- [Android apk动态加载机制的研究](http://blog.csdn.net/singwhatiwanna/article/details/22597587)
- [携程Android App插件化和动态加载实践](http://mp.weixin.qq.com/s?__biz=MzAwMTcwNTE0NA==&mid=400217391&idx=1&sn=86181541ce0164156dfab135ed99bb5c&scene=0&key=b410d3164f5f798e61a5d4afb759fa38371c8b119384c6163a30c28163b4d4d5f59399f2400800ec842f1d0e0ffb84af&ascene=0&uin=MjExMjQ&pass_ticket=Nt5Jaa28jjFxcQO9o+vQiXX+0iXG5DlZlHNW97Fk1Ew=)
- [DynamicLoadApk 源码解析](http://codekk.com/open-source-project-analysis/detail/Android/FFish/DynamicLoadApk%20%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90)
- [Small插件FAQ](https://github.com/wequick/Small/wiki/Android-faq) 对各种插件方法进行了优缺点比较


### 动态加载jar

- [Android动态加载外部jar文件](http://icyfox.com/2015/02/09/android-load-jar/)
- [Android用DexClassLoader实现动态调用jar包](http://blog.csdn.net/cheligeer1988/article/details/13774271)
- [Java ClassLoader基础及加载不同依赖 Jar 中的公共类](http://www.trinea.cn/android/java-loader-common-class/)
- [ android jar包插件化以及远程更新jar包思路](http://blog.csdn.net/xuduzhoud/article/details/17448871)



### 热修复

- [让App像Web一样发布新版本](http://bugly.qq.com/bbs/forum.php?mod=viewthread&tid=16)
- [安卓App热补丁动态修复技术介绍](http://zhuanlan.zhihu.com/p/20308548)
- [Android 热补丁动态修复框架小结](http://blog.csdn.net/lmj623565791/article/details/49883661)
- [各大热补丁方案分析和比较](http://blog.zhaiyifan.cn/2015/11/20/HotPatchCompare/)
- [Android HotFix方案](http://blog.hwangjr.com/2016/03/02/Android-HotFix%E6%96%B9%E6%A1%88/)
- [美团Android DEX自动拆包及动态加载简介](http://tech.meituan.com/mt-android-auto-split-dex.html)

## 产品

- [apkplug](http://www.apkplug.com/)	模块化框架 + 组件市场
- [UBSDK](http://news.bestsdk.com/detail/1312.html)


