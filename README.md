# thingsboard_compose

Thingsboard 的 docker-compose 部署

> 参考文档：https://thingsboard.io/docs/user-guide/install/docker/

## 初始化

```bash
mkdir -p volumes/data && sudo chown -R 799:799 volumes/data
mkdir -p volumes/logs && sudo chown -R 799:799 volumes/logs
```

## 访问
- 地址：http://localhost:8080
- 账户：
    - System Administrator: sysadmin@thingsboard.org / sysadmin
    - Tenant Administrator: tenant@thingsboard.org / tenant
    - Customer User: customer@thingsboard.org / customer
