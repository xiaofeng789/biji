
#useradd
添加用户:  useradd  
****

#userdel
userdel  name  不会删除主目录
-r  删除主目录
****

#passwd
passwd   name
passwd  -l  name 锁用户
passwd  -u  name 锁用户
passwd        -d清除密码 
***

#ctrl\+alt
切换终端界面
ctrl+alt+f2：
f7切换图形界面
echo  roger
直接设置密码给roger
echo 密码  |  passwd  --stdin  roger
****

#usermod
usermod  -c    
修改主目录
usermod  -d  /home/roger1 roger
更改shell
usermod -s  /sbin/nologin roger

***seradd***也可以用对应的参数，直接设置

截至日期
添加用户:usermod -e 2023-12-31 roger

#用户用户组

root:  x:  0:  0:  root:  /root:  /bin/bash
用户名:是否有密码:用户id:组id:用户描述:用户主目录:shell
-rw-------. 1 root root 1432 Sep  5 14:49 anaconda-ks.cfg
 
                    用户 用户组
创建用户组：groupadd   XXGC
id  name
![[Pastedimage20230926104743.png]]
