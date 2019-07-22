# 百度前端学院MVVM学习日志
***
### 第一堂课 熟悉Git使用
* 配置用户名_邮箱 <br>
    git config --global user.name '' <br>
    git config --global user.email ''

* 克隆远程仓库 <br>
    git clone '' <br>
    （克隆版本库的时候，所使用的远程主机自动被Git命名为origin）如果要使用其他主机名<br> 
    git clone -o ''

* 分支管理 <br>
    * 列出/创建/删除分支: git branck <参数> <分支名>
    （都无参数列出现有分支 有参数名创建分支 -d 删除分支）
    * 切换分支： git checkout <参数><分支名> （-b 创建并立即切换到）
    * 合并分支： git merge <分支名> 将分支合并到主分支中
    （同文件名不同文件内容时会出现合并冲突，手动 git add 解决）
    * 标签： git tag <参数><分支名> （-a 标签加注释 -d 删除标签）
    git show <标签> 产看标签的版本改动

* 管理远程主机名
    * git remote 命令列出所有远程主机
    * git remote -v 查看远程主机的网址
    * git remote show <主机名> 查看该主机的详细信息

+ 远程主机的版本库有了更新（commit）取回本地的操作
    * git fetch <远程主机名> <br>
    通常用来查看其他人的进程，对本地代码没有影响 <br>
    * 如果要与本地分支合并（改变本地代码）
    git pull <远程主机名><远程分支名>:<本地分支名>