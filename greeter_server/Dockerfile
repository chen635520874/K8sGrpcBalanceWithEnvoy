FROM alpine
MAINTAINER chenliang

RUN mkdir -p /opt/hall/server
WORKDIR /opt/hall/server
COPY ./log-metrics /opt/hall/server

CMD ["./server"]
