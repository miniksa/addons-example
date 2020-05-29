ARG BUILD_FROM
FROM $BUILD_FROM

# Add env
ENV LANG C.UTF-8

# Setup base
RUN \
    apk add php7 --update-cache --repository http://dl-cdn.alpinelinux.org/alpine/edge/community/ --allow-untrusted

# Copy data
COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
