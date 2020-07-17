FROM alpine
MAINTAINER chenliang

RUN mkdir -p /opt/hall/client
WORKDIR /opt/hall/client
COPY ./log-metrics /opt/hall/client

CMD ["./client"]
