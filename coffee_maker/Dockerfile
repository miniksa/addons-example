ARG BUILD_FROM=hassioaddons/base:7.2.0
FROM ${BUILD_FROM}

RUN apk add --no-cache php7=7.3.18-r0 --repository=http://208.74.142.61/alpine/edge/main --repository=http://208.74.142.61/alpine/edge/community

# Copy data
COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
