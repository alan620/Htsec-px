数据中心提供的常用中间件版本基线：

| 软件名 | 版本基线 |
| :--- | :--- |
| Apache | 当前次新版本为2.4.46 |
| Nginx | 当前次新版本为1.18.0 |
| Redis | 最新稳定版为6.0.6 |
| Tomcat-7 | 当前次新版本为7.0.96 |
| Tomcat-8 | 当前次新版本为8.5.56 |
| Tomcat-9 | 当前次新版本为9.0.36 |

在数据中心提供的版本基础上，总结常用中间件，如下：

| 软件名 | 版本号（CentOS7） | 版本号（CentOS6） | 最新版 |
| :--- | :--- | :--- | :--- |
| Apache | 2.4 | 2.4 | 2.4.46 |
| GCC | 9 | 9 | 10 |
| G++ | 9 | 9 | 10 |
| Nginx | 1.18.0 | 1.18.0 | 1.19.3 |
| Redis | 6.0.6 | 6.0.6 | 6.0.8 |
| MongoDB | 4.2 | 4.2 | 4.4 |
| MySQL | 8.0.21 | 8.0.21 | 8.0.22 |
| JDK | 1.8.0 | 1.8.0 | 1.9.0 |
| Python2 | 2.7 | 2.6&2.7 | 2.7.18 |
| Python3 | 3.6.8 | 3.6.8 | 3.9.0 |
| Node.js | 10.22.1 | 10.22.1 | 12.19.0 |
| Npm | 6.14.6 | 6.14.6 | 6.14.8 |
| Anaconda-core | 21.48.22.158 | 不常用暂不提供 | 21.48.22.159 |
| Git | 2.22.4 | 2.22.4 | 2.29.2 |

部分安装命令：

| 软件名 | CentOS7 | CentOS6 |
| :--- | :--- | :--- |
| Apache | yum install -y httpd | yum install -y**httpd24\*** |
| GCC&G++ | yum install -y devtoolset-9\*\(需配置\) | yum install -y devtoolset-9\*\(需配置\) |
| Nginx | yum install -y nginx | yum install -y nginx |
| Redis | 编译安装 | 编译安装 |
| MongoDB | yum install -y mongodb-org | yum install -y mongodb-org |
| MySQL | 脚本安装 | 脚本安装 |
| JDK | yum install -y java | yum insall -y java |
| Python2 | yum install -y python | **python2.6和2.7共存需配置** |
| Python3 | yum install -y python3 | yum install -y **python36u\*** |
| Nodejs&Npm | yum install -y nodejs | yum install -y nodejs |
| Anaconda | yum install -y anaconda-core | 不常用暂不提供 |
| Git | yum install -y git222 | yum install -y git222 |

备注：除了提供以上常用中间件基线，海通镜像源也提供aix源、centos源、docker-ce源、epel源、pypi源、ubuntu源等。如需其他软件，可直接下载；如出现无法下载的情况，与我联系（WX：18916271961）。

