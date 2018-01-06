#VERSION 0.0.2
#symfony3 基于apache2 php7实现 开发环境
FROM xcyxiner/symfony
#签名
MAINTAINER xcyxiner "xcyxiner@me.com"
RUN apt-get update
#git 
RUN apt-get install -y git
#vim中文乱码
ADD .vimrc  /root/.vimrc
#默认目录
WORKDIR /var/www/html
#bash 无法输入中文
ENV LANG C.UTF-8
#安装 tree
RUN apt-get install -y tree
#时区
ADD usr_share_zoneinfo_Asia_Shanghai /etc/localtime
