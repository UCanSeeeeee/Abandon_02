# Git 操作

#### 创建仓库 && 第一次提交
// cd -> init -> add -> commit -> remote -> push  
cd 根目录  
git init  //建立仓库  
git add . //这个命令会把当前路径下的所有文件添加到待上传的文件列表中。如果想添加某个特定的文件，只需把 . 换成特定的文件名即可  
git commit -m "这里写上提交的注释"  
git remote add origin+你的库链接  
git push -u origin master  

#### 第二次及以后提交  

cd 文件  
git add .  
git commit -m ''  
git push   

#### 从github拉取仓库 // 本地未init  

cd 目录  
git clone xxxxxx // 仓库地址  

#### 从remote拉取仓库 // 本地已init  

cd 目录  
// git status  
git pull  

#### 获取历史版本  

git log  
git checkout commit(id)  
// git branch // 检查此时所在分支  
// 若...，则此时获取想要的文件后再回到master即可  
git checkout master  
// 而后操作根据需求进行  

#### 获取误删文件 // master && 未commit  
git status  
git restore xxx  

<<<<<<< HEAD
#### 分支  
git branch xxx // 分支名字  
...  
git checkour master  
git merge xxx // 分支名字  

#### tag // 版本控制,相当于commit id
(1)  
git tag 2.0.0 -m ''  
(2)  
git log  
git checkout xxx // commit id  
git tag 2.0.0 -m ''  

#### 解决冲突  // 结果是两次commit.  

// git push 未成功后  
git pull // 提示出现冲突  
解冲突  
git add .  
git commit -m ''  
git push  

#### 未知解决冲突的知识点(先记录一下，用到的时候再重写这一部分)  
- 冲突  
git fetch origin main  
git rebase origin main   
- 解决冲突  
git add .  
git rebase --continue  
git push  

#### 解释  
- git reset xxx // changes -> untracked files  
- git status // 查看状态  
- git log // 查看历史日志 - ‘利用好commit’  
