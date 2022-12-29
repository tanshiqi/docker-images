FROM golang:alpine
RUN go install tailscale.com/cmd/derper@main
CMD /go/bin/derper --hostname $DERP_DOMAIN -http-port -1 --stun
