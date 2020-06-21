“cd”改变当前路径
“cd 文件名”打开某文件
“cd ..” 返回上一层目录
ls 无参数时，显示当前目录下的文件。当前目录就是指，用户操作命令时，所处的目录，可用pwd看到
ls 显示当前下面的文件及文件夹
ls -a 显示当前目录下的所有文件及文件夹包括隐藏的.和..等
mkdir 新建文件夹
code .打开目录
1.print为一般输出，同样不能保留精度格式转化，也不能换行输出 
2.printf常用于格式转换，但需要注意不是换行输出，只用于精度转换 
3.println为换行输出，不能用于格式转换
Git基本操作
1. 使用git初始化工作目录 git init
2. 查看文件状态 git status
3. 提交自己的修改到本地git服务器 git add;git commit
4. 将git远程服务器地址关联到工作目录
git remote add orgin https://github.com/<yourid>/<yourrepo>.git
5. 推送代码到远程 git push
6. 从远程拉取代码到本地 git pull
7. 查看提交历史 git log
使git忽略某些文件
在某些情况下，可能需要使 git 忽略掉工作目录下的一些文件/文件夹
eg· 编辑器自动生成的文,node_modules、临时文件等
做法：
新建一个名为.gitignore的文本文件， 将需要忽略的文件/文件夹写在
该文件中
创建和切换分支
创建分支
git branch (branchname)
切换分支
git checkout (branchname)
创建并切换到该分支
git checkout -b (branchname)
查看和删除分支
查看所有分支
git branch
删除分支
git branch -d (branchname)
版本回退
代码提交了之后才发现提交有问题，如何撤销这次提交呢？
git reset
git revert
