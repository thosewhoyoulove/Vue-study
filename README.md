# Vue-study

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve /pnpm serve
```

### Compiles and minifies for production
```
npm run build /pnpm build
```

### Lints and fixes files
```
npm run lint /pnpm lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## ref属性
 - 被用来给元素或者子组件注册引用信息(id的替代者)
 - 应用在HTML标签上获取的是真是DOM元素，应用在组件标签上是组件实例对象(vc)
  
## **总结TodoList案例**
1. ### 组件化编码流程：
    - 拆分静态组件：组件要按功能点拆分，命名不要与HTML元素冲突。
    - 实现动态组件：考虑好数据的存放位置，数据是一个组件在用，还是一些组件在用：
    <br>  - 一个组件在用：放在组件自身就可以了。
    <br>  - 一些组件在用，放在它们共同的父组件上(状态提升)。
    - 实现交互：从绑定事件开始。
2. props适用于：
   - 父组件 ===》 子组件 通信
   - 子组件 ===》 父组件 通信(要求父先给子一个函数)
3. 使用v-model时要切记：v-model绑定的值不能是props传过来的值，因为props是不能被修改的！
4. props传过来的值若是对象类型的值，修改对象中的属性时Vue不会报错，但不推荐这样做。



## **如何删除node—modules**
+ 全局安装rimraf,这是一个删除文件的**node**命令行工具
```
 pnpm install rimraf -g
```
+ 然后执行下列命令删除**node_modules**文件夹
```
 rimraf node_modules
```
    
