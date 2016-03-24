Git is a distributed version control system.
Git is free software distributed under GPL.
Git has mutable index called stage.
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