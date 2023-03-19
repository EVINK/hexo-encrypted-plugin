Add a lock for your Hexo article.

## Easy to use

1. In your blog root directory, execute command beblow:

```sh 
$ npm i hexo-encrypted-plugin 
```

2. Set password in the article which you want it to get locked

```ejs
---
title: Chrome插件迁移至Manifest V3
urlname: chrome-extension-move-to-manifest-v3
tag: chrome-extension
date: 2022-06-15
password: 123456
---

```

3. Done.

Oh wait, if you'd like to customize your own unlock style and logic

  * you can just simpliy change any content in `/blog_root/_posts/@encrypted/index.html`
  * or you can specific an existed page rendering as the dealing process, like this:
    ```ejs
    ---
    ...
    password: 123456
    encryptedModel: my-unlocking-page/
    ---
    ```

