# demo
这是一个git学习笔记
git命令

git   commit -m "版本名" 文件名

查看版本
git reflog 查看引用日志信息
只能看见6位版本号

git log 查看完整日志信息
可以查看全部版本号以及提交人


穿梭版本（使用后会有日志，记录本次操作）
git reset  --hard 版本号
版本穿梭机制底层其实就是移动了head指针，使他指向不同的版本



分支 （使用分支就是对主线master的copy ，拿着副本去做修改，即使代码修改失败，也不会对主线master产生影响）

查看分支
git branch -v 

创建分支
git branch 分支名

切换分支
git checkout 分支名

合并分支
git merge 分支名（此分支名是要拉取的分支，在那个分支下运行就是吧拉取分支合并到当前分支）

冲突合并并手动修改提交时，提交本地库不用带文件名



git.ignore配置文件（配置在windows家目录下）

# Compiled class file
*.class

# Log file
*.log

# BlueJ files
*.ctxt

# Mobile Tools for Java (J2ME)
.mtj.tmp/# Package Files #
*.jar
*.war
*.nar
*.ear
*.zip
*.tar.gz
*.rar

hs_err_pid*

.classpath
.project
.settings
target
.idea
*.iml



git主配置文件需要引用此文件
[core]
	excludesfile = C:/Users/PC-001/git.ignore


