Git is a distributed version control system.
Git is free software distributed under the GPL.
Git has a mutable index called stage.
Git tracks changes of files.
Creating a new branch is quick AND simple.

My new learn git.

// 初始化一个Git仓库
git init

// 第一步，先添加 Add
git add file1.txt

git add file2.txt file3.txt

// 第二步，再提交 commit
git commit -m "add 3 files."

// 查看库的当前状态
git status

// 查看修改内容
git diff

// 查看修改提交记录
git log
git log --pretty=oneline

// 查看命令历史
git reflog

// 回退到指向版本
// HEAD指向当前版本，HEAD~1代表上一个版本，以此类推，HEAD~100
// 也可以commit_id号，可以写开始不重复的几位
git reset --hard commit_id

// 用版本库里的版替换工作区的版本
git checkout -- file

// 删除文件
git rm

// gitHub
// 添加远程库
git remote add origin git@github.com:NathanWorld/gitStudy.git

// 推送本地库的所有内容到远程库
// 第一次需加 -u 参数
git push -u origin master
git push origin master

// 克隆远程库到本地
git clone git@github.com:NathanWorld/gitskills.git

// 查看分支
git branch 

// 创建分支
git branch <name>

// 切换分支
git chectout <name>

// 分支 -b 表示创建并切换分支
git checkout -b <name>

// 合并分支, 将分支dev上的工作成果合并到master分支上
// 合并某分支到当前分支
git merge <name>

//删除分支
git branch -d dev
