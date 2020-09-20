# 9.20学习笔记

### First

- 克隆他人的项目需要先在项目中先邀请他人，复制SSH链接，进入要复制到的地址，使用git clone =SSH链接进行复制。
- 对文件进行修改后，还是应该先add然后commit -m然后push origin master
- 如果有冲突，比如多人同时修改文件，就把别人做的删掉然后再push
- 也可以先pull，拉到本地，看看现在改成了啥样



### Second

- 关于分支的话，如果要查看，就是直接git branch，如果要新建，就是git branch +名字，切换分支就是git checkout +分支名字
- 合并分支要先切换回要合并到的那个分支（比如master）然后使用git merge +另一个分支的名字，再git push，然后重复git add与commit，最后git push推到远程
- 删除分支的命令是git branch -d dev

