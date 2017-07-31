# git-learning  [廖雪峰的git教程](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)

##安装git
##管理版本库
- git init  创建
- git add 增加，提交修改和提交新文件都要做
- git commit  本次提交的说明，可以输入任意内容，当然最好是有意义的 
- git diff  查看difference, 比如git add readme.txt
- git log/git log --pretty=oneline 查看日志/单行显示日志
- git reset 版本回退
- git reset --hard HEAD^  回退到上一个版本。上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100。
- git reset --hard 3628164  3628164指的是commit id
- 工作区、版本库、暂存区、master的区别
- git checkout -- file
- git rm+git commit:两部操作删除文件
- git rm+git checkout -- 需要恢复的文件名 

##github
- ssh-keygen -t rsa -C "youremail@example.com"    创建SSH Key
- Create repository  添加远程库
- git remote add origin git@github.com:michaelliao/learngit.git   其中，michaelliao替换成你自己的GitHub账户名，否则，你在本地关联的就是我的远程库，关联没有问题，但是你以后推送是推不上去的，因为你的SSH Key公钥不在我的账户列表中
-  ssh -T git@github.com后有个提示记得输入yes，表示确认连接。不然后面容易出现错误  '''
Host key verification failed.
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
'''
##git clone


##分支管理
###创建分支
- git checkout -b dev 相当于git branch dev加上git checkout dev
- git branch
- git checkout master
- git merge dev
- git branch -d dev  

###解决冲突
- git log --graph --pretty=oneline --abbrev-commit   查看分支的合并情况

###分支策略
- git merge --no-ff -m "merge with no-ff" dev  禁用Fast forward模式，保留开发者自己的分支
- bug/特性都可以拉出独立的分支，适合多人写作

###标签管理

##搭建git服务器





