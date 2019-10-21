    
######     git操作
    bash定位到.get目录
    git clone https://git.lug.ustc.edu.cn/xiaokuan/first.git  克隆远程代码
    git add 文件名 文件名    添加到缓存区
    git commit -m '提交文字描述'   将缓存区里的文件提交到本地仓库
    git pull   		      从远程仓库更新本地仓库
    git push   		      将本地仓库代码推送到远程仓库  (git push -f  强制推送)
    git log    		      查看历史提交信息
    git branch -a         获取远程仓库最新分支状态
    git checkout -b test  新建本地分支（在远程创建需git pull）
    git checkout          分支名称   切换分支  
    git merge  dev        将本地仓库的dev分支合并到本地仓库master分支  
    git push              将本地仓库的master分支，推送到远程仓库的master分支 
    git reset --hard 版本号   回退本地版本号 （git log  查看）

###### 注意：代码推送到远程分支前，一定要pull,就能避免冲掉别人代码的情况

    setting->repositories->Protected Branches  开启或关闭分支保护
    GitLab是一个开源的代码管理平台，可在Linux/unix上安装，供开发者使用，公司内部使用的就是这个

######     扩展：
    解决git提交代码的操作是老要输入密码
    命令：git config --global credential.helper store
