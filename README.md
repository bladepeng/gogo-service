[![wercker status](https://app.wercker.com/status/77d75a37d5549e4d81b4b21e550efccc/s/master "wercker status")](https://app.wercker.com/project/byKey/77d75a37d5549e4d81b4b21e550efccc)

# GoGo
A microservice for playing the game of Go

该代码是[Cloud Native Go](http://rootsongjc.github.io/cloud-native-go)书中的示例，主要用来演示使用[api blueprint](https://github.com/apiaryio/api-blueprint)来创建RESTful服务的API文档。

该项目中API文档`api.html`文件使用[aglio](https://github.com/danielgtaylor/aglio)工具生成，命令如下：

```
aglio -i apiary.apib -o api.html
```

原书中使用Apiary来生成API文档，可以在 http://docs.gogame.apiary.io/ 访问。