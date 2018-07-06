# gitskills
一.上传本地项目到git
1、在本地创建一个版本库（即文件夹），通过git init把它变成Git仓库；
2、把项目复制到这个文件夹里面，再通过git add .把项目添加到仓库；
3、再通过git commit -m "注释内容"把项目提交到仓库；
4、在Github上设置好SSH密钥后，新建一个远程仓库，通过git remote add origin https://github.com/guyibang/TEST2.git将本地仓库和远程仓库进行关联；
5、最后通过git push -u origin master把本地仓库的项目推送到远程仓库（也就是Github）上；（若新建远程仓库的时候自动创建了README文件会报错，解决办法看上面）。

二.将git远程库中的项目拉到本地
1.打开终端，cd到自己想要存放项目的文件夹
2.输入git clone url ，url为你要拉取的项目地址

三.如果改动后的项目要上传到github
1.git add 你改动后的文件,如果想要全部上传 git add .
2.执行git commit -m “要添加的注释”
3.git push 上传，可能会让你输入github账号和密码按提示输入即可

四.修改上传的用户名和密码
git config --global user.name "Your Name"
git config --global user.email you@example.com
全局的通过vim ~/.gitconfig来查看
git config user.name "Your Name"
git config user.email you@example.com
