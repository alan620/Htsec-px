### GCC&G++

#### CentOS7

执行安装命令：

```
yum install devtoolset-9-gcc devtoolset-9-gcc-c++ devtoolset-9-binutils
```

![](/assets/gcc1.png)

临时使用`gcc9`：

```
source /opt/rh/devtoolset-9/enable
```

永久使用`gcc9`：

```
echo "source /opt/rh/devtoolset-9/enable" >>/etc/profile
```

查看版本：

```
gcc -v
g++ -v
```

![](/assets/gcc2.png)

#### CentOS6

同上



