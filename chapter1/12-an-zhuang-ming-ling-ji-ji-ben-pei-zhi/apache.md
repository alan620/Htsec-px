### CentOS7

执行安装命令：

```
yum install httpd 
```



查看版本：

```
httpd -v
```

### CentOS6

执行安装命令：

```
yum install httpd24*
```

默认安装路径：

```
/opt/rh/httpd24/root
```

添加配置文件链接：

```
ln -s /opt/rh/httpd24/root/etc/httpd/conf/httpd.conf /etc/httpd.conf
```

添加二进制命令链接：

```
ln -s /opt/rh/httpd24/root/usr/bin/* /usr/local/bin
```

```
ln -s /opt/rh/httpd24/root/usr/sbin/* /usr/local/sbin
```



