FROM alpine
MAINTAINER chenliang

RUN mkdir -p /opt/hall/server
WORKDIR /opt/hall/server
RUN GOPROXY=https://goproxy.cn,direct GO111MODULE=on GOPRIVATE=git.huoys.com go build

#COPY ./server /opt/hall/server

CMD ["./server"]
