FROM alpine:3.9

LABEL maintainer "Sven <sven@ocular-d.tech>" \
    org.label-schema.vendor = "TestTheDocs" \
    name="ci-base" \
    description="Alpine base image for CI"

RUN adduser -s /bin/false -D -H ttd \
    && apk --no-cache add \
    tini \
    su-exec \
    bash \
    git \
    openssh \
    tar \
    gzip \
    ca-certificates
