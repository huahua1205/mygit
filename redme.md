1，git 安装

2，git 初始化：git  init

3，git配置用户

​	3.1 git config --global user.name "用户名"

​	3.2 git config --global user.email "邮箱地址"

4，代码保存到git仓库中

​	4.1 放到大门口 ：

​			4.1.1 git add ./文件路径  这个是把指定的一个文件放到暂存区

​			4.1.2  git add ./    这个是把所有修改的文件放到暂存区

​	4.2 放到仓库房间 ： git commit -m "说明"

6，也可以一次性把文件放到版本库

​	git commit --all -m "说明"

5，查看文件状态 git status

​	5.1 红色代表在工作区

​	5.2 绿色代表在大门口（暂存区）

​	5.3 白色代表在仓库房间（版本区）

