# Getting Started Guides

### Install Linux
可以参考[Linux Setup](https://github.com/iamcoach/linux-setup/blob/master/Install.md)进行安装并配置，安装双系统一定注意，一不小心选错了就会把原来的系统格掉，结果很惨烈的，特别要重视，实在不放心请自行备份重要文件。


### Install IntelliJ IDEA Community Edition: 
可以到[官网下载](https://www.jetbrains.com/idea/download/#section=linux)并安装IntelliJ IDEA的社区版本，最终版功能更多，但需付费购买。

如果使用的是Ubuntu系统，安装完成后可以先禁用Ubuntu冲突的快捷键，然后可以进行一些常用配置。

**Here’s a list of tweaks you need to make with default system key bindings so that they won’t interfere with IntelliJ IDEA actions:**

- Disable the Shade window action, assigned to Ctrl + Alt + S (Settings dialog).
- Change or disable the Lock Screen action, assigned to Ctrl + Alt + L (Reformat code).
- Disable the Move window action, assigned to Alt + F7 (Find usages).
- Change or disable the Resize window action, assigned to Alt + F8 (Evaluate expression).
- Change or disabled the fcitx switch virtual board, assigned to Ctrl + Alt + B (go to implement).
- Change or disable Dashboard, assigned to Alt + F1 (Select Target) 
	- You can refer [How to Do It](http://askubuntu.com/questions/271386/how-to-prevent-alt-f1-from-selecting-dash). Also can try the command: `sudo apt-get install compizconfig-settings-manager compiz-plugins-extra -y`
- You can import the [Settings](assets/settings.jar) to IntelliJ if you like. Backup yours first.

Please refer to the [Keyboard Shortcuts You Cannot Miss](https://www.jetbrains.com/help/idea/2016.2/keyboard-shortcuts-you-cannot-miss.html) and do more practice.

### IntelliJ IDEA常用Tips
- Java代码应删去没有引用到的包，Import语句为灰色即是，Mac可以通过`Control + Option + O`快捷键删去，Linux为`Ctrl + Alt + L`。
- 类文件开始处不要出现 "/* xxx create xxx */" 这样自动生成的注释，在IntelliJ的settings中搜索`File and Code Template`，找到`File`页中的两个Header项，分别删除其中的模板内容后Apply即可。
- 修改Import为非`*`模式，并且按照一定的顺序排序，在`Code Style -> Java -> Imports`中分别将Import数5和3修改大一些，在Import Layout中可以指定顺序，比如：`static all other imports`, `java.*`, `javax.*`, `org.*`, `net.*`, `com.*` and `all other imports`，通常根据Team情况而定。
- 还有一个很好用的Feature，确保`Smart Keys -> User "CamelHumps" words`是开启的，这样在驼峰命名上可以智能移动光标。
- 对于前端的代码，React风格校验不过的，在IntelliJ的settings中搜索到`Language & Frameworks`，找到`Javascript`修改为`JSX Harmony`后Apply即可。


### Git Learning Guide
首先，可以申请一个[Github](http://github.com/)帐号，然后使用分布式版本控制工具Git对源代码进行管理，以下是一些关于Git学习的资料和教程，仅供参考：

- [Try Git](https://www.codeschool.com/courses/try-git)
- [Learn Git Branching](http://learngitbranching.js.org/)
- [Git SCM](http://git-scm.com/book/en/v2)
- [优雅地使用Git](http://blog.waterstrong.me/master-git/)


### 补充学习：
可以提前看一些TDD内容，对于Java的测试框架为JUnit, Mockito，构建工具为Gradle，可以提前查资料学习下。有时间可以了解一下OO, Refactor, Clean Code, Design Pattern, Functional programming, Java8等。




