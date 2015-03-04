FROM wellsie/centos7-phantomjs
MAINTAINER Jono Wells <_oj.io>

ENV CASPERJS_VERSION 1.1.0-beta3

RUN cd /usr/local && \
    git clone -b develop https://github.com/rdpanek/casperjs.git && \
    ln -s /usr/local/casperjs/bin/casperjs /usr/bin/casperjs

CMD [ "/usr/bin/casperjs" ]
