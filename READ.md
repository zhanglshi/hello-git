github不能访问,ping不通github.com解决办法
https://blog.csdn.net/sdta25196/article/details/80203152

翻墙的锅：解决办法如下
打开 hosts文件，地址：C:\Windows\System32\drivers\etc 
然后在hosts文件中添加：
192.30.253.112 github.com
151.101.88.249 github.global.ssl.fastly.net


关于Git增、删、改源地址问题
https://www.cnblogs.com/BHfeimao/p/6496877.html

1.如何查看当前远程Git库源地址呢？
$git remote -v
$git remote -version
//以上两种方法都是查看当前Git库源地址的
 
2.这时如果你想修改当前的源地址：
$git remote set-url origin [GIT URL]
//orgin为当前源地址名，[GIT URL]为欲修改源地址

3.添加一个新的Git库源地址：
$git remote add [NAME] [GIT URL]
//[NAME]为新的Git库源地址名，[GIT URL]为新的git库源地址

4.删除一个Git库源地址：
$git remote remove [NAME]
$git remote rm [NAME]
//[NAME]为Git库源地址名
