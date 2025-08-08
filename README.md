# thingsboard_compose

Thingsboard 的 docker-compose 部署

> 参考文档：https://thingsboard.io/docs/user-guide/install/docker/

## 初始化

```bash
# 创建目录
mkdir -p volumes/data && sudo chown -R 799:799 volumes/data
mkdir -p volumes/logs && sudo chown -R 799:799 volumes/logs

# 首次启动
docker compose run --rm -e INSTALL_TB=true -e LOAD_DEMO=true thingsboard-ce
```

## 启动

```bash
sudo docker compose up -d
```

## 端口

- 8080: Web管理入口
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
