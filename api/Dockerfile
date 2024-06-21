FROM golang:alpine as builder

RUN mkdir /build

ADD . /build/

WORKDIR /build

RUN go build -o main .

FROM alpine

RUN adduser -S -D -H -h /app appuser

USER appuser

COPY . /app

COPY --from=builder /build/main /app/

WORKDIR /app

EXPOSE 3000

CMD ["./main"] 
#  The Dockerfile is a multi-stage build. The first stage is the builder stage where the Go application is built. The second stage is the final stage where the Go application is copied from the builder stage to the final stage. 
#  The  docker-compose.yml  file is used to define the services that make up the application. 
#  version: '3.7'