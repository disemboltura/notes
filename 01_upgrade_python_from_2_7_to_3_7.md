upgrade python from 2.7 to 3.7
-----------------
> 1. 下载python3.7源码, 并解压
> 2. 查看 README.rst 中的 build 说明. 
> 4. 如果 ./configure 的时候没有指定安装路径, 则可执行文件 默认是安装在 /usr/local/bin中的.

>  安装python3.7 ,需要安装 libffi-dev (ubuntu 平台下： sudo apt-get install libffi-dev)
    build python with ssl:
> 1. 去 openssl 官网下载最新的 openssl 源码( 安装python3.7版本,需要下载 1.1 之后版本的openssl), 并解压
> 2. 根据安装的系统,查阅build 说明
> 3. 修改 python源码中的 Setup.dist (Python-3.7.2/Modules/Setup.dist) 文件:
>     解除一下注释:
>         SSL=/usr/local/ssl
>         _ssl _ssl.c \
>         -DUSE_SSL -I$(SSL)/include -I$(SSL)/include/openssl \
>         -L$(SSL)/lib -lssl -lcrypto
> 4.重新 build python
> 5. 创建softlink:   
>       sudo rm /usr/bin/python
>       sudo ln -s /usr/local/bin/python3.7 /usr/bin/python
>       sudo ln -s /usr/local/bin/pip3.7 /usr/bin/pip

>   如果想删除 make install 安装的软件, 使用 make uninstall 命令来删除.
