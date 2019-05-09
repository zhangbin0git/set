=========================
conda set
=========================

相关命令
=========================================
获取版本号
conda --versiont

获取帮助
conda --help

创建制定python版本的环境
conda create --name your_env_name python=2.7
conda create --name your_env_name python=3
conda create --name your_env_name python=3.5

创建包含某些包的环境
conda create --name your_env_name numpy scipy

复制某个环境
conda create --name new_env_name --clone old_env_name 

删除某个环境
conda remove --name your_env_name --all

导出环境
conda env export > environment.yml

导入环境
conda env create -f environment.yml



～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～
# 相关问题
～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～～

============================


