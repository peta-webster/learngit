## Git

### 本地仓库：

`git init`

`git add -A`

`git commit -m " "`

`git log`: Q退出日志查询界面

`cd xxx`

`ls`:查看当前目录下的文件

`echo "写入内容" >> README.md `:创建文件并写入内容

`cat text.txt`;

### 远程仓库：

`git remote add origin 仓库地址`： 建立连接



第一次：`git push -u origin master`； 以后：`git push origin master`



`git fetch origin`; `git merge origin/master`



`git remote -v`:查看远程库 ; `git remote rm origin`：删除远程库 

- 执行 `git fetch origin master` 时，它的意思是从名为 **origin** 的远程上拉取名为 **master** 的分支到本地分支 **origin/master** 中。既然是拉取代码，当然需要同时指定远程名与分支名，所以分开写。
- 执行 `git merge origin/master` 时，它的意思是合并名为 **origin/master** 的分支到当前所在分支。既然是分支的合并，当然就与远程名没有直接的关系，所以没有出现远程名。需要指定的是被合并的分支。
- 执行 `git push origin master` 时，它的意思是推送本地的 **master** 分支到远程 **origin**，涉及到远程以及分支，当然也得分开写了。



错误：git branch origin2(创建新的分支)； git checkout origin2

​	git merge origin2(将当前分支与origin2分支合并)

​	git branch -d origin2(删除分支)

​	
