# Git 操作

#### 创建仓库
// cd -> init -> add -> commit -> remote -> push  
cd 根目录  
git init  //建立仓库  
git add . //这个命令会把当前路径下的所有文件添加到待上传的文件列表中。如果想添加某个特定的文件，只需把 . 换成特定的文件名即可  
git commit -m "这里写上提交的注释"  
git remote add origin+你的库链接  
git push -u origin master  

#### 从github拉取仓库 // 本地未init  

cd 目录  
git clone https://xxxxxx 仓库地址  

#### 从remote拉取仓库 // 本地已init  


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




- git reset xxx // changes -> untracked files  
- git status // 查看状态  
- git log // 查看历史日志 - ‘利用好commit’  
