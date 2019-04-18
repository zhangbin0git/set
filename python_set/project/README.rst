===================
项目名称
===================

目的
=====

应用模块的具体功能

工具版本
====================

:Python:     2.7.8
:pip:        1.5.6
:virtualenv: 1.11.6


安装与启动方法
=======================

从版本库获取代码，然后在该目录下搭建virtualenv环境::

   $ hg clone git@github.com:zhangbin0git/security.git
   $ cd security
   $ virtualenv .venv
   $ source .venv/bin/activate
   (.venv)$ pip install .
   (.venv)$ security
    * Running on http://127.0.0.1:5000/


开发流程
=========

用于开发的安装
------------------

1. 检测
2. 按以下流程安装::

     (.venv)$ pip install -e .

变更依赖库时
---------------------

1. 更新``setup.py``的``install_requires``
2. 按以下流程更新环境::

     (.venv)$ virtualenv --clear .venv
     (.venv)$ pip install -e ./security

3. 将setup.py提交到版本库

变更依赖库时
---------------------

1. 更新``setup.py``的``install_requires``
2. 按以下流程更新环境::

     (.venv)$ virtualenv --clear .venv
     (.venv)$ pip install -e ./security
     (.venv)$ pip freeze > requirements.txt

3. 将setup.py和requirements.txt提交到版本库






