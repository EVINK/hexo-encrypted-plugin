为你的文章加一把锁

## 简单易用

1. 在你的博客根目录下, 执行以下方法

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

3. 完成

你可以[点击这里](https://code.evink.cn/2023/03/post/an-article-with-password/)来查看具体效果(密码：1234)

等等… 如果你想要自定义解锁样式和逻辑的话
  * 在页面 `/blog_root/_posts/@encrypted/index.html` 里，替换掉你不喜欢的内容
  * 或指定一个存在的页面，用于处理渲染流程，像这样：
    ```ejs
    ---
    ...
    password: 123456
    encryptedModel: my-unlocking-page/
    ---
    ```

