FROM golang:1.10-alpine3.8 AS builder

WORKDIR /go

COPY . /go/src

ENTRYPOINT [ "go", "run", "src/hello.go" ]

# FROM alpine:3.8
# WORKDIR /go
# COPY --from=builder /go /go
# ENTRYPOINT [ "go", "run", "src/hello.go" ]
# CMD [ "ls" ]
