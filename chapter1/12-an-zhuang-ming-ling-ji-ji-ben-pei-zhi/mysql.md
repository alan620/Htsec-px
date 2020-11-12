### MySQL

#### CentOS7

首先卸载MySQL低版本和MariaDB：

```
rpm -qa | grep mysql* mariadb*，yum remove mysql* mariadb*
```

删除所有mysql的目录

```
find / -name mysql
rm -rf 以上
```

![](/assets/mysql1.png)

使用脚本进行安装：

```
wget -P /root/ http://172.190.92.118/package/htsec7/mysql8.sh
```

#### ![](/assets/mysql2.png)

执行脚本：

```
sh /root/mysql8.sh
```

#### ![](/assets/mysql3.png)

启动mysqld：

```
systemctl start mysqld
```

![](/assets/mysql4.png)

查看默认密码：

```
cat /var/log/mysqld.log | grep password
```

![](/assets/mysql5.png)

登录mysql：

```
msyql -u root -p 默认密码
```

![](/assets/mysql6.png)

修改默认密码：

```
ALTER USER 'root'@'localhost' IDENTIFIED BY '新密码';
```

![](/assets/mysql7.png)

#### CentOS6

使用脚本进行安装：

```
wget -P /root/ http://172.190.92.118/package/htsec6/mysql8.sh
```

其余同上

备注：如果安装失败，检查是否已经全部删除已安装的MySQL和MariaDB及其目录。

