# syntax=docker/dockerfile:1
FROM golang:1.21-alpine AS build
WORKDIR /app
COPY . .
RUN go mod download
RUN go build -o read_products read_products.go
CMD ["./read_products"]
