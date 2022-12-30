FROM golang:1.19-alpine

RUN go install tailscale.com/cmd/derper@main
ENTRYPOINT ["/go/bin/derper"]
