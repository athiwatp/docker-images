FROM wellsie/centos7-nginx
MAINTAINER Jono Wells <_oj.io>

RUN yum -y install \
  nginx \
  nodejs \
  npm \
  supervisor \
  && yum -y clean all

ADD supervisord.conf /etc/supervisord.conf
ADD supervisord.d/* /etc/supervisord.d/

CMD [ "/usr/bin/supervisord", "-n", "-c", "/etc/supervisord.conf" ]
