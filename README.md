# Mutil Selector Power by Vue

## 目标
练手项目：做一个基于`Vue2`的列表选择模块

## 技术栈
* Vue2
* ES6 + Babel 转义
* Webpack 打包
* Webpack-dev-server 调试

## 记录
### 起手遇坑，引入Vue后跑demo报错
* 情况
```
import Vue from 'vue'；
```
* 报错
```
[Vue warn]: Failed to mount component: template or render function not defined. (found in root instance)
```
* 原因
`Vue2`开始划分了**完整版**(`~/vue/dist/vue.js`)和**运行时版**(`~/vue/dist/vue.runtime.common.js`)，运行时版不包括Vue Template，而`import Vue from 'vue'；`引用的是运行时版，所以报错了。
* 解决方法
```
import Vue from 'vue/dist/vue.js'；
```

## 关注点
* vue 项目构建工具流
* vue 的模块化(template)
* 动起来
