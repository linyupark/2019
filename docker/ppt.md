---
theme: "Beige"
transition: "convex"
highlightTheme: "atom-one-dark"
# logoImg: "http://linyu.dynv6.net:9001/images/ppt/html5.png"
logoImg: "http://git.cairenhui.com/uploads/-/system/appearance/logo/1/logo.png"
slideNumber: false
title: "前端 Docker"
---

## Docker 前端组分享

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/docker_logo_media_social_170.66666666667px_1213006_easyicon.net.png){style=border:none;box-shadow:none}

---

## 为什么要用？

<br>

🙏 运行环境一致{.fragment}

💡 更快、更小、更多(对比虚拟机){.fragment}

📚 更好的隔离性(端口暴露占用网络环境等){.fragment}

🍻 更简单的分布{.fragment}

💪 定制镜像简单{.fragment}

---

## 对比虚拟机

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/dockervsvm.jpg)

* Docker 应用抽象层
* 硬件抽象层

---

## 对前端的意义

<br>

::: block
* 可指定前端组统一化配置(工程、编辑器配置等等){.fragment}

* 不同接口环境制作不同镜像方便开发、测试、部署{.fragment}

* git之外又一层可回滚的备份机制(持续交付部署){.fragment}
:::
{style=font-size:38px}

---

## Docker 基本概念

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/095016afpafos1zcan1ic3.jpg)

* 镜像（Image)
* 容器 (Container)
* 仓库 (Repository)

---

## 镜像 

特殊的文件系统

* 提供运行时所需程序、库、资源、配置

* 可在原有镜像基础上继承覆盖

---

## 容器

new 一个镜像

* 容器是镜像运行的实例，可以控制状态

* 存储层非持久（因此需要Volume）

---

## 仓库

存放镜像的地方

* 仓库名:标签 管理不同镜像
* 官方 hub.docker.com
* 国内 基于官方镜像加速 + 私有库

---

## Dockerfile 

快速撸一个自定义镜像

---

## 1.FROM

继承自某镜像

```yaml
# 基于最新的node环境镜像
FROM node:lastest
```

---

## 2.RUN

执行一些命令完善镜像环境

```yaml
# 安装全局包
RUN npm i -g typescript
```

---

## 3.COPY / ADD

给镜像里加文件
{style=font-size:32px}

ADD更强大一些如可以外链跟自动解压缩
{style=font-size:32px}

```yaml
# 将当前目录的src文件放入镜像 /data 目录中
COPY ./src /data
```

---

## 4.ENV

设置镜像环境变量 (shell export)

```yaml
# 设置默认工作目录
ENV WORKHOME /data

# COPY就可以引入代替写死路径方便继承配置
COPY ./src ${WORKHOME}
```

---

## 5.WORKDIR

默认进入的目录影响 RUN的位置

---

## 6.ENTRYPOINT / CMD

功能都是容器启动后执行的最终命令
{style=font-size:32px}

CMD 只看最后一行
```yaml
CMD echo hello
CMD echo world
# 等同 echo world
```

两者都存在时 CMD会被视为入参

```yaml
ENTRYPOINT ["echo","hello","i am"]
CMD ["docker"]
# 等同 echo hello i am docker
```

区别CMD可被docker命令行加入的入参覆盖

```yaml
# 启动后进入 bash 交互
CMD /bin/bash
```

```bash
docker run -ti image /bin/sh
# 会覆盖 用 sh 代替 bash
```

---

## 7.EXPOSE

镜像服务中会用到的端口
{style=font-size:32px}

作用更多是用来告知使用人

---

## 8.不常用

* USER 镜像用什么用户去执行
* VOLUME 镜像与宿主目录挂载卷映射

---

## BUILD 创建镜像

执行 Dockerfile 创建镜像

1. 命令行
```bash
# docker build -t 镜像名称:镜像标签(版本号) Dockerfile所在位置
docker build -t test/service-vue:v1.0.0 .
```

2. VScode Docker插件右键文件执行build （镜像名默认为目录名:latest）

---

## 查看镜像

命令行

```bash
docker images|grep provider或者docker image list|grep provider
```

推荐vscode docker插件

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/QQ20191230-152023@2x.png)

---

## 镜像跑容器实例

命令行 

```bash
docker run -d --name=服务名 -p 宿主端口:容器端口 -v 宿主存储卷:容器存储卷 镜像ID
```
容器的操作都推荐在vscode上执行

---

## 更优雅的方式

docker-compose

```yaml
version '3'
services:
  web:
    image: crh/web-app:1.0.0
    build:
      context: .
      dockerfile: Dockerfile-dev
    ports:
      - "8080:9000"
    volumes: 
      - "./app-dev:${WORKHOME}"
```

---

## 演示讨论