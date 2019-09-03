---
title: 兄弟会-复习
published: true　　
---

# git 



```
git clone

git init        创建一个空的Git仓库或者初始化一个已存在的仓库

git add         添加文件内容至索引

git mv          移动或重命名一个文件 目录或符号链接

git reset       重置当前 HEAD 到指定状态

git rm          从工作区和索引中删除文件

git status      显示工作区状态

git branch -d XXX 删除

git branch -vv 查看已设置的跟踪分支

git branch -v  查看每个分支最后一次提交

git branch --merged 查看与所在分支合并了的分支

git branch --no-merged

git checkout xxx   切换到xxx分支当下

git checkout -b xxx 创建xxx分支

git diff XXX

git merge experiment 分支执行合并

git checkout master  
git merge experiment   
 将experiment分支,与master合并

git rebase XXX 重新绑定XXX分支

git fetch --all
git branch -vv  从另一个仓库下载对象和引用

git pull [远程储存库] [想要弄来的分支]  
获取并整合另外的仓库或一个本地分支 

git push origin --delete XXX 想要从服务器删除XXX分支

git push
```

## vim篇

```
n<space>    移动光标所在位置的后20个字符距离

G  移动到这个档案的最后一行

nG 移动到第 n 行

gg 移动到这个档案的第一行

n<Enter> 光标向下移动n行

/word 沿光标向下搜索

n 重复前一个搜索动作

$s/word1/word2/g 第一行到最后一行寻找 word1 
字符串,并替换成Word2

$s/word1/word2/gc 单个替换

dd 删除光标所在行

ndd 删除光标向下n行

yy 复制光标所有行

nyy 何止光标所在向下n行

p,P 粘贴下 粘贴上

u 复原前一个动作

Ctrl + r 重做上一个动作

. 重复前一个动作的意思
```

## Linux操作命令

```
find ./ -name "*XXX*"

sudo find ./ -name "*name*"

find ./ -name "[A-Z]*"

pwd

cd

ls

cat 合并文件、显示内容

grep 查找字符串

touch 创建一个空白文件

cp 拷贝    cp 源文件 目标文件

mv 移动文件

rm 删除文件

rmdir 删除文件夹

mount 挂载文件系统

umount 卸载已挂载上的文件系统

df 检查硬盘分区和已挂上的文件系统的磁盘空间

du 显示文件目录和大小

fsck 检查和修复

压缩

tar -zcvf xxx.tar.gz 

tar -jcvf xxx.tar.bz2

zip zzz.zip


解压

tar -xvf xxx.tar.gz

tar -jxvf xxx.tar.bz2

unzip zzz.zip


shutdown

reboot

ps  查看目前程序执行情况

top 查看目前程序执行情况和内存使用情况

kill 终止进程

date 查看日期

cal 显示日历

chmod 改变权限

su    修改用户

useradd 添加用户

man 查询,解释一个命令

locate 定位文件和目录

whatis 寻找命令的含义

head   查看文件头部

tail   查看文件尾部

less , more 分页工具

ftp    传输文件

bye    结束连线并结束程序

ping   检测主机

telnet 远程登录

rlogin 远程登入

netstat 查看网络情况

which  从path环境变量寻找,显示路径名称

whereis 找出可执行文件,源代码文件

locate 带记忆的文件搜索

updatedb 更新数据库

echo 打印

clear 清除

passwd 密码
```