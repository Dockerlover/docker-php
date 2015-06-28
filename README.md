# docker-php
Docker化php

## 镜像特点

- 2015/6/28 继承基础镜像docker-ubuntu

## 使用方法

- 获取代码并构建

        git clone https://github.com/Dockerlover/docker-php.git
        cd docker-php
        docker build -t docker-php .

- 运行容器

        docker run -d -it --name php -p 8081:80 \
        -v /var/data/php:/app docker-php
