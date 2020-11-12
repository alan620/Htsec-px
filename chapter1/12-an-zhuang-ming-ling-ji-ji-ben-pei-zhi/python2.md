### Python2

#### CentOS7

执行安装命令：

```
yum install python python-tools python-pip
```

查看版本：

```
python
```

#### ![](/assets/python1.png)

#### CentOS6

备注：如有特殊需求，需在centos6上实现python2.6和2.7共存，按以下步骤；如无此需求，则跳过。

注意：centos6默认存在`python2.6`，安装完`python2.7`之后会出现很多问题，以下安装过程实现两个版本并存。

①升级所有包，同时也升级软件和系统内核：

```
yum -y update
```

②安装开发工具集：

```
yum groupinstall -y 'development tools'
```

③安装python工具需要的软件包，不然安装`setuptools`和`pip`会出错：

```
yum install -y zlib-devel bzip2-devel openssl-devel xz-libs wget
```

④源码安装python2.7，下载安装脚本：

```
wget -P /root/python27/ http://172.190.92.118/package/htsec6/python27.sh
```

⑤然后执行脚本文件：

```
sudo sh ./root/python27/python27.sh
```

⑥查看版本：

```
python2.7
```

⑦解决`yum`不能支持python2.7使用的问题：`vi /usr/bin/yum`， 将第一行`#!/usr/bin/python`改为`#!/usr/bin/python2.6`

⑧centos6上`python2.6.6`，`python2.7.5`，`python3.6.8`三版本共存

![](/assets/python2.png)

