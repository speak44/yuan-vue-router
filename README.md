# yuan-vue-router
手撸一个vue-router！
实现router的思路
首先要实现router，我们必须清楚我们这次到底要做什么东西，先把他们列出来:

实现并导出一个Router实例，供外部调用
实现一个公共组件RouterView，用来加载路由视图
实现一个RouterLink，用来跳转路由
整理一下每个组件的需求

Router实例，需要接收router传入的options，将所有路由以及嵌套路由处理和收集起来，并监听url的变化。并且他作为插件存在，应该有一个install方法
RouterView组件，根据自己的路由嵌套层级，找出对应的路由里面的组件，并展示出来
RouterLink组件，创建一个a标签，插入写入的文本，并根据props中to的值进行跳转
## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
