FROM pkeropen3/storm_debian:0.10.0
MAINTAINER pkeropen3<pkeropen3@163.com>

LABEL description="Docker Storm Nimbus image"

RUN /usr/bin/config-supervisord.sh nimbus 
RUN /usr/bin/config-supervisord.sh drpc

EXPOSE 6627
EXPOSE 3772
EXPOSE 3773
ADD start-supervisor.sh /usr/bin/start-supervisor.sh
CMD /usr/bin/start-supervisor.sh
