FROM pkeropen3/storm_debian:0.10.0
MAINTAINER pkeropen3<pkeropen3@163.com>

LABEL description="Docker Storm Supervisor image"

EXPOSE 6700
EXPOSE 6701
EXPOSE 6702
EXPOSE 6703
EXPOSE 8000

RUN /usr/bin/config-supervisord.sh supervisor
RUN /usr/bin/config-supervisord.sh logviewer
CMD /usr/bin/start-supervisor.sh




