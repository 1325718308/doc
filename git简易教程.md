#git 简易教程
##第一步：安装git
###通过以下命令
	$ git	//查看本机是否已经安装了git
	The program 'git' is currently not installed. You can 	install it by typing:
	sudo apt-get install git	//安装git
##第二步：创建版本库
###首先我们需要cd到本机的一个目录下，新建一个目录
	ydzdeMacBook-Pro-2:~ ydz$ cd develop\ files/
	ydzdeMacBook-Pro-2:develop files ydz$ mkdir doc
	ydzdeMacBook-Pro-2:~ ydz$ cd develop\ files/cd coc/
	ydzdeMacBook-Pro-2:doc ydz$ git init
	Initialized empty Git repository in /Users/ydz/develop files/doc/.git/
瞬间Git就把仓库建好了，而且告诉你是一个空的仓库（empty Git repository），细心的读者可以发现当前目录下多了一个.git的目录，这个目录是Git来跟踪管理版本库的，没事千万不要手动修改这个目录里面的文件，不然改乱了，就把Git仓库给破坏了。
##第三步：将本地的版本库添加到远程仓库
###通过浏览器打开gitup,登录自己的账号，然后创建一个repository

![](https://github.com/1325718308/doc/blob/master/images/001.jpeg)


![](https://github.com/1325718308/doc/blob/master/images/002.jpeg)

###至此远程仓库已经创建完成，接下来要做的就是将本地版本库与远程仓库关联。
	git commit -m "first commit"
	git remote add origin https://github.com/1325718308/doc.git
	git push -u origin master
	
至此本地版本库已经与远程仓库关联成功了。


	