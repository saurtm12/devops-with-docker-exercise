FROM golang:1.16-alpine

RUN apk update && apk add git

WORKDIR /app
RUN git clone https://github.com/docker-hy/material-applications.git

WORKDIR /app/material-applications/example-backend

RUN go mod download
RUN go build .


CMD ["./server"]


