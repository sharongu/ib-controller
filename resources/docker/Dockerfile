FROM ib-gateway:template
#MAINTAINER clifton <cliftonk@gmail.com>

# install init scripts and binaries
ADD gateway.tar /ib-gateway
ADD bin/run-gateway /usr/bin/run-gateway

RUN chmod 777 /usr/bin/run-gateway \
 && chmod -R 777 /ib-gateway

# 4003 for the gateway API via socat
EXPOSE 4003

#VOLUME /ib-gateway

CMD ["/usr/bin/run-gateway"]
