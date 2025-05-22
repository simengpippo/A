#本文件主要记录git学习过程中用到的一些命令

#首先操作需要进入目标文件夹

#初始化代码库
git init

#添加文件到代码库
git add readme.txt

#提交文件
git commit -m"添加了一个readme.txt文件"   //-m后输入说明

#添加远程仓库from github
#首先在github上创建仓库
#要在本地生成密钥，然后再github上保存密钥，才可以互认
#关联远程库
git remote add origin git@github.com:simengpippo/A.git
#本地库和远程库的名字并不需要一致，可以理解问本地库的.git文件与远程库的.git文件关联
#origin为本地库认为的远程库的名字

#关联之后就可以进行推送等操作
#向远程库推送本地内容
git push -u origin master    //-u 是 --set-upstream 的缩写，主要用于建立本地分支与远程分支的追踪关系
#从远程库拉取内容，同步远程更改
git pull origin master
#从远程库克隆 //不必关联
git clone git@github.com:simengpippo/add

**心得：不能代码仓库包含代码仓库



