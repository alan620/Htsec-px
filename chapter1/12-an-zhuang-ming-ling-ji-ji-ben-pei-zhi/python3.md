### Python3

#### CentOS7

执行安装命令：

```
yum install python3 python3-pip
```

![](/assets/python31.png)

查看版本：

```
python3
pip3 --version
```

![](/assets/python32.png)

注意：如果`command not found`，添加软链接：

```
ln -s /usr/bin/python3.6 /bin/python3
ln -s /usr/bin/pip3.6 /bin/pip3
```

#### CentOS6

执行安装命令：

```
yum install python36u python36u-pip
```

其余同上

