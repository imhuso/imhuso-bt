FROM imhuso/bt:1.0

MAINTAINER imhuso <imhuso@126.com>

WORKDIR /www/server/panel/install

RUN chmod +x *.sh \
	&& bash install_soft.sh 1 install nginx 1.12.2 \
	&& bash install_soft.sh 1 install mysql 5.6.37 \
	&& bash install_soft.sh 1 install php 7.2.3 \
	&& bash install_soft.sh 1 install phpmyadmin 4.7

CMD ["/start.sh"]