# 项目简述

#### git 基本工作流程

1.  克隆远程资源到本地目录，作为工作目录
2.  在本地克隆资源上添加，修改或删除文件
3.  如果远程资源有修改，需要同步远程的内容，更改本地的文件
4.  提交修改前，查看修改情况，处理冲突文件
5.  添加修改到缓冲区，提交修改到本地版本库
6.  提交修改后，将本地版本推送到远程git服务器

####  四个区域的名称

1.   workspace           代表工作区域
2.   staging area        代表暂存区或缓存区
3.   local repository    代表版本库或本地仓库
4.   remote repository   代表远程仓库

#### 创建仓库

1.  git init         初始化一个git仓库
2.  git init hello   在 hello 的文件夹中生成一个.git

#### 克隆远程资源或拉取更新

1.  git clone https://gitee.com/window-of-the-world_0/helloworld.git
2.  git pull origin maser     拉取远程文件到本地
3.  https://       GiT     SSH     三种协议

#### git的用户信息配置

1.  git config --global user.name '陈旗' 
2.  git config --global user.email '2490995289@qq.com'
3.  git config --list   查看用户信息
4.  git diff            查看更新的详细信息  
5.  git reset HEAD      取消缓存命令
6.  git rm              删除命令
7.  git mv              移动或重命名命令

#### git常用命令
  
1.  git status     查看修改情况
2.  git add .      添加修改到缓冲区
3.  git commit -m '提交描述'    提交到本地的git仓库
4.  git push origin maser  将本地的修改推送到远程git仓库

#### 分支与合并操作命令

1.   git branch	            查看分支
2.   git branch hello	    创建 hello 分支
3.   git checkout hello	    切换到 hello 分支
4.   git checkout -b hello  创建并切换到 hello 分支
5.   git merge hello        在 maser 目录下执行合并 hello 分支
6.   git checkout maser     合并冲突先解决主分支的，再解决要合并的分支 然后再合并
5.   git branch -d hello    删除 hello 分支

#### 查看提交历史的一些操作命令

1.   git log	         查看历史提交记录并列出记录详情
2.   git log --oneline   查看记录的简介版
3.   git log --graph 	 查看历史记录中出现的分支与合并。
4.   git log --reverse   逆向显示历史日志	     
5.   git log --author=chenqi oneline -8  查找指定用户的提交日志	         
6.   git log --oneline --before={2023-03-01} --after={2024-10-01} --no-merges 
0.   git log --since     指定筛选日期
7.   git log --before    指定筛选日期	         
8.   git log --until     指定筛选日期
9.   git log --after     指定筛选日期
10.  git log --no-merges 选项以隐藏合并提交

#### 查看配置标签命令

1.  git log --oneline --decorate 指向分支和标签
2.  git tag -a v1.0     创建新标签
3.  git tag -a v0.6 d4f5158    追加一个标签
4.  git tag            查看所有标签
5.  git tag -a <tagname> -m "d4f5158"  指定标签信息命令
6.  git tag -s <tagname> -m "d4f5158"  指定标签信息命令 

#### 远程仓库添加到本地并命名为 hello

1.   git remote add hello https://gitee.com/window-of-the-world_0/helloworld.git 
2.   git remote  查看当前有哪些远程仓库
3.   git fetch hello  获取远程仓库的数据，然后执行下一条命令才算完成
4.   git merge hello/master   将获取的仓库数据合并到当下分支:支持空仓库
5.   git pull hello master --allow-unrelated-historiesFrom https://gitee.com/
6.       window-of-the-world_0/helloworld.git 获取远程仓库并合并到本地
7.   git fetch hello master --allow-unrelated-historiesFrom https://gitee.com/
8.       window-of-the-world_0/helloworld.git 获取远程仓库不合并
7.   git push hello master  推送你的新分支与数据到指定的远程仓库
8.   git remote add hello https://gitee.com/helloworld.git 添加一个远程仓库
9.   git remote -rm hello    删除一个远程仓库
10.   git remote         查询远程都有哪些仓库
11.   git remote -v      查询远程仓库详情地址url
12.   echo 203.208.40.66 translate.googleapis.com > >|C:\Windows\System32\drivers\etc\hosts & ipconfig/flushdns > nul
