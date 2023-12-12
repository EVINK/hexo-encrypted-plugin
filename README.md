English | [中文](https://github.com/EVINK/hexo-encrypted-plugin/blob/main/README.zh-CN.md)

Add a lock for your Hexo article.

## Easy to use

1. In your blog root directory, execute command beblow:

```sh
$ npm i hexo-encrypted-plugin
```

2. Set password in the article which you want it to get locked

```ejs
---
title: Transfer to Chrome Manifest V3
urlname: chrome-extension-move-to-manifest-v3
tag: chrome-extension
date: 2022-06-15
password: 123456
---

```


[Click here](https://code.evink.cn/2023/03/post/an-article-with-password/) to see the presentation(password: 1234)

## Warning

* Do NOT use version of 0.0.7 - 0.0.9

* If you found this plugin was broken after updated to the lateset version

  please try to remove folder "public/" and "db.json", then regenerate them

```sh
$ rm -rf public/
$ rm db.json
$ hexo g
```