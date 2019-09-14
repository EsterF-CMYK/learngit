Git is a distributed version control system.
Git is free software.


/*安装git之后的设置*/
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"


/*创建git仓库*/
$ mkdir learngit   //创建新目录
$ cd learngit    //进入新目录
$ pwd  //显示当前位置
/Users/michael/learngit
$ git init  //将该目录变成Git可以管理的仓库
Initialized empty Git repository in /Users/michael/learngit/.git/

/*提交*/
$ git add readme.txt   //无提示
$ git commit -m "wrote a readme file"
[master (root-commit) eaadf4e] wrote a readme file
 1 file changed, 2 insertions(+)
 create mode 100644 readme.txt
 
使用命令git add <file>，注意，可反复多次使用，添加多个文件；
使用命令git commit -m <message>，完成。


/**/
HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id。
穿梭前，用git log可以查看提交历史，以便确定要回退到哪个版本。
要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。