FROM golang:1.19
RUN go install tailscale.com/cmd/derper@main
CMD /go/bin/derper --hostname $DERP_DOMAIN -http-port -1 --stun
