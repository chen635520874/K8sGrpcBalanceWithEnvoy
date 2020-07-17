FROM alpine
MAINTAINER chenliang

RUN mkdir -p /opt/hall/client
WORKDIR /opt/hall/client
RUN GOPROXY=https://goproxy.cn,direct GO111MODULE=on GOPRIVATE=git.huoys.com go build

CMD ["./client"]
