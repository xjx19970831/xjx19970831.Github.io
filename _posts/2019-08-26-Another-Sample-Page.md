---
title: 兄弟会-第五天--日报
published: true
---

   1. 权限

        ls  -l     查看文件权限

        ls          查看文件

        chmod   修改文件权限  (所有者或root可以改)                 　　　　　　　 所有者，所有组，其他人

        chmod  -R改变目录下所有文件权限

        ​    　

         r  = 4,w = 2, x = 1

      rwx作用到文件：

      　　　　r:可以读取查看

      　　　　w：可以修改
      
      ​                  x: 可以执行
      
      rwx 作用到目录：  　
      
        　  　     r:可以读取，ls查看目录内容
      
      　　　　w :可以修改，目录内创建，删除，重命名目录
      
      　　　　x：可以进入该目录
      
      ​                  
      
      ​     例：rwxrw-r--       764                 　　　　chmod  764  haha
      
      ​                                                                                  ls  -l    haha
      
      ![](/home/chenjiaxing/图片/2019-08-24 14-45-51 的屏幕截图.png)

２．权限管理－－权限转让

　　　2.１　用root新建一个文档　touch  kkk

​              2.2    新建一个用户　　　useradd   xiaoming

​               2.3   转让用户　　　　　chown   xiaoming   kkk

​               2.4   查看权限　　　　　ls  -l   kkk

  ３.   新建账户

　　　　root 下　　　useradd    xiaoming

​                 查看用户　　　cd    /home                    ll

​      ４. 删除用户　　　

　　　　　userdel     xiaoming

   5 .  查询用户信息　

　　　　　　id   xiaoming

  6  .    切换用户,从权限高的切换到权限低的用户，不需要密码，反之需要，exit退出

​       su -  xiaoming    

　7 . 用户组

　　增加组　　　groupadd    tongxue

​          删除组　　　groupdel    tongxue

​          增加用户时直接加上组　　　useradd   -g    xiaoming   tongxue

​          修改用户组　　　usermod    -g    shaolin   zhangshanfeng        

​            修改文件所在的组　　chgrp  tongxue   nihao.txt            

7 .1 其他组　　除文件的所有者和所在组用户外，系统的其他用户都是都是文件的其他组。　

8 . 文件信息　　 都在home目录下　　cd   /home

　　用户配置文件（用户信息）　cat　　　　/etc/passwd

​        组配置文件（组信息）　　　　cat　　　/etc/ group

​        口令配置文件（密码和登录信息。加密的）cat     /etc/shadow　　    

９ . 压缩解压

 　　压缩　　　　　gzip     文件　　　　         　.gz后缀　

　　解压　　　　　gunzip   文件

​    10 . 组管理和权限管理

　        



 





