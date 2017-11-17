# Idea Vim Configuration

本仓库为[ideavim](https://github.com/JetBrains/ideavim)的个人配置，尽最大可能兼容Chrome Surfingkeys插件的行为习惯。

## 使用

#### 手工添加

建立一个硬链接，直接让IDEA读取其配置。

```shell
ln VimProjects/ideavimrc/local.vimrc ~/.ideavimrc
```

#### ideavimrc自动添加

```shell
./build-ideavimrc.sh
```
#### spacevim自动添加

配置基本的spacevim属性。

```sh
./build-spacevim.sh
```

#### idea properties自动添加

该策略主要是防止idea升级时覆盖自定义的配置路径，或者是多主机使用时，配置同步盘达到多机配置同步的功能。

```sh
./build-idea-proerties.sh
```

## 键位设置

在不与Surfingkeys的大部分默认键位冲突下，有如下规则：

1. 尽量选用与原快捷键的意义相近的关键字键位
2. 在关键字无法避让的情况下采用**就近原则**或**大写策略**

如果键位不幸与默认键位冲突，优先满足默认键位，将冲突键位放置于特殊字符处，如`;`。

