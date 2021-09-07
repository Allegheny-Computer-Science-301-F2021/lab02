
## cs301Fall2021-lab02

## DUE by 3:00pm, September 25th

## Introduction

Designed for use with [GitHub Classroom](https://classroom.github.com/), this repository contains the starter files for a class activity one.

In this class we will use GitHub for all course materials and most of the assignments. We will also use Markdown for writing. This activity invites students to explore the use of GitHub and to learn to use Markdown language as they reflect on an assigned article.

## Tasks

 - First, please familiarize yourself with GitHub. For example, [Git Handbook](https://guides.github.com/introduction/git-handbook/) provides a good reference guide.

 -  Then, clone your lab repository locally to your computer. To do so, click on "Code" button in your lab  repository's Web page, then make sure "HTTPS" is selected (unless you have previously set up SSH keys), and copy the displayed command.

 - Next, open your terminal window, navigate to a folder/directory where you would like to store this course's materials, and paste the command you copied in a previous step.

 - Now you can explore Markdown by using [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) as a guide. You can also watch a video on [Markdown Tidbits](https://www.youtube.com/watch?v=cdJEUAy5IyA&list=PLsYZRXov75ZHSwWiCk0-jd1RcTuu_-zmD&index=5).

 - Complete your `writing/part1.md` for Part1.

 - Complete your website with the requirements of the lab.

 - Issue your site link in the course Discord channel.

 - Complete `writing/part2.md` for Part2.


 - As you work, use the commands, `commit` and `push` to push your work to GitHub. The commands are below and are to be used in your terminal window. Please make sure you are in your lab directory when you type these commands.

	- `git add .` OR 	`git add -A`

	- `git commit -m "Replace this text with your own commit message"`

	- `git push`

 - Refresh your Web browser with your repository on GitHub and make sure that you see your changes have been committed correctly.


 - Do not use a word processor such as Google Docs, Word or Libreoffice for your writing. Instead, please write in a text file using the Markdown styling syntax.


## GitHub and Markdown
 If you have not done so already, please read all of the relevant [GitHub Guides](https://guides.github.com/) that explain how to use many of the features that GitHub provides. In particular, please make sure that you have read the following GitHub guides: [Mastering Markdown](https://guides.github.com/features/mastering-markdown/), [Hello World](https://guides.github.com/activities/hello-world/), and [Documenting Your Projects on GitHub](https://guides.github.com/features/wikis/). Each of these guides will help you to understand how to use both [GitHub](http://github.com) and [GitHub Classroom](https://classroom.github.com/).


 ### Running GatorGrader Locally

 To run GatorGrader locally to see if your solution satisfies minimal writing requirements of the lab,
 once you have installed [Docker Desktop](https://www.docker.com/products/docker-desktop),
 you can use the following `docker run` command to start `gradle grade` as a containerized application, using the [DockaGator](https://github.com/GatorEducator/dockagator) Docker image available on [DockerHub](https://cloud.docker.com/u/gatoreducator/repository/docker/gatoreducator/dockagator).



### Mac:

 ```bash
 docker run --rm --name dockagator \
   -v "$(pwd)":/project \
   -v "$HOME/.dockagator":/root/.local/share \
   gatoreducator/dockagator
 ```
Note: you may need to remove the .dockagator directory before running the above. If there are problems, run `rm ~/.dockagator/` and try the command again.



### Linux:
```
sudo docker run --rm --name dockagator \
	-v "$(pwd)":/project \
	-v "$HOME/.dockagator":/root/.local/share \
	gatoreducator/dockagator
```

Note: you may need to remove the .dockagator directory before running the above. If there are problems, run `rm ~/.dockagator/` and try the command again.

 The command above will use `"$(pwd)"` (i.e., the current directory) as the project directory and `"$HOME/.dockagator"` as the cached GatorGrader directory. Please note that both of these directories must exist, although only the project directory must contain something. Generally, the project directory should contain the source code and technical writing of this assignment, as provided to a student through GitHub. Additionally, the cache directory should not contain anything other than directories and programs created by DockaGator, thus ensuring that they are not otherwise overwritten during the completion of the assignment. To ensure that the previous command will work correctly, you should create the cache directory by running the command `mkdir $HOME/.dockagator`.

 If you are running your program on a Windows Operating System, you should run the following command instead, replacing the word "user" with the username of your machine:

 ```bash
 docker run --rm --name dockagator -v "%cd%":/project -v "C:\Users\user/.dockagator":/root/.local/share gatoreducator/dockagator
 ```


Please ask questions as necessary.
