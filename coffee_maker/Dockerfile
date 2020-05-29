ARG BUILD_FROM
FROM $BUILD_FROM

# Add env
ENV LANG C.UTF-8

# Setup base
RUN apk add --no-cache \
        curl \
        evtest \
        php7 \
        php7-curl \
        php7-openssl \
        php7-pdo \
        php7-pdo_sqlite \
        php7-sqlite3 \
        php7-sockets \
        screen \
        sudo

# Copy data
COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
