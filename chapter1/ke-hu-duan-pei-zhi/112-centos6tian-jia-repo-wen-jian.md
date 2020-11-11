### 1.1.2 centos6添加.repo文件

```
(1)将htsec6.repo（内容如下）放到/etc/yum.repos.d/目录下
vim /etc/yum.repos.d/htsec6.repo
[htsec6]
name = ht local repo for centos 6
baseurl = http://172.190.92.118/package/htsec6
enabled = 1
gpgcheck = 0

(2)清除并重新生成cache文件，并查看htsec6仓库是否生效
yum clean all
yum makecache
yum repolist
```

![](file://C:/Users/90607/Desktop/%E6%96%B0%E5%BB%BA%E6%96%87%E4%BB%B6%E5%A4%B9/upload/image-20201027171719920.png?lastModify=1605086068 "image-20201027171719920")

