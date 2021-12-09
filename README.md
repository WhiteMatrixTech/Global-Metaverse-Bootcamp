## Github PR Submission Guide ##

 **PR Submission Deadline: 2021.Dec.23rd 00:00 PST(2021.Dec.18th 08:00 UTC)** 

**1. [Create a Github account.](https://github.com/)**

**2. [Download Git BASH Client](https://gitforwindows.org/) and complete Github configuration in local environment.**

   Open Gitbash Terminal.

   Enter the following command line in the terminal (name and email are filled in according to the github account).

    git config --global user.name xxx
   
    git config --global user.email xxxxxx@xxx.com

 ![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/Gitconfig.png)

   Create a local SSH —— Secure Shell.

    ssh-keygen -t rsa -C "xxxxxx@xxx.com" 
 ![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/Gitlocalssh.png)

   Configure SSH into Github Settings.

> **Linux**: /home/username/.ssh
> 
> **Mac**:  /Users/username/.ssh
> 
> **Windows**: C:\Documents and Settings\Administrator\.ssh **OR** C:\Users\username\\.ssh


 ![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/SSH_File.png)


Open the file **id_rsa.pub** with Notepad and copy the content.
> ssh-rsa XXXXX....XXX
>
>  xxxxxx@xxx.com

   Go to github and login your account.

   Find "SSH and GPG keys" in personal account settings.

   Click "New SSH key" and paste the content from the file "id_rsa.pub". 

   Then, click "Add SSH key". There is no any specific requirement for title.

   ![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/GithubSettings.png)

   ![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/SSH+and+GPG+keys.png)

Validate if the comfiguration is successful.

    ssh -T git@github.com

![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/SSH_Validation.png)

**3.Fork the open-source codes into the personal remote repository.**

Repository URL: [https://github.com/WhiteMatrixTech/Gobal-Metaverse-Bootcamp](https://github.com/WhiteMatrixTech/Gobal-Metaverse-Bootcamp)

  ![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8208.png)


**4.Clone personal github repository into local environment via SSH.**

  ![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/Code_Clone_SSH.png)

    git clone git@github.com:XXXxx

  Enter the destination folder.

``` 
cd xxxxxxxxxxx
```

  The downloaded folder in Windows can be checked in the route below.
  
> C:\Users\user name\Global-Metaverse-Bootcamp\

**5.Create a folder named by your team name under projects. Generate a README.md file which contains the information of your team, your project and the link to your github repository.**

	Team Number:
	Job Allocation:
	Project Intro:
	Video Link:
	Repository Addr:
	(Repository must contain ppt slides.)

Use the command line "git push" to upload the project folder to github.

    git add .
    git commit -m 'submit'
    git push 

![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/GitPush.png)

  Then, the README.md file can be seen on the github repository.

![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/Github_README.png)

**6.Click "New pull request" and create a PR(Pull Request).**

![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8213.png)

**7.Convert PR into Draft where all the match-related resources should be placed.**

![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/ConvertPR2Draft.png)

![](https://chainide-forum-img.s3.ap-northeast-1.amazonaws.com/8237.png)

**8.Accomplish the project and submit.**

**9.Convert the status of PR into "Ready For Review" as long as the submission has been done. Bootcamp staff will merge all the PRs.**
![](https://chainide-global-metaverse-bootcamp-pr-img.s3.ap-northeast-1.amazonaws.com/Ready4View.png)

