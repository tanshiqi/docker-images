FROM golang:latest

ARG DERP_VERSION=latest
RUN go install tailscale.com/cmd/derper@${DERP_VERSION}
ENTRYPOINT ["/go/bin/derper"]
