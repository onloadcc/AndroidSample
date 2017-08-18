Android Sample 导入
==================

* 从仓库上查找需要版本的下载
<https://android.googlesource.com/platform/development.git/+/android-5.1.1_r37/samples/ApiDemos/>

* 导入 studio 后，根据错误提示更改


## 遇到异常

* `版本和下载版本需要对应`

* 提示文件添加 `.xml` 后缀

* 编译版本和下载的版本对应
~~~
compileSdkVersion 22
~~~

* 添加依赖 根据编译版本找对应版本
 ~~~
 dependencies {
     compile 'com.android.support:appcompat-v7:22.0.0'
     compile 'com.android.support:support-v4:22.0.0'
   }
 ~~~
 
* 添加版本号
~~~
    minSdkVersion 19
    targetSdkVersion 22
~~~

* 注释文件中依赖的 `com.google.android.mms`
