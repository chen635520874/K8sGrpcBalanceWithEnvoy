# This file is a template, and might need editing before it works on your project.
FROM git.huoys.com:9999/docker-image/golang:1.14-gcc-alpine AS builder

WORKDIR /usr/src/server

COPY . .


RUN GOPROXY=https://goproxy.cn,direct GO111MODULE=on GOPRIVATE=git.huoys.com go build

FROM alpine:3.5

# We'll likely need to add SSL root certificates
#RUN apk --no-cache add ca-certificates

WORKDIR /usr/local/bin

COPY --from=builder /usr/src/server/server server

CMD ["./server"]

