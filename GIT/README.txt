1.先在终端上面配置用户名和邮箱
git config --global user.name 'tangshi706'
git config --global user.email '364244432@qq.com'
2.初始化git让其产生.git的文件夹
git init
3.添加文件到缓冲区
git add 文件名
注意：要是文件夹则需要把路径包括
git add scripts/  #这就表示上传文件夹scripts
4.给上传的文件/文件夹添加说明性文字
git commit -m "说明性文字"
5.和远程的仓库建立连接
git remote add origin 仓库地址
这里origin只是初次上传的，也只有文件初次上传才需要进行连接，下次这不需要
6.同步仓库和本地
git pull --rebase origin master
或者
git pull origin master
7.上传到远程的仓库
git push origin master
注意：我们第一次推送master分支时，加上了 –u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令
git push -u origin master
详细参考下面网站：
https://blog.csdn.net/u011535541/article/details/83379151
