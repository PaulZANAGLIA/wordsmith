FROM golang:alpine as builder
COPY dispatcher.go .
RUN go build dispatcher.go

FROM alpine
COPY --from=builder /go/dispatcher .
COPY static static

# Run code
CMD ["./dispatcher"]

# Build it with : docker build -t "web-tp1" .