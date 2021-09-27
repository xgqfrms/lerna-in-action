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

## lerna script

> lerna create

```sh
# lerna create < name > [loc]
# 创建一个包，name 包名，loc 位置可选(默认放在 workspaces[0]所指位置)

# create
$ lerna create x-test packages
# OR (packages/@xgqfrms 不好使 ?)
$ lerna create x-test packages/@xgqfrms

```

> lerna add

```sh
# lerna add [@version] [--dev] [--exact]
# 增加本地或者远程 package 做为当前项目 packages 里面的依赖

# Adds the module-1 package to the packages in the 'prefix-' prefixed folders
lerna add module-1 packages/prefix-*

# Install module-1 to module-2
lerna add module-1 --scope=module-2

# Install module-1 to module-2 in devDependencies
lerna add module-1 --scope=module-2 --dev

# Install module-1 in all modules except module-1
lerna add module-1

# Install babel-core in all modules
lerna add babel-core


```

```sh
$ 

$ lerna list


```



## refs

https://juejin.cn/post/6844903856153821198

