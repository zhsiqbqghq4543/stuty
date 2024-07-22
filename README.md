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
