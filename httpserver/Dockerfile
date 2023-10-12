FROM golang:1.20 AS builder
WORKDIR /app
COPY . .
ENV CGO_ENABLED=0
RUN go mod download \
&& go build -o main .

FROM ubuntu
COPY --from=builder /app/main /main
CMD ["/main"]
