## 1.1 客户端配置

首先`cat/etc/issue`或者`cat/etc/centos-release`查看操作系统内核版本是CentOS7还是CentOS6

根据不同的操作系统，以下操作可能会有轻微不同

### CentOS7

1.将htsec7.repo放到/etc/yum.repos.d/目录下

`vim /etc/yum.repos.d/htsec7.repo`

```
[htsec7]
name = ht local repo for centos 7
baseurl = http://172.190.92.118/package/htsec7
enabled = 1
gpgcheck = 0
```

2.清除并重新生成cache文件，并查看htsec7仓库是否生效

```
yum clean all
yum makecache
yum repolist
```

![](/assets/image-20201027171601466.png)

### CentOS6

1.将htsec6.repo放到/etc/yum.repos.d/目录下

`vim /etc/yum.repos.d/htsec6.repo`

```
[htsec6]
name = ht local repo for centos 6
baseurl = http://172.190.92.118/package/htsec6
enabled = 1
gpgcheck = 0
```

2.清除并重新生成cache文件，并查看htsec6仓库是否生效

```
yum clean all
yum makecache
yum repolist
```

![](file://C:/Users/90607/Desktop/新建文件夹/upload/image-20201027171719920.png?lastModify=1605087087 "image-20201027171719920")

