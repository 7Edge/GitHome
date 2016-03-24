Git is a distributed version control system.
Git is free software distributed under GPL.
Git has mutable index called stage.
Git tracks changes of files.
Acount:
#git config --global user.name "+7"
#git config --global user.email "1399622866@qq.com"
Create store house:
#cd /e/
#mkdir GitHome
init:
#git init

Git是分布式的版本控制系统。
和集中式的相比，集中式SVN是有中央服务器的，每次需要下载和上传，需要连接互联网。
GIT是本地管理版本库，多方协作是通过互相交换更改的信息，来保持双方版本同意和知道对方的版本修改。

back old version:

#git log  查看提交历史
#git reset --hard HEAD~1 2 3  or git reset --hard HEAD^  ^^
#git log 
#git reflog	查看命令历史
#
关于工作区-暂存区-master区  还有HEAD操作 
具体访问：http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/0013745374151782eb658c5a5ca454eaa451661275886c6000
有人说：暂存区相当于购物车，将修改的东西都加到购物车暂存区中，如果不像提交，就是不像付款，还可以使用checkout单独将某个文件恢复过去，如果直接提交，那么这次修改的多个文件看作一个整体版本归档，这样要恢复一个文件是不可能了，只有恢复全部文件到上一个版本。

git local  assoc  github:
本地的仓库和github远程的仓库关联
#git remote add origin git@github.com:7Edge/GitHome.git 
这样，将本地的GitHome和origin远程库名管理，在远程的库名其实我命名也为GitHome。关联后一直有效。
只需要每次push 就可以将本地库推送到远程。
#git push -u origin master 第一次加-u参数，以后本地提交完成，就不需要-u直接：
#git push origin master

测试：
在dev分支上修改并add commit但是没有合并，然后切换到master，再修改master add commit 查看结果，再合并，查看结果是什么样的。