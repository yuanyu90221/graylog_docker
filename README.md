# graylog_docker

This repository is for docker setup for graylog

## Notice

```yaml
deploy:
  resources:
    limits:
      memory: 1g
```

is for docker-swarm feature

must use option **--compatibility** to use it:

```shell
docker-compose --compatibility up -d
```

```shell
docker-compose --compatibility down -d
```

## 在graylog 加入 gelf input 讓 docker 可以直接透過這個 input 蒐集資料

https://www.jianshu.com/p/25e310596559

## 需要再研究一下 winston 集中送 log 到graylog 的方式
