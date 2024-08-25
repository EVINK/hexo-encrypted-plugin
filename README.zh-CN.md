为你的文章加一把锁

## 简单易用

1. 在你的博客根目录下, 执行以下命令

```sh
$ npm i hexo-encrypted-plugin
```

2. 在需要加密的文章里，设置一个密码

```ejs
---
title: Chrome插件迁移至Manifest V3
urlname: chrome-extension-move-to-manifest-v3
tag: chrome-extension
date: 2022-06-15
password: 123456
---

```


你可以[点击这里](https://code.evink.cn/2023/03/post/an-article-with-password/)来查看具体效果(密码：1234)

## 注意

* 请不要使用此插件的 0.0.7 - 0.0.9 版本

* 若使用新版本报错，请尝试移除 public/ 文件夹 和 db.json，然后重新生成文章

```sh
$ rm -rf public/
$ rm db.json
$ hexo g
```
