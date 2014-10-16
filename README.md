BsLight
==================

A theme based on [Light](https://github.com/hexojs/hexo-theme-light) for [Hexo](http://hexo.io)

- **[Demo](http://deffi.info)**

## Install

Execute the following command and modify `theme` in `_config.yml` to `bs-light`.

```
git clone https://github.com/DaiXiang/hexo-theme-BsLight.git themes/bs-light
```

## Update

Execute the following command to update BsLight.

```
cd themes/bs-light
git pull
```

## Change Log

### 2014-10-08 Add [Swiftype](https://swiftype.com/) Support
需自行在主题配置:
```
swiftype_search:
  enable: true
  #安装码，从 swiftype 提供的代码中获取
  install_code:
  #选择 SAME PAGE 模式，需指定搜索框 ID
  search_input_selector: st-search-input
```

### 2014-08
- 增加文章目录导航，Quick Nav
  - 需要在 post 中配置 ```toc: true```
- 增加返回顶部，Return to Top
- 增加底部社交网络设置，Social Network
- 增加文章分享，Share
  - 需要在 post 中配置 ```share: true```
- 更新主题部分颜色
- 更新头部样式，Like Bootstrap
- 更新侧边栏 Widget 样式，Like Bootstrap
- 更新 Read More/Comment 链接样式和位置
  - 评论需在 post 中配置才能打开 ```comment: true```
- 优化响应式支持

## Config

Default:

``` yaml
menu:
  Home: /
  Archives: /archives

widgets:
# search/tag/category/recent_posts/tagcloud
- tag

excerpt_link: Read More

twitter:
  username:
  show_replies: false
  tweet_count: 5

social:
# key weibo/twitter/google/github/stackoverflow/rss
# value url
# e.g github: https://github.com/DaiXiang
  github: https://github.com/DaiXiang
  rss: /atom.xml

share:
# Only support Sina-Weibo/Google-Plus now
# key weibo/google
# value share link
  weibo: http://v.t.sina.com.cn/share/share.php
  google: https://plus.google.com/share

addthis:
  enable: false
  pubid:
  facebook: true
  twitter: true
  google: true
  pinterest: true

fancybox: true

google_analytics:
rss:

swiftype_search:
  enable: false
  install_code: 
  search_input_selector: # st-search-input
```

- **menu** - Main navigation menu
- **widget** - Widgets displaying in sidebar
- **excerpt_link** - "Read More" link text at the bottom of excerpted articles
- **twitter** - Twitter widget config
  - **username** - Twitter username
  - **show_replies** - Enable displaying replies
  - **tweet_count** - Tweets display in widget
- **social** - Private Social Network buttons at the buttom of site
- **share** - Share buttons at the buttom of articles
- **addthis** - Share buttons at the buttom of articles (Powered by [AddThis])
  - **enable** - Enable share buttons
  - **pubid** - Profile ID of [AddThis]
  - **facebook** - Enable Facebook button
  - **twitter** - Enable Twitter button
  - **google** - Enable Google+ button
  - **pinterest** - Enable Pinterest button
- **fancybox** - Enable [Fancybox]
- **google_analytics** - Google Analytics ID
- **rss** - RSS subscription link (change if using Feedburner)