FROM registry.cn-shenzhen.aliyuncs.com/imhuso/bt:1.0

MAINTAINER imhuso <imhuso@126.com>

WORKDIR /www/server/panel/install

RUN bash /www/server/panel/install/install_soft.sh 1 install nginx 1.12.2 \
	&& bash /www/server/panel/install/install_soft.sh 1 install mysql 5.6.37 \
	&& bash /www/server/panel/install/install_soft.sh 1 install php 7.2.3

CMD ["/start.sh"]