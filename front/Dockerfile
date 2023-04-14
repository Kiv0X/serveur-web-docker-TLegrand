FROM golang:alpine

WORKDIR /app

COPY . .
RUN go mod download

EXPOSE 8000

RUN go build -o app dispatcher.go

CMD ["/app"]