# Git 操作

#### 创建仓库

cd 根目录
git init  //建立仓库
git add . //这个命令会把当前路径下的所有文件添加到待上传的文件列表中。如果想添加某个特定的文件，只需把 . 换成特定的文件名即可
git commit -m "这里写上提交的注释"
git remote add origin+你的库链接
git push -u origin master