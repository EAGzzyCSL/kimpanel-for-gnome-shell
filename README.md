KDE's kimpanel implementation for GNOME Shell

Install requirements
gettext
cmake

If you'd like to install it as user, run ./install.sh under the root of source.

-------

分--------------------割--------------------线

-------

# 我的魔改

> bg: 我使用gnome和fcitx，该插件可以让fcitx的输入面板和gnome风格一致，非常棒。but不幸的是在高分屏下不知是fcitx还是kimpanel的问题，反正高分屏总会遇到一些问题，候选词框的位置在chrome下是预期位置的两倍坐标处，在vscode下是预期位置的一半坐标处……。类似的情况还出现在atom这些electron app下。

我在插件的代码里面加入了一个自定义的函数用来检测当前输入的window是chrome或vscode，从而对面板的位置x2或者/2……
