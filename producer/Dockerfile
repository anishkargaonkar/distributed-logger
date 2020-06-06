
FROM golang:1.14

WORKDIR /app

ADD go.mod .

RUN go mod tidy

ADD . .

RUN go build -o main ./producer/main.go

CMD ["./main"]