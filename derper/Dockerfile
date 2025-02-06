FROM golang:1.21-alpine

RUN go install tailscale.com/cmd/derper@${DERP_VERSION}
ENTRYPOINT ["/go/bin/derper"]
