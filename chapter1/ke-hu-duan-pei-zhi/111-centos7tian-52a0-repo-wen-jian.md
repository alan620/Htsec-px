### 1.1.1 centos7添加.repo文件

```
(1)将htsec7.repo（内容如下）放到/etc/yum.repos.d/目录下
vim /etc/yum.repos.d/htsec7.repo
[htsec7]
name = ht local repo for centos 7                #仓库描述
baseurl = http://172.190.92.118/package/htsec7        #仓库路径
enabled = 1                            #启用为1，否则为0
gpgcheck = 0                            #包安全性检查，建议设置为0

(2)清除并重新生成cache文件，并查看htsec7仓库是否生效
yum clean all
yum makecache
yum repolist
```

![](file://C:/Users/90607/Desktop/%E6%96%B0%E5%BB%BA%E6%96%87%E4%BB%B6%E5%A4%B9/upload/image-20201027171601466.png?lastModify=1605085995 "image-20201027171601466")

