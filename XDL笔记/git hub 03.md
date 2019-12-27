## day04

```
 git       创建库提交步骤：
​ git hub教程：                https://www.runoob.com/git/git-tutorial.html
​ 公钥和私钥理解：        http://dy.163.com/v2/article/detail/E4MO5M5P0511L2E2.html
                                                 https://blog.csdn.net/baudu_36327010/article/details/78659665
​ jekyll 文档：                   http://jekyllcn.com/
​ jekyll模板() ：                http://jekyllthemes.org/
​ jekyll安装：                    https://ywnz.com/linuxyffq/4335.html
​     Git 创建仓库
                        git        init                                          使用当前目录作为Git仓库  并初始化.
                        git        add                                          添加
                        git        status                                        命令用于查看项目的当前状态。
                        git      commit -m "备注信息"      提交到暂存区
                        git      remote add origin  http:// 远程仓库连接地址
                        git      push -u  origin   master      推送到远程服务器master分支下
                        git       clone                                        克隆命令   
                        git       diff                                                   执行来查看执行git status的结果的详细信息。
                        git        push  origin  test : test                    远 程库创建test 分支
                        git      merge    origin /分支文件      提取所有分支文件
                        git      fetch   -a                                        获取所有远程分支
                        git reset HEAD                                        命令用于取消已缓存的内容。
                        git   rm-缓存<文件>        删除文件
                        git clone	[url]					        Git 仓库到本地，让自己能够查看该项目，或者进行修改
                        git diff									        尚未缓存的改动
                        git diff --cached					      查看已缓存的改动：
                        git diff HEAD								 查看已缓存的与未缓存的所有改动：
                        git diff --stat									显示摘要而非整个 diff：
                        git commit									 将缓存区内容添加到仓库中
​    要从Git中移除某个文件，就必须要从已跟踪文件清单中移除，然后提交。可以使用以下命令完成这项工作

​     可以递归归删除，即如果后面跟的是一个目录做为参数，逐步递归归删除整个目录中的所  有子目录和文件：
              git rm –r * 
              git rm –r * 
​    git mv
              git mv命令用于移动或重命名一个文件，
              git mv自述文件README.md
​	创建分支命令：
              git branch
​切换分支命令:	
             git checkout 
​ 	合并分支命令:		     
               git merge
​删除分支命令          ：git branch -d 
​列出分支基本命令 ：git branch
​ 分支合并                  :   git merge




 ​git pull origin master //将远程仓库里面的项目拉下来。
 ​dir   查看远程仓库项目里面的文件夹
```

### 1.	Git

#####  1.1 Github社区与git软件

```
            1.  创建github社区账号
                通过百度搜索github 进入到git社区中，创建自己的账号
            2.	点击右上角+号，选择新存储库选项，然后创建库
            3.	安装本地git软件
                a.	打开终端  输入命令：sudo apt-get install git
                b.	验证git是否安装成功，输出命令：git version
                c.	配置用户名和邮箱，输入命令：
                        git config --global user.name "XXXX"         配置用户名，用户名为上面自己创建的github的账号
                       git config --global user.email  "XXXXXXXXXX"    配置邮箱，确保邮箱存在且正确
                d.	查看是否配置成功，输入命令：git config --list
                e.	配置Git的私钥和公钥.密码为空.  输入命令：ssh-keygen -t rsa  -C "用户邮箱"      注：出来需要输入的							东西，直接回车
                f.	证书已经生成成功，进入指定路径下，输入命令：cd ~/.ssh/
                g.	打开github社区，选择头像下的设置选项中的SSH和GPC密钥被选项
                h.	看到上面的GitHub的SSH配置后,在新建一个SSH Key.
                i.	vim 打开Git的公钥证书.(在上述查看证书的文件夹下)
                j.	打开证书文件，复制文件中全部的文字，到GitHub中的key中
                k. 验证Git是否配置成功: ssh git@github.com   
            4.	Git创建仓库
```

##### 1.2 git创建仓库

```
                1. 在自己所需目录下创建新目录,比如在home目录下
                    mkdir a
                2. 进入该目录，初始化该目录，此目录就可以成为一个git仓库
                    cd	a
                       git init
                3.	初始化后，该目录下会出现 .gif的文档，也可以在该目录下创建并编辑其他文档,然后用git add 命令让                       git对其进行跟踪
                    touch 1.txt              vim 2.txt
                    git add 1.txt    跟踪1.txt        git add . 		跟踪所有文档
                4. 提交到缓存区
                    git commit -m "备注"
                5. 建立远程
                    git remote add origin "url"
                6. 推送到github社区
                    git push -u origin master		git push -u origin 分支
```

##### 1.3 git工作流程

```
                    a.  克隆 Git 资源作为工作目录。
                    b.  在克隆的资源上添加或修改文件。
                    c.  如果其他人修改了，你可以更新资源。
                    d.  在提交前查看修改。
                    e.  提交修改。
                    f.  在修改完成后，如果发现错误，可以撤回提交并再次修改并提交。
```

### 1.5 git分支管理

```
git branch  														   分支列表
git branch 分支名					 							 创建新分支
git checkout 分支名			   							  切换分支
git checkout -b 分支名			 							切换并进入分支
git branch  -d  分支名										   删除分支
git merge	分支名												  合并分支
```

#### 2.	团队合作流程

2.1	流程
		a.	在github社区新建仓库  
				item
		b.	创建本地仓库，建立文档，推送到github社区仓库
				mkdir work			创建目录
				cd work					进入目录
				git init					创建仓库
				touch zp.txt		 简历文档
				git add .				 添加跟踪
				git commit -m "zp"   提交到缓存区
				git remote add origin ""	建立远程
				git push -u origin master	提交
		c.	点击设置——合作者——通过用户账号邀请组员
		d.	自己创建分支，添加文件或文档，推送到github.
				git  branch zp			建立分支
				git checkout zp		切换至分支
				touch 1204.txt      添加文档
				git add .
				git commit -m 'zp'
				git push -u origin zp       git push origin zp:zp
		e.	等待组员提交
		f.	组员提交后，拉取分支到本地
		         git checkout zp      切换至分支
		         git fetch -a          拉取分支到本地     
		g.	合并组员分支到自己的分支，并提交
			git merge origin/分支1
			git merge origin/分支2
			git merge origin/分支3
			git add .
			git commit -m 'zp'
			git push -u origin zp   
		h.	切换之master ,合并自己的分支到master.并提交
			git checkout master
			git merge zp    合并分支
			git add .
			git commit -m 'zp'
			git push -u origin master
2.2	 	相关操作
			git fetch   -a 拉取分支到本地
			git	merge origin/分支     合并组员分支

#### 3. 安装Jekyll的方法步骤 

```
                1.	$ sudo apt-get  update
                2.	$ sudo apt-get upgrade
                3.	$ sudo apt-get install make build-essential
                4.	$ sudo apt-get install ruby ruby-dev
                5.	vim		~/.bashrc
                6.	进入vim编辑器之后转换到插入模式，在最后一行插入

                    export GEM_HOME=$HOME/gems
                    export PATH=$HOME/gems/bin:$PATH
                    之后，保存退出。
                7.	$ source ~/.bashrc
                8.	$ gem install bundler
                9.	$ gem install jekyll
```

#### 4. Jekyll搭建静态网站

```
            1.	在github 上注册一个 账号，例如注册用户名为：zp0993
            2.	新建一个仓库：仓库名称格式为：用户名.github.io
               （注意：仓库名称一定要按格式）
            3.	在本地建仓库，在里面新建一个index.html的文件，在里面输入任意内容，然后
                代码推送到git上。
            4.	在浏览器访问http://zp0993.github.io/,可以发现index.html里面的内容就被访  
```

### GIT HUB   删除命令注意事项

```
1.上面的方法会把对应的本地文件也删除掉，如果不想把本地文件删除，只把缓存区中的对应部分删除，则加上--cached
git rm --cached 文件 //本地中该文件不会被删除
git rm -r  --cached  文件夹 //删除文件夹
在git add .后面执行上面的命令，再推送到github远程仓库上的时候，仓库里面对应的文件/文件夹就会被删除
```

```
git简写
git st   # git status
git ci   # git commit
git br   # git branch
git co   # git checkout
git mg   # git merge
git line # git log --oneline

git init 			#初始化gi库
git add file 			#增加库文件,也可以用git add .意思为添加所有
git commit -m "update"   	#提交并注释
git push origin -u master master #首次推送到远程仓库
git push origin test 		#推送到test分支
git branch  			#查看本地分支
git branch -a 			#查看所有分支
git branch test 		#创建test分支,但不切换
git checkout -b test 		#如果test分支存在就切换到test分支,如果不存在就创建并且换到test分支
git checkout test               #切换到test分支
git push 			#推送
git push -u origin/test         #提交本地库到远程test分支
git push origin test:test 	#提交本test分支作为test分支
git push origin test:master 	#提交本test分支作为master分支
git branch -d test 		#删除本地分支
git push origin --delete crond 	#删除远程分支
git push origin :test 		#删除远程分支
git branch -m | -M oldbranch newbranch #重命名分支，如果newbranch名字分支已经存在，则需要使用-M强制重命名，否则，使用-m进行重命名
git branch -d | -D test 	#删除本地test分支
git branch -d -r test 		#删除远程分支
git remote -v                           #查看远程仓库
git remote add [name] [url]             #添加远程仓库
git remote rm [name]                    #删除远程仓库
git remote set-url --push[name][newUrl] #修改远程仓库


下面是网上找的git常用命令

查看、添加、提交、删除、找回，重置修改文件
git help <command> # 显示command的help
git show # 显示某次提交的内容 git show $id
git co -- <file> # 抛弃工作区修改
git co . # 抛弃工作区修改
git add <file> # 将工作文件修改提交到本地暂存区
git add . # 将所有修改过的工作文件提交暂存区
git rm <file> # 从版本库中删除文件
git rm <file> --cached # 从版本库中删除文件，但不删除文件
git reset <file> # 从暂存区恢复到工作文件
git reset -- . # 从暂存区恢复到工作文件
git reset --hard # 恢复最近一次提交过的状态，即放弃上次提交后的所有本次修改
git ci <file> 
git ci . 
git ci -a # 将git add, git rm和git ci等操作都合并在一起做
git ci -am "some comments"
git ci --amend # 修改最后一次提交记录
git revert <$id> # 恢复某次提交的状态，恢复动作本身也创建次提交对象
git revert HEAD # 恢复最后一次提交的状态
查看文件diff
git diff <file> # 比较当前文件和暂存区文件差异 git diff
git diff <id1><id2> # 比较两次提交之间的差异
git diff <branch1>..<branch2> # 在两个分支之间比较
git diff --staged # 比较暂存区和版本库差异
git diff --cached # 比较暂存区和版本库差异
git diff --stat # 仅仅比较统计信息
查看提交记录
git log git log <file> # 查看该文件每次提交记录
git log -p <file> # 查看每次详细修改内容的diff
git log -p -2 # 查看最近两次详细修改内容的diff
git log --stat #查看提交统计信息



Git 本地分支管理
查看、切换、创建和删除分支
git br -r # 查看远程分支
git br <new_branch> # 创建新的分支
git br -v # 查看各个分支最后提交信息
git br --merged # 查看已经被合并到当前分支的分支
git br --no-merged # 查看尚未被合并到当前分支的分支
git co <branch> # 切换到某个分支
git co -b <new_branch> # 创建新的分支，并且切换过去
git co -b <new_branch> <branch> # 基于branch创建新的new_branch
git co $id # 把某次历史提交记录checkout出来，但无分支信息，切换到其他分支会自动删除
git co $id -b <new_branch> # 把某次历史提交记录checkout出来，创建成一个分支
git br -d <branch> # 删除某个分支
git br -D <branch> # 强制删除某个分支 (未被合并的分支被删除的时候需要强制)
 分支合并和rebase
git merge <branch> # 将branch分支合并到当前分支
git merge origin/master --no-ff # 不要Fast-Foward合并，这样可以生成merge提交
git rebase master <branch> # 将master rebase到branch，
相当于:git co <branch> && git rebase master && git co master && git merge <branch>
 Git补丁管理(方便在多台机器上开发同步时用)
git diff > ../sync.patch # 生成补丁
git apply ../sync.patch # 打补丁
git apply --check ../sync.patch #测试补丁能否成功
 
 
 
 
 Git暂存管理
git stash # 暂存
git stash list # 列所有stash
git stash apply # 恢复暂存的内容
git stash drop # 删除暂存区
Git远程分支管理
git pull # 抓取远程仓库所有分支更新并合并到本地
git pull --no-ff # 抓取远程仓库所有分支更新并合并到本地，不要快进合并
git fetch origin # 抓取远程仓库更新
git merge origin/master # 将远程主分支合并到本地当前分支
git co --track origin/branch # 跟踪某个远程分支创建相应的本地分支
git co -b <local_branch> origin/<remote_branch> # 基于远程分支创建本地分支，功能同上
git push # push所有分支
git push origin master # 将本地主分支推到远程主分支
git push -u origin master # 将本地主分支推到远程(如无远程主分支则创建，用于初始化远程仓库)
git push origin <local_branch> # 创建远程分支， origin是远程仓库名
git push origin <local_branch>:<remote_branch> # 创建远程分支
git push origin :<remote_branch> #先删除本地分支(git br -d <branch>)，然后再push删除远程分支
Git远程仓库管理
git remote -v # 查看远程服务器地址和仓库名称
git remote show origin # 查看远程服务器仓库状态
git remote add origin git@ github:robbin/robbin_site.git # 添加远程仓库地址
git remote set-url origin git@ github.com:robbin/robbin_site.git # 设置远程仓库地址(用于修改远程仓库地址) 
git remote rm <repository> # 删除远程仓库
创建远程仓库
git clone --bare robbin_site robbin_site.git # 用带版本的项目创建纯版本仓库
scp -r my_project.git git@ git.csdn.net:~ # 将纯仓库上传到服务器上
mkdir robbin_site.git && cd robbin_site.git && git --bare init # 在服务器创建纯仓库
git remote add origin git@ github.com:robbin/robbin_site.git # 设置远程仓库地址
git push -u origin master # 客户端首次提交
git push -u origin develop # 首次将本地develop分支提交到远程develop分支，并且track
git remote set-head origin master # 设置远程仓库的HEAD指向master分支
也可以命令设置跟踪远程库和本地库
git branch --set-upstream master origin/master
git branch --set-upstream develop origin/develop
```

