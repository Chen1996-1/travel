# travel

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

## git 问题
每当使用
```
git branch [分支名]
```
的时候，需要pull 一下

在新建分支提交代码后，需要回到主分支 
```
git checkout main

git merge [新建分支名]

git push
```
合并一下