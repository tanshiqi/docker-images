### 部署

```
docker run -itd --name derper \
-p 8001:8001 \
-p 3478:3478/udp \
-a :8001 \
ghcr.io/tanshiqi/derper:latest
```
