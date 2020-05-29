ARG BUILD_FROM=hassioaddons/base:7.2.0
FROM ${BUILD_FROM}

RUN apk add --no-cache php7

# Copy data
COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
