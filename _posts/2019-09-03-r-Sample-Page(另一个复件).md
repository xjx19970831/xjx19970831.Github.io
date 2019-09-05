---
title: 兄弟会-复习
published: true　　
---

# 



```
* {
	margin:0;
	padding:0;
}
.small_box {
	width:180px;
	height:180px;
	margin-left:10px;
	margin-top:10px;
	position:relative;
}
.small_box img {
	width:180px;
	height:180px;
}
.small_box .mask {
	position:absolute;
	width:100%;
	height:100%;
	background:rgba(0,0,0,0.5);
	opacity:0;
	z-index:2;
	cursor:move;
}
.small_box .float_layer {
	position:absolute;
	width:80px;
	height:80px;
	background:rgba(0,0,0,0.5);
	display:none;
}
.big_box {
	position:absolute;
	left:200px;
	top:10px;
	width:180px;
	height:180px;
	overflow:hidden;
	display:none;
}
.big_box img {
	position:absolute;
}
```

## 

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="cssha.css">
  
</head>
<body>
        <div class="small_box">
                <span class="mask"></span>
                <span class="float_layer"></span>
                <img src="/home/chenjiaxing/图片/2019-09-05 13-32-53 的屏幕截图.png">
            </div>



            <div class="big_box">
                <img src="/home/chenjiaxing/图片/2019-09-05 13-32-53 的屏幕截图.png"  >
            </div>
            <script src="/home/chenjiaxing/bao/jQ/jquery-3.3.1.js" ></script>


            <script src="/home/chenjiaxing/bao/jQ/jquery-3.3.1.js" ></script>
            <script>
                $(".mask").mouseover(function() {
    $(".float_layer").show()
    $(".big_box").show()
})
$(".mask").mouseout(function() {
    $(".float_layer").hide()
    $(".big_box").hide()
})
$(".mask").mousemove(function(e) {
    var l = e.pageX - $(".small_box").offset().left - ($(".float_layer").width() / 2)
    var t = e.pageY - $(".small_box").offset().left - ($(".float_layer").height() / 2)
    if (l < 0) {
        l = 0
    }
    if (l > $(this).width() - $(".float_layer").width()) {
        l = $(this).width() - $(".float_layer").width()
    }
    if (t < 0) {
        t = 0
    }
    if (t > $(this).height() - $(".float_layer").height()) {
        t = $(this).height() - $(".float_layer").height()
    }

    $(".float_layer").css({
        "left": l,
        "top": t
    })
    var pX = l / ($(".mask").width() - $(".float_layer").width())
    var pY = t / ($(".mask").height() - $(".float_layer").height())
    $(".big_box img").css({
        "left": -pX * ($(".big_box img").width() - $(".big_box").width()),
        "top": -pY * ($(".big_box img").height() - $(".big_box").height())
    })
})
            </script> 
</body>
</html>
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

```
pwd      显示当前目录
cd       改变目录
grep    在文件中查找某个字符
touch   创建文件
rm  删除文件
ls        查看内容
cp    复制文件
cat    查看文件内容
mv   移动文件
redir    删除目录
mount    挂载磁盘
umount   卸载挂载
df        检查磁盘分区和已经挂载上来的文件系统的磁盘空间
du    显示文件目录和大小
fsck    检查修复linux文件系统
zip/unzip    解压缩
gzip/gunzip   解压缩
bzip2/bunzip2　解压缩
tar      　　　　　创建备份和归档
shutdown     关机
reboot    重启
ps    查看目前程序执行情况
top   查看目前程序执行情况和内存使用情况
kill   终止一个进程
date   查看日期
cal   显示日历
chmod   修改用户权限
su  修改用户
useradd   增加用户
man   查看用法
locate   定位文件和目录
whatis    查找某个命令的含义
head    查看文件的开头部分
tail       查看结尾
less  /more   分页查看
ftp   传送文件
bye   结束连线结束程序
ping   检测主机
netstat   显示网络状态
telnet   远端登录
rlogin   远端登入
updatedb   更新索引数据库
whereis   找出特定程序的可执行文件，源代码以及路径
find   按条件收缩　并执行一定的动作
locate   带记忆的文件搜索
passwd   修改密码
echo  显示一字串
clear  清除显示器
lpq    查看在打印列队中等待的作业
lpr   打印
lprm  取消打印


```

