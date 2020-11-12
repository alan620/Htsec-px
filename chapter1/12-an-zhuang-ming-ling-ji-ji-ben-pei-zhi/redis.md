### Redis

#### CentOS7

使用脚本进行编译安装：

```
wget -P /root/ http://172.190.92.118/package/htsec7/redis.sh
```

执行脚本：

```
sh /root/redis.sh
```

启动redis：

```
/root/redis-6.0.6/src/redis-server
```

#### ![](/assets/redis1.png)

使用内置的客户端与Redis进行交互：

```
/root/redis-6.0.6/src/redis-cli
```

#### ![](/assets/redis2.png)

#### CentOS6

同上

