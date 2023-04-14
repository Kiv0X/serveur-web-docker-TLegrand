FROM golang:alpine
LABEL key="vale"
WORKDIR /app

COPY . .
RUN go mod download


EXPOSE 8080

RUN go build -o app dispatcher.go

CMD ["/app/app"]