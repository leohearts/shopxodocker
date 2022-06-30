# 用docker-compose 部署shopxo

## 部署步骤

- git clone git@github.com:leohearts/shopxodocker.git
- git submodule update --recursive
- 安装 docker-compose
- docker-compose up -d
- 访问 http://127.0.0.1:10000/ 继续安装，可修改 docker-compose.yml 来指定 mysql 密码，默认为: 
 - 地址 shopxomysqldb
 - 数据库名 db
 - 用户名 root
 - 密码 pass
