# swagger2axios

利用 swagger 配置自动生成访问后台 WebApi 代码(ts)

## 1、首先打开终端输入以下命令安装 swagger 包

```shell
yarn add nswag --dev
```

## 2、package.json 中添加代码

```javascript
  "scripts": {
    "generate-client": "node_modules/.bin/nswag swagger2tsclient /input:%npm_package_devConfig_genClient_input% /output:%npm_package_devConfig_genClient_output%"
  },
  "devConfig": {
    "genClient": {
      "input": "http://192.168.1.2:8080/api/v2/api-docs",
      "output": "src/client.ts"
    }
  },
```

## 3、运行

```shell
yarn run generate-client
```

# 利用 swagger 配置自动生成访问后台 WebApi 代码(js)

[另一个版本](https://github.com/nnhjgg/GenerateRequestFiles)
