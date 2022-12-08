# GIT复习  
  
## 起步  
  
### 三种区  
  
* 工作区（ workspace ）、暂存区（ Index/Stage ）、repository  
  
### 三种状态  
  
* …  
  
### 流程  
  
* 工作区修改文件  
    * 更改完暂存  
        * 提交将暂存区文件储存到仓库  
  
### .gitconfig是git全局变量配置文件，配置用户名邮箱这些  
  
## 基础  
  
### 如何获取仓库  
  
* 1.本地创建  
    * 切到文件夹下，执行git init，生成一个.git隐藏文件  
* 2.远程克隆  
    * git clone git@github.com:zhangsensen7/nft.git  
  
### 工作区  
  
* 可能存在的所有文件状态  
    * 未被git管理（未跟踪untracked）  
        * 未跟踪会有两个红色？？  
    * 已管理  
        * 未修改（unmodified）  
            * 工作中工作区都要处于未修改状态  
        * 已修改（modified）  
        * 已暂存（staged）  
  
### git status 查看文件状态  
  
* git status -s（简写）  
  
### git add跟踪  
  
* 功能  
    * 1.跟踪新文件  
        * 绿色的A  
    * 2.已修改的文件，放到暂存区  
        * 修改一下index内容，执行git status -s  
            * 红色的M  
                * 通过git add 放到暂存区  
                    * 绿色M  
        * 放多个修改过的文件到暂存区  
            * git add .(常用)  
    * 3.冲突文件标记为已解决  
  
### git commit -m （从暂存区出发）提交到仓库  
  
* 提交第一次跟踪的文件  
* 提交已暂存的文件  
  
### git checkout -- index.html撤销工作区文件的修改，无法还原！  
  
* 本质是还原仓库保存的版本  
  
### git reset HEAD index.html 取消暂存区文件  
  
* …  
  
### git commit -a - m 从工作区直接到仓库  
  
### 移除文件  
  
* …  
  
### 忽略文件  
  
* …  
    * Glob模式（简化正则）  
        * …  
            * 举例子  
                * …  
  
### git log 查看提交历史  
  
* git log -2  
* git log -2  
* git log -2 -- pretty=oneline  
  
### git reset --hard 回退到指定版本  
  
* git reset --hard b7b73af7cd248746ee673e9e3b658761ce9f88be  
    * …  
  
## 分支  
  
### 本地仓库上传到github  
  
### 创建和切换  
  
* git branch  
    * 直接执行  查看所有分支  
    * git branch 分支名称，基于当前分支创建新的分支，（本质复制了一份）  
        * 注意创建完还是在当前分支  
* git checkout 分支名字  
    * 快速创建并切换  
        * git check -b 分支名称  
  
### 合并分支  
  
* 1.先切回master  
    * 2.在master上执行 git merge 分支名称  
  
### git branch -d  
  
* 删除分支  
    * 分支合并完没用了  
        * 注意删的时候不能在当前分支，最好站在master上  
  
### 冲突合并  
  
* 两个分支对同一个文件做了不同的修改  
    * …  
        * …  
            * …  
  
### 第一次提交本地分支到远程仓库 git push -u origin 分支名字  
  
* …  
    * 以后直接git push  
  
### git remote show  origin（默认名字）远程仓库名字  
  
* 展示远程仓库所有分支  
  
### 跟踪分支（拉取远程分支）git check 分支名  
  
* …  
    * …  
  
### 更新分支拉取最新代码  
  
* git pull  
    * …  
  
### 删除远程分支  
  
* …  
  
## …  
  
## …  
  
