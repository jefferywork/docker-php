# docker-php
Docker PHP 镜像

## Docker镜像地址

- https://hub.docker.com/r/jefferyjob/php

## 镜像构建与发布
```php
# 编译
docker build -t php:8.2.0 .

# 测试扩展是否安装
docker run -itd --name php-test php:8.2.0

# 重命名
docker tag php:8.2.0 jefferyjob/php:8.2.0

# 登陆docker
docker login -u jefferyjob

# 发布docker镜像
docker push jefferyjob/php:8.2.0
```

## 分支版本更新说明

### 8.2.0
- 基于 php:8.2-fpm-alpine 镜像初始化构建，安装常用的扩展