FROM alpine:3.3

RUN apk --no-cache update && \
    apk --no-cache add rsync python py-pip py-setuptools ca-certificates groff less && \
    pip --no-cache-dir install awscli && \
    rm -rf /var/cache/apk/*