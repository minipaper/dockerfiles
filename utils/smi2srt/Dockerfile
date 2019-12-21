#
# Dockerfile for smi2srt
#

FROM alpine
MAINTAINER minipaper <pianoday@gmail.com>

RUN apk add --no-cache npm \
    && npm --version \
    && npm install -g smi2srt
    && smi2srt --version

WORKDIR /data

ENTRYPOINT ["smi2srt"]
CMD ["--help"]
