# Github PR提交流程 #

1. [创建一个github账户](https://github.com/)

2. [下载gitbash客户端，并在本地配置github](https://gitforwindows.org/)

   打开gitbash，在终端输入以下命令行（name及email均按照github账户填写）

    git config --global user.name xxx
   
    git config --global user.email xxxxxx@xxx.com

 ![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8201.png)

   创建本地ssh

    ssh-keygen -t rsa -C "xxxxxx@xxx.com" 
 ![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8266.png)

   将ssh配置到Github中

   在mac os X 下前往文件夹，/Users/自己电脑用户名/.ssh。

   windows应该是（C:\Documents and Settings\Administrator\.ssh （或者 C:\Users\自己电脑用户名\\.ssh）中）。

   linux是/home/自己电脑用户名/.ssh


 ![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8203.png)

   用记事本打开id_rsa.pub文件，复制文件内容：
> ssh-rsa XXXXX....XXX
>
>  xxxxxx@xxx.com

   登录github网址，个人账户的settings-SSH and GPG keys，点击New SSH key并粘贴id_rsa.pub文件中内容，点击Add SSH key, title随便写。

   ![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8204.png)

   ![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8205.png)

   验证是否配置成功

    ssh -T git@github.com

![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8207.png)

3.fork开源代码到自己的远程仓库

  ![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8208.png)



4.通过SSH的方法Clone自己的仓库到本地电脑

  ![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8209.png)

    git clone git@github.com:XXXxx

进入到该文件夹下

``` 
cd xxxxxxxxxxx
```

  windows在本电脑C盘/用户/user name中可找到下载到本地文件

5.在projects中生成一个目录，以你们团队命名，并在该目录下生成一个README.md文件，其中包含团队、作品信息及作品github链接，将修改后的文件夹git push至github端

    git add .
    git commit -m 'submit'
    git push 

![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8233.png)

  此时github端就生成了README.md文件

![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8239.png)

6.点击New pull request, 创建一个 PR（pull request）

![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8213.png)

7.在 Github 上将 PR 转成 Draft，之后将所有参赛相关信息放在其中

![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8236.png)

![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8237.png)

8.在个人端完成项目，修改内容

9.当完成作品时请修改 PR 状态为 Ready For Review，会有工作人员合并 PR
![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8238.png)

