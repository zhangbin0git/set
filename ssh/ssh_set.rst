ssh_set
===================================



安装ssh客户端
===================================
# sudo apt-get install ssh
或者推荐
# sudo apt-get install openssh-client    



OpenSSh 分为客户端openssh-client 与服务端 openssh-server.一般情况下，我们的linux系统都会自带 client端的。
===================================
最简单的方法：
apt-get install openssh-client
apt-get install openssh-server

开启服务
service ssh start

安装完成以后,可以通过以下命令看到它们运行的进程:
ps -e |grep ssh

修改后以后，我们需要重新启动服务：
方法一：
 /etc/init.d/ssh restart
方法二：
service ssh restart

通过 service ssh status 可以查看服务的状态
