# dm.vector

on dmdock02
```
docker build -t 127.0.0.1:5000/vector .
docker push 127.0.0.1:5000/vector
docker service create --name vector --label traefik.port=80 --label traefik.domain=sysadmin.dm.marine.ie --network traefik-net 127.0.0.1:5000/vector
```

