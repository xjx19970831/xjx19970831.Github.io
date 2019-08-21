---
title: 兄弟会-第四天--操作远程库
published: true
---

### 远程库与本地库交互

1. 克隆远程库到本地  - 

   - git init    初始化
   - git clone +远程库的地址    完成克隆

2. 本地信息提交到远程库  完成一次交互    

   - git  remote -v   查看连接信息
   - git remote origin +远程库地址
   - git remote -v   再次检查
   - git pull origin master  提交之前最好拉取一下
   - git push origin master   提交
   - git remote rm origin  删除连接

   3. 查看分支：`git branch`
   
      ​        创建分支：`git branch <name>`
   
      ​        切换分支：`git checkout <name>`
   
      ​        创建+切换分支：`git checkout -b <name>`
   
      ​        合并某分支到当前分支：`git merge <name>`
   
      ​        删除分支：`git branch -d <name>`
   
   4. git reset --hard 值
   
   5. git reflog  查看命令历史
   
   6. git rm --cashed 文件名   取消跟踪
   
   7. git  diff 查看区别
   
   8. git rm 文件名     删除文件
   
   
   9.





 





