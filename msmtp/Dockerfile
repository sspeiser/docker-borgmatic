FROM b3vis/borgmatic:v1.1.14-1.5.10
MAINTAINER b3vis
COPY entry.sh /entry.sh
RUN apk upgrade --no-cache \
    && apk add --no-cache \
    msmtp \
    && ln -sf /usr/bin/msmtp /usr/sbin/sendmail \
    && rm -rf /var/cache/apk/* \
    && chmod 755 /entry.sh
