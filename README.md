# lerna-in-action

https://github.com/xgqfrms/lerna-in-action


```sh
$ npm i -g lerna

```

```sh
# 创建一个新的 git 代码仓库
# $ git init lerna-repo && cd lerna-repo

$ cd lerna-repo
# 将上述仓库转变为一个 Lerna 仓库：
$ lerna init

```

## packages

```sh
# $ mkdir lerna-test && cd lerna-test
$ mkdir lerna-test && cd $_

$ mkdir x-utils x-cli x-templates

# 初始化包
$ cd x-utils
$ npm init -y 

$ cd x-cli
$ npm init -y

$ cd x-templates
$ npm init -y

```


## refs

https://juejin.cn/post/6844903856153821198

