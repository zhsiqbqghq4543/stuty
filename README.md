# 前言

## 1.新建仓库+拉取

```shell
1. `mkdir workspace` #在linux环境下新建一个文件夹(假设名字是workspace)
2. `cd workspace` #进入
3. `git init` #初始化git环境
4. `git clone git@github.com:zhsiqbqghq4543/stuty.git` #在界面点击ssh然后复制
5. 成功拉取到本地
```

## 2.加ssh密钥命令

```shell
1. `ssh-keygen -t rsa` #一路enter, 不要输入密码
2. `ssh-add ~/.ssh/id_rsa` #
3. `eval `ssh-agent` #
4. `cat ~/.ssh/id_rsa.pub` #然后将显示的公钥复制填入
5. `git clone ...`
```

## 3.把下面复制然后扔进gpt

```shell
(base) ykxcai@ykxcaideMacBook-Pro-2 stuty % ls
README.md       learnGit        learnShell
(base) ykxcai@ykxcaideMacBook-Pro-2 stuty % git status
位于分支 main
您的分支与上游分支 'origin/main' 一致。

尚未暂存以备提交的变更：
  （使用 "git add <文件>..." 更新要提交的内容）
  （使用 "git restore <文件>..." 丢弃工作区的改动）
        修改：     README.md

未跟踪的文件:
  （使用 "git add <文件>..." 以包含要提交的内容）
        learnGit/
        learnShell/

修改尚未加入提交（使用 "git add" 和/或 "git commit -a"）
(base) ykxcai@ykxcaideMacBook-Pro-2 stuty % git add learnGit/  learnShell/  README.md
(base) ykxcai@ykxcaideMacBook-Pro-2 stuty % git commit -m "20240722"
[main 9531374] 20240722
 Committer: 1592226240@qq.com <ykxcai@ykxcaideMacBook-Pro-2.local>
您的姓名和邮件地址基于登录名和主机名进行了自动设置。请检查它们正确
与否。您可以对其进行设置以免再出现本提示信息：

    git config --global user.name "Your Name"
    git config --global user.email you@example.com

设置完毕后，您可以用下面的命令来修正本次提交所使用的用户身份：

    git commit --amend --reset-author

 3 files changed, 107 insertions(+), 2 deletions(-)
 create mode 100644 learnGit/learnGit.md
 create mode 100644 learnShell/learnShell.md
(base) ykxcai@ykxcaideMacBook-Pro-2 stuty % git push
总共 0（差异 0），复用 0（差异 0），包复用 0
To github.com:zhsiqbqghq4543/stuty.git
   0231c97..9531374  main -> main
(base) ykxcai@ykxcaideMacBook-Pro-2 stuty % 
```
