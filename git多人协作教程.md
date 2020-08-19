## git多人协作教程



##### 1.总结：

在本地的每个分支都与远程的分支有个链接。可以通过

git checkout -b 本地分支 origin/远程分支 

来让本地分支和远程分支链接在一起，还可以

git clone 

与主分支有个链接，同时可以通过

$ git branch --set-upstream-to=origin/<branch>  本地分支 

来链接，现在有三种方法可以链接

##### 2、其他

1、git push origin 远程分支

2、链接后可以直接使用git pull

3、当你从远程分支拉取时，在本地更改内容之后准备push时，如果远程分支发生了改变，就push不了。需要git pull 当然git pull需要有链接，之后会有冲突，手动解决后就可以push了。

