# MvpDaggerRetrofit
this is a demo used by MVP,Dagger,Retrofit.

#### 项目说明
1. 项目使用`mvp`模式，结合`dagger`和`retrofit`,使得项目架构更加清新，松耦合的设计对于后期维护改动有非常大的好处。
2. 可以看到使用该模式后，项目中比平常正常逻辑多了很多代码，但是可以知道这些代码都是基于接口设计的。
基于接口编程的好处也毋庸置疑，所以前期这些代码的编写是值得的。
3. 一个清晰的框架可以使项目开发维护成本降低，新加入的项目成员能快速上手。
4. **这只是一个Demo**，并不是一个框架，只是为了显示如何去融合目前比较流行的框架结合使用。

#### 功能说明
1. `MainActivity`也就是程序进入的第一个界面。只是简单的使用Dagger2来传递获取数据, 通过点击`click`按钮,将输入在
输入框中的文字显示在上面的TextView中。因为Dagger2是本程序的重难点,故做了这个简单的Dagger2实例。
2. `LoginActivity`是点击MainActivity的Click跳转进入的界面。该界面主要展示两种不同获取数据的方式,<p/>
    + 本类处理逻辑是按照`Mvp+Dagger2+Retrofit`处理。(这节才是**重点**)
    + `regiter`按钮是通过`retrofit`网络框架获取gitHub上对应用户名的信息。
    + `login`按钮是调用获取其他Module中定义的数据,演示传递数据。
