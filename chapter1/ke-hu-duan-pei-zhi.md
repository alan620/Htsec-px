## 1.1 客户端配置

首先`cat/etc/issue`或者`cat/etc/centos-release`查看操作系统内核版本是CentOS7还是CentOS6

根据不同的操作系统，以下操作可能会有轻微不同

### CentOS7

1.将`htsec7.repo`放到`/etc/yum.repos.d/`目录下

`vim /etc/yum.repos.d/htsec7.repo`

\[htsec7\]

name = ht local repo for centos 7					\#仓库描述

baseurl = http://172.190.92.118/package/htsec7		\#仓库路径

enabled = 1											\#启用为1，否则为0

gpgcheck = 0										\#包安全性检查，建议设置为0



\(2\)清除并重新生成cache文件，并查看htsec7仓库是否生效

yum clean all

yum makecache

yum repolist







![](file://C:/Users/90607/Desktop/新建文件夹/upload/image-20201027171601466.png?lastModify=1605085995)

  


