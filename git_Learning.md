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