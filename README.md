# thingsboard_compose

Thingsboard 的 docker-compose 部署

> 参考文档：https://thingsboard.io/docs/user-guide/install/docker/

## 启动

```bash
# 首次启动
docker compose run --rm -e INSTALL_TB=true -e LOAD_DEMO=true thingsboard-ce
# 常规启动
docker compose up -d
```

## 端口

- 8080: HTTP
- 8443: HTTPS
- 1883: MQTT
- 8883: MQTT over TLS
- 5683-5688: UDP
- 7070: Edge RPC

## 访问
- 地址：http://localhost:8080
- 账户：
    - System Administrator: sysadmin@thingsboard.org / sysadmin
    - Tenant Administrator: tenant@thingsboard.org / tenant
    - Customer User: customer@thingsboard.org / customer
