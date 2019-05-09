kali-linux_set
==================

设置kali 中文
==============================
首先选择在kali的系统set中修改语言
如果不行如下
确定locales已经安装，用”apt-get install locales”命令；之后可用”locale -a”查看当前系统支持的字符集。

1.在命令行输入”dpkg-reconfigure locales”。进入图形化界面之后，（空格是选择，Tab是切换，*是选中），选中en_US.UTF-8和zh_CN.UTF-8，确定后，将en_US.UTF-8选为默认。
2. 安装中文字体，”apt-get install xfonts-intl-chinese “和” apt-get install ttf-wqy-microhei”，这时发现网页不乱码，系统也不乱码。
3. 重启 。

查看ip地址
==============================
ifconfig -a