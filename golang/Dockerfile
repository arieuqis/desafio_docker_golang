FROM golang:1.10-alpine3.8 AS builder

WORKDIR /go

COPY . /go/src

RUN go build -ldflags "-w" ./src/hello.go

FROM hello-world:latest
WORKDIR /go
COPY --from=builder /go /go
ENTRYPOINT [ "./hello" ]
