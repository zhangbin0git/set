=========================
git �������
=========================

��װgit
=========================================
Debian/Ubuntu
For the latest stable version for your release of Debian/Ubuntu
# apt-get install git

ж��git
=============================
# sudo apt-get autoremove --purge <softname>
sudo �������� ��ȡ root Ȩ��
apt-get ������ ִ�а�װж�ع��ܵ����
autoremove �� ���� apt-get ������Ҫ���Ĳ������Ƴ����
--purge ������ ע����ǰ���������̻��ߣ���������Ǹ�������Ҫ�����ĸɾ��ĳ��׵��Ƴ���

����github
=============================
# git config --global user.name "zhangbin0git"
# git config --global user.email "zhangbin.email@foxmail.com"
# ssh-keygen -t rsa -C "zhangbin.email@foxmail.com"
# ssh -T git@github.com

����githubԶ�ֿ̲�
==================================
# echo "# security" >> README.md
# git init
# git add README.md
# git commit -m "first commit"
# git remote add origin git@github.com:zhangbin0git/security.git
# git push -u origin master

����.gitignore
===========================
GitHub�Ѿ�Ϊ����׼���˸���.gitignore�����ļ���ֻ��Ҫ���һ�¾Ϳ���ʹ���� https://github.com/github/gitignore

eg��
---------------------------------
# Windows:
Thumbs.db
ehthumbs.db
Desktop.ini

# Python:
*.py[cod]
*.so
*.egg
*.egg-info
dist
build

# My configurations:
db.ini
deploy_key_rsa
---------------------------------

�㷢�֣�������.gitignoreд�������⣬��Ҫ�ҳ��������ĸ�����д���ˣ�������git check-ignore������
# git check-ignore -v App.class

git ���ñ���
================
# git config --global alias.st status
# git config --global alias.co checkout
# git config --global alias.ci commit
# git config --global alias.br branch
����git reset HEAD file���԰��ݴ������޸ĳ�������unstage�������·Żع�����
# git config --global alias.unstage 'reset HEAD'
����һ��git last��������ʾ���һ���ύ��Ϣ
# git config --global alias.last 'log -1'
# git lg
# git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"

���git config����
=================================
��
# git config --global ���� 'ֵ';
��:
��������������Ҳ����ֱ�Ӹ����޸�,�������滻git config�����е�����
# git config --global --replace-all user.email "�����������"
# git config --global --replace-all user.name "��������û���"
ɾ��
# git config --global --unset  ����

��֧���
=========================
# ���Ǵ���dev��֧��Ȼ���л���dev��֧
git checkout -b dev

# git checkout�������-b������ʾ�������л����൱��������������
git branch dev
git checkout dev

# ��git branch����鿴��ǰ��֧
git branch

#dev��֧�Ĺ�����ɣ����ǾͿ����л���master��֧
git checkout master

# ���ǰ�dev��֧�Ĺ����ɹ��ϲ���master��֧��
git merge dev

# �ϲ���ɺ󣬾Ϳ��Է��ĵ�ɾ��dev��֧
git branch -d dev

�鿴��֧��git branch

������֧��git branch <name>

�л���֧��git checkout <name>

����+�л���֧��git checkout -b <name>

�ϲ�ĳ��֧����ǰ��֧��git merge <name>

ɾ����֧��git branch -d <name>


==============================





��������������������������������������������������������������������������������
# �������
��������������������������������������������������������������������������������
git [packet_write_wait connection to xx.xx.xx.xx Broken pipe]����취
============================
�ҵ�git��װ��Ŀ¼/etc/ssh����ssh_config�ļ����������޸ģ�������ӣ�

Host *  ---->Host����ͼ���ҵ�
ServerAliveInterval 120


ssh ����
==============================
����ssh -T -v git@github.com�鿴���������Ϣ���ٸ�����Ϣ������

