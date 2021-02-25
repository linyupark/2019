---
theme: "Beige"
transition: "convex"
highlightTheme: "atom-one-dark"
# logoImg: "http://linyu.dynv6.net:9001/images/ppt/html5.png"
logoImg: "http://git.cairenhui.com/uploads/-/system/appearance/logo/1/logo.png"
slideNumber: false
title: "2019 前端分享"
---

## 前端年度分享

微服务 · Docker {style=font-size:36px;color:#999}

<br><br>

<a href="mailto://linyu0710@cairenhui.com">
  📩
  linyu0710@cairenhui.com
</a>

🍼 🚴 🏀 📷

---

## 回顾

Web 开发

---

巨石 (Monolith)

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/QQ20191216-112133@2x.png){style=width:80%;border-radius:15px}

---

前后端分离 (Frontend & Backend)

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/QQ20191216-122420@2x.png){style=width:80%;border-radius:15px}

---

后端微服务 (Microservice)

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/QQ20191216-123936@2x.png){style=width:80%;border-radius:15px}

---

## 回顾

前端开发

---

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/js-modules.png){style=width:90%;border-radius:15px}

---

### 🤔 Why 模块化?

<br>

🚫 浏览器不支持{.fragment}

🍣 代码拆分复用{.fragment}

🤝 管理依赖关系{.fragment}

🚥 按序加载资源{.fragment}

---

👽 高科技

⬇

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/module-bundlers.png){style=width:80%;border-radius:15px}

⬇

😀 接地气

---

### 🤔 又Why工程化打包？

<br>

🙏 文件合并减少请求数{.fragment}

💡 变更文件名缓存控制{.fragment}

📚 语法转译适配多平台{.fragment}

🍻 优化压缩个性化配置{.fragment}

---

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/QQ20191216-152455@2x.png){style=width:80%;border-radius:15px}

👬 [CRH Vue Components](http://linyupark.github.io/projects/storybook-crh-vue/)

---

### 🤔 叒Why UI组件化？

<br>

🚫 浏览器支持少且兼容性较差{.fragment}

🙅 远离`jQuery`命令式低效编程{.fragment}

💎 结合UI模块化更有效地复用{.fragment}

💪 解耦程度更高便于单元测试{.fragment}


---

<!-- .slide: data-background="http://linyu.dynv6.net:9001/images/ppt/mircofed/8c1001e93901213f59f4f4e259e736d12e2e95cd.gif" -->

<div style="background: #D2593E; color: #fff; width: 250px; height: 250px; border-radius: 50%; text-align: center; position: absolute; left: 18%; padding: 20px; opacity: .9; box-shadow: 0 0 10px #000;">
  <br>
  组织
  <br>
  <p><small>模块，组件</small></p>
</div>

<div style="background: #617A7F; color: #fff; width: 250px; height: 250px; border-radius: 50%; text-align: center; position: absolute; right: 18%; top: 190px; padding: 20px; opacity: .9; box-shadow: 0 0 10px #000;">
  <br>
  优化
  <br>
  <p><small>压缩，代码分割，动态加载</small></p>
</div> 

<div style="background: #A8AB66; color: #fff; width: 250px; height: 250px; border-radius: 50%; text-align: center; padding: 20px; position: absolute; left: 20%; top: 380px; opacity: .9; box-shadow: 0 0 10px #000;">
  <br>
  生产
  <br>
  <p><small>打包，共享库CDN，自动脚本CLI</small></p>
</div>

---

<!-- .slide: data-background="http://linyu.dynv6.net:9001/images/ppt/mircofed/9f510fb30f2442a7eaa460acdc43ad4bd1130214.gif" -->

<div style="background: #444; color: #fff; width: 250px; height: 250px; border-radius: 50%; text-align: center; position: absolute; left: 18%; padding: 20px; opacity: .9; box-shadow: 0 0 10px #000;">
  <br>
  🌲🌲🌲
  <br>
  成长
</div>

<div style="background: #444; color: #fff; width: 250px; height: 250px; border-radius: 50%; text-align: center; position: absolute; right: 18%; top: 190px; padding: 20px; opacity: .9; box-shadow: 0 0 10px #000;">
  <br>
  🍄🍄🍄
  <br>
  增多
  <br>
  🐵🐵🐵
</div> 

<div style="background: #444; color: #fff; width: 250px; height: 250px; border-radius: 50%; text-align: center; padding: 20px; position: absolute; left: 20%; top: 380px; opacity: .9; box-shadow: 0 0 10px #000;">
  <br>
  ✨✨
  <br>
  库✨框架
</div>

---

### 微前端

![](https://pic4.zhimg.com/v2-369aff8f4b18636dd33e2f26641d206c_1200x500.jpg)

😇 既然服务端有微服务，前端为什么不能有？？ {style=font-size:36px;color:#999}

---

## Micro 优势

<br>

🚤 船小好掉头技术重构不用愁{.fragment}

💴 不同业务选合适的技术架构避免浪费 (App Shell){.fragment}

💪 严格业务划分问题定位更快捷{.fragment}

🤞 独立部署自动化测试更新迭代不拖沓{.fragment}

---

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/verticals-headline.png){style=width:80%;border-radius:15px}

小型自治服务集群

---

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/QQ20191217-141407@2x.png){style=width:80%;border-radius:15px}

构建大型复杂应用 (App shell)

---

## 场景分析

<br>

单实例 ✔ | 多实例
------|-------
同页面单应用 | 同页面混合多应用 
具备完整应用生命周期 | 适合组件业务封装而非应用
{style=font-size:28px}

---

## 单例方案

<br>

现代 ✔ | 传统 (体验差通讯难)
------|-------
注册路由 混合 SPA | 整页跳转
[single-spa](https://single-spa.js.org/) · [qiankun](https://github.com/umijs/qiankun) ✔| IFrame + postMessage
{style=font-size:28px}

---

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/QQ20191219-165208-HD.gif)

技术栈无关 ✔ 独立开发部署 ✔ 独立运行时 ✔ {style=font-size:28px}

---

### 🌰 code

::: block
```javascript
import * as Vue from "vue";
import App from "./App.vue";
import "./main.css";

import {
  registerMicroApps,
  setDefaultMountApp,
  runAfterFirstMounted,
  start
} from "qiankun";

window.Emitter = new Vue();

new Vue({
  el: "#root",
  render: h => h(App)
});

function render({ appContent, loading }) {
  document.querySelector("#loading").style.display = loading
    ? "block"
    : "none";
}

/** 注册所有微应用 */
registerMicroApps(
  [
    {
      // Vue 应用
      name: "AppVue",
      entry: "http://localhost:8081",
      render,
      activeRule: () => {
        return ~location.hash.search("#/app-vue");
      }
    },
    {
      // React 应用
      name: "AppReact",
      entry: "http://localhost:8082",
      render,
      activeRule: () => {
        return ~location.hash.search("#/app-react");
      }
    }
  ],
  {
    beforeLoad: [
      app => {
        console.log("应用加载前", app);
      }
    ],
    beforeMount: [
      app => {
        console.log("应用挂载前", app);
        window.Emitter.$emit('app.mounted', app.name);
      }
    ],
    afterUnmount: [
      app => {
        console.log("应用卸载后", app);
        document.getElementById('container').innerHTML = '<h3>微前端+docker部署展示</h3>';
      }
    ]
  }
);

// setDefaultMountApp("/#/app-vue");
// runAfterFirstMounted(() => {
//   console.info("首个应用挂载完毕");
// });

start();
```
{style=font-size:24px}
:::
::: block
[阿里乾坤](https://github.com/umijs/qiankun) | 
[积分商城活动服务 app shell](http://git.cairenhui.com/openx/microfed-bootstrap)
{style=font-size:18px}
:::

---

## MFE开发部署挑战

<br>

* 操作系统不同

* node版本不同

* 全局包遗漏或版本不同

* 端口占用状况不同

---

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/docker_logo_media_social_170.66666666667px_1213006_easyicon.net.png){style=border:none;box-shadow:none}

### Docker 构建开发部署环境

---

### 简介

![](http://linyu.dynv6.net:9001/images/ppt/mircofed/095016afpafos1zcan1ic3.jpg)

---

### 实践

将现有项目转为基于 `Docker` 环境开发

---

## Dcokerfile

```dockerfile
# 必填 指定基础镜像 node版本在这里最好统一
FROM node:12.13-alpine

# 可跟 项目版本一致
LABEL version="1.0"

# 可选 维护人
LABEL maintainer="<linyupark@gmail.com>"

# 可选 说明
LABEL description="Docker Demo"

# 将项目文件导入工作目录
COPY . /data/

# 指定命令运行目录
WORKDIR /data

# 暴露项目会用到的端口
EXPOSE 3000

# 创建时安装依赖
RUN \
npm config set registry https://registry.npm.taobao.org && \
npm install

CMD ["npm", "start"]
```

---

## docker-compose

```yaml
version: '3'
services: 
  app-shell:
    # dockerfile 位置
    build: ./app-shell
    # 挂载卷
    volumes: 
      - ./app-shell/src:/data/src
    # 容器对应本地映射端口
    ports:
      - "8080:8080"
    # 自启动服务
    # restart: always
  app-vue:
    # dockerfile 位置
    build: ./app-vue
    # 挂载卷
    volumes: 
      - ./app-vue/src:/data/src
    # 容器对应本地映射端口
    ports:
      - "8081:8081"

    # 自启动服务
    # restart: always
  app-react:
    # dockerfile 位置
    build: ./app-react
    # 挂载卷
    volumes: 
      - ./app-react/src:/data/src
    # 容器对应本地映射端口
    ports:
      - "8082:8082"
    # 自启动服务
    # restart: always
```

---

## 演示&提问

THANKS