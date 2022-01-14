# SubQuery-Practice
> learning subquery

### 安装subquery
> node version >= 14

```shell
npm install -g @subql/cli
```

### 新建一个subquery项目
> 此处需要开代理
```shell
subql init myProject
```
### 安装项目依赖
> 注意将package.json中的polkadot.js的依赖改为^6
```shell
cd myProject
yarn install
yarn build
```
可以看到编译后产生了`dist`文件夹

```shell
docker-compose up
```
> 可以看到启动了三个容器

### 运行项目
>打开浏览器，localhost:3000,进行查询
```
{
  query{
    starterEntities(last:10, orderBy:FIELD1_ASC){
      nodes{
        field1
      }
    }
  }
}
```