[![wercker status](https://app.wercker.com/status/77d75a37d5549e4d81b4b21e550efccc/s/master "wercker status")](https://app.wercker.com/project/byKey/77d75a37d5549e4d81b4b21e550efccc)

# GoGo
该代码是[Cloud Native Go](http://rootsongjc.github.io/cloud-native-go)书中的示例，主要用来演示使用[api blueprint](https://github.com/apiaryio/api-blueprint)来创建RESTful服务的API文档。

该项目中API文档`api.html`文件使用[aglio](https://github.com/danielgtaylor/aglio)工具生成，命令如下：

```
aglio -i apiary.apib -o api.html
```

原书中使用Apiary来生成API文档，可以在 http://docs.gogame.apiary.io/ 访问。

## 说明

该项目使用[wercker](http://www.wercker.com)构建，构建完成后自动push到docker hub，镜像名称为`jimmysong/gogo-service:latest`。

## 如何使用

直接使用docker启动

```
docker run -d --name gogo -p 8088:3000 jimmysong/gogo-service:latest
```

容器内部程序启动的端口号是3000，映射宿主机端口8088。

现在可以使用curl或者其他工具如postman向`http://localhost:8088`发送请求了。

API文档见[api.hmtl](api.html)。

