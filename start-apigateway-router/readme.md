<!--
 * @Descripttion: 
 * @Author: Wang Dejiang(aei)
 * @Date: 2022-07-30 21:57:43
 * @LastEditors: Wang Dejiang(aei)
 * @LastEditTime: 2022-08-14 22:29:13
-->
<h1 align="center">api-gateway 组件快速应用</h1>
<p align="center" class="flex justify-center">
  <a href="https://nodejs.org/en/" class="ml-1">
    <img src="https://img.shields.io/badge/node-%3E%3D%2010.8.0-brightgreen" alt="node.js version">
  </a>
  <a href="https://github.com/devsapp/start-sae/blob/master/LICENSE" class="ml-1">
    <img src="https://img.shields.io/badge/License-MIT-green" alt="license">
  </a>
  <a href="https://github.com/devsapp/start-sae/issues" class="ml-1">
    <img src="https://img.shields.io/github/issues/devsapp/start-sae" alt="issues">
  </a>
  </a>
</p>

# 使用api-gateway组件快速部署应用
## 本地快速体验
通过该应用，您可以简单快速的使用api-gateway组件部署使用api网关的Docusaurus项目和KOA项目应用。

- 下载命令行工具：`npm install -g @serverless-devs/s`
- 初始化一个模版项目：`s init start-gateway-router`
- 执行`s deploy`命令，输入对应字段，自动将api网关，Docusaurus应用，KOA应用部署到相应的API网关服务和函数计算服务中。
 
  <!-- 放置组件部署截图 -->
- 部署成功后使用api网关组件返回的自定义域名访问两个应用：路由`/web/*`对应Docusaurus网站路由；路由`/koa/*`对应koa应用的`/*`路由

  <!-- 放置部署成功后终端截图和网站截图 -->


注意事项:
  
  初始化时不输入自定义域名选项，则api网关组自动生成的公网域名访问时会由于请求头格式原因直接将响应作为文件下载。如果需要访问页面，则需要绑定好提前备案且经过解析的域名。域名备案解析过程详情可见：[分组的域名绑定](https://help.aliyun.com/document_detail/159014.html)。


-----

> - Serverless Devs 项目：https://www.github.com/serverless-devs/serverless-devs   
> - Serverless Devs 文档：https://www.github.com/serverless-devs/docs   
> - Serverless Devs 钉钉交流群：33947367    