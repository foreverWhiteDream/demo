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
