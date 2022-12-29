### 部署

```
docker run -itd --name derper -e DERP_DOMAIN=www.example.com -p 443:443 -p 3478:3478/udp ghcr.io/tanshiqi/derper:latest
```
