=========================
python_set
=========================

python 项目通用结构
=========================================
project:

touch LICENSE
touch MANIFEST.in
touch README.rst
mkdir conf
mkdir fabfile
mkdir others
touch requirements.txt
touch setup.py
mkdir src
touch .gitignore

# LICENSE AND .gitignore AND README.rst 三个文件需要从model中拷贝

virtualenv 配置
====================================
# 安装virtualenv
$ pip install virtualenv

# 创建虚拟环境：
$ virtualenv --no-site-packages venv (创建纯净环境)
$ virtualenv --system-site-packages venv （创建环境，继承原安装的模块）

# 激活该虚拟环境：
$ source venv/bin/activate

# 退出虚拟环境：
$ deactivate







