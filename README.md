redis的安装配置
# tar -xzvf redis-stable.tar.gz -C /opt
1
注意：-C 指定解压到的位置，这里我解压到/opt下

编译redis
切换到解压到的目录下

# cd /opt/redis-stable
1
然后执行make命令

# pwd
/opt/redis-stable
pwd
/opt/redis-stable

# make install
1
2
3
4
运行redis
安装后，您可以通过执行redis-server命令，开启redis服务

# redis-server

# redis-server /opt/redis-stable/redis.conf
测试redis服务是否正常
不要关闭启动redis服务的窗口，重新开启一个命令行窗口，在新的窗口输入

# redis-cli
1
会看到进入>符号的模式

127.0.0.1:6379>
1
要检查redis服务是否正常工作，我们可以发送ping命令测试

127.0.0.1:6379>ping
1
如果服务器运作正常的话会输出

PONG
1
退出redis-cli程序

127.0.0.1:6379>quit
或
127.0.0.1:6379>exit
