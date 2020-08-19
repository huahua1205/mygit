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

7,如果某些文件不想放到版本区里，可以通过gitignore设置，一行写一个路径
    7.1 ./文件名   忽略指定文件
    7.2  ./文件夹名   忽略指定的文件夹
    7.3  ./文件夹名/*.文件扩展名   忽略指定文件夹下的指定的同一类型的文件

8, 查看日志
    8.1 git log 查看历史提交的日志
    8.2 git log --oneline  查看简洁版的日志

9，回退版本
    9.1 git reset --hard Head~0  回退到上一版本
    9.2 git reset --hard Head~1  回退到上一版本  以此类推
    9.3 git reset --hard 版本号   可以精确的回到某一版本
    9.4 git reflog  可以查到所有版本的提交记录


## 分支
1，默认又一个主分支  master
2，创建分支
    git branch dev   创建了一个dev的分支
3，切换分支
    git checkout dev  切换到指定的分支
    git branch  可以查看有哪些分支，带有*的为当前所在的分支
4，在新的分支里可以提交新的文件
5，合并分支
    git merge dev 合并分支内容，把当前分支与指定分支（dev）合并
