FROM centos:7.4.1708

MAINTAINER imhuso <imhuso@126.com>

USER root

COPY ./start.sh /start.sh

RUN yum install -y wget \
    && wget -O install.sh http://download.bt.cn/install/install.sh \
    && sed -i 's/read -p "Do you want to install Bt-Panel to the $setup_path directory now?(y\/n): " go;/go="y"/g' install.sh \
    && sed -i 's/password=`cat \/dev\/urandom | head -n 16 | md5sum | head -c 8`/password="xiaoming@515"/g' install.sh \
    && sh install.sh \
    && chmod +x /start.sh

EXPOSE 80 88 443 3306 6378 8888

CMD ["/start.sh"]