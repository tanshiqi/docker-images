FROM golang:1.21-alpine

RUN go install tailscale.com/cmd/derper@main
ENTRYPOINT ["/go/bin/derper"]
