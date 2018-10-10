# CHIRIMENホームページのソースコード

## chirimen-ohのサイトを編集する手順について
1. issueを作る
1. fork して pull-req  or  ブランチ して pull-req
1. Merge する
1. 基本的にmaster は、直接いじらない

[![Build Status](https://travis-ci.org/chirimen-oh/chirimen-oh.github.io.svg?branch=master)](https://travis-ci.org/chirimen-oh/chirimen-oh.github.io)

### 初期設定

#### 必要なソフトウェアのインストール

ローカルでGitHub Pagesのローカル環境を起動するのに Docker が必要になります。
MacOSX や Windows をご利用の場合は、以下のようなソフトウェアをインストールして `docker` コマンドが利用できるようにしてください。

 + Docker
   + MacOSをご利用の方: [Docker for Mac](https://docs.docker.com/docker-for-mac/)
   + Win10をご利用の方: [Docker for Windows](https://docs.docker.com/docker-for-windows/)
   + Windows(10以外)をご利用の方: [Docker Toolbox](https://docs.docker.com/toolbox/overview/)

### ブログの書き方

公式ドキュメントの[Post を書く](http://jekyllrb-ja.github.io/docs/posts/)を参照してください。

### 確認の仕方

以下のコマンドを実行後 http://localhost:4000 にアクセスするとWebページが表示されます

```
$ docker run -t --rm -v "$PWD":/usr/src/app -p "4000:4000" starefossen/github-pages

Configuration file: /usr/src/app/_config.yml
       Deprecation: The 'gems' configuration option has been renamed to 'plugins'. Please update your config file accordingly.
            Source: /usr/src/app
       Destination: /_site
 Incremental build: disabled. Enable with --incremental
      Generating... 
    Liquid Warning: Liquid syntax error (line 21): Expected id but found number in "{{ site.404-img }}" in /_layouts/error.html
                    done in 2.465 seconds.
 Auto-regeneration: enabled for '/usr/src/app'
    Server address: http://0.0.0.0:4000
  Server running... press ctrl-c to stop.
```

ローカルのファイルが変更されると、自動的にビルドが実行されるので、ページをリロードするだけで大丈夫です。

```
      Regenerating: 1 file(s) changed at 2018-09-05 10:43:11     Liquid Warning: Liquid syntax error (line 21): Expected id but found number in "{{ site.404-img }}" in /_layouts/error.html
...done in 2.151323191 seconds.
```

終了するときは、`Ctrl+C` でコンソールを止めたあとで、以下のコマンドを実行してください。

```
$ docker stop $(docker ps -q --filter ancestor="starefossen/github-pages" )
```

### リリース方法

 *  問題がある場合はissuesに上げてください、
    その後実装担当者はforkもしくは別ブランチを切って修正後、プルリクエストを当リポジトリのmasterへ送ってください。

 * 自分で問題を対応できる場合は、即fork後修正し、プルリクエストから開始しても問題有りません。


-----
## Original Readme Content

[![Join the chat at https://gitter.im/PanosSakkos/personal-jekyll-theme](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/PanosSakkos/personal-jekyll-theme?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

# { Personal } Jekyll Theme

{ Personal } is a free responsive Jekyll theme, about you :wink:

You can watch it in action [here](https://panossakkos.github.io/personal-jekyll-theme/)!

## What value does { Personal } add

* Fork of [Timeline](https://github.com/kirbyt/timeline-jekyll-theme) (mashup of [Grayscale by Start Bootstrap](https://github.com/IronSummitMedia/startbootstrap-grayscale) and [Agency Jekyll Theme](https://github.com/y7kim/agency-jekyll-theme))
  * Modern and minimal design
    * Responsive templates for home page, blog archive and posts. Looks great on mobile, tablet, and desktop devices
    * Sweet animations
    * Gracefully degrades in older browsers. Compatible with Internet Explorer 8+ and all modern browsers
  * Timeline
    * Tell your story so far with a sleek timeline of dates, pictures and descriptions
  * White on black text, making the reading experience tireless
  * Google analytics  
* Customization and full control of your website and blog through the site config
* Customization of the website's coloring
* Blogging functionality
  * Preview of the latest post in the home page
  * Archive page
  * Syntax highlighting
  * Emojis
  * Gesture navigation in archive and post pages by swiping
  * Hashtags
  * Categories
  * Disqus comments
  * Bootstrap share buttons
  * RSS feed
* Author blurb under the posts
* 404 page
* iOS and Android Web App mode
* Enforcing of https protocol
* Protection from email harvesting
* Sitemap
* Travis CI integration with [html-proofer](https://github.com/gjtorikian/html-proofer)

## { Personal } à la JekyllNow

Want to get { Personal } without messing with jekyll installations and terminal commands?

  1. Fork the personal-jekyll-theme repository
  2. Rename the forked repository to yourgithubusername.github.io
  3. Visit https://yourgithubusername.github.io
  4. Start modifying the \_config.yml and editing your blog's posts from Github's online editor or a third party online editor (i.e. [Prose](https://prose.io/))

## Documentation

The theme contains documentation in the form of [blog posts](https://panossakkos.github.io/personal-jekyll-theme/blog/index.html).

## Screenshots
### Header
![Intro](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/index.jpg)
### About
![About](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/about.jpg)
### Latest post preview
![Blog](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/blog.jpg)
### Timeline
![Timeline](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/timeline.jpg)
### Blog Archive
![Archive](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/archive.jpg)
### Gesture navigation instructions
![Instructions](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/swipe.jpg)
### Post page
![Post](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/post.jpg)
### Author blurb
![Blurb](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/blurb.jpg)
### Hashtags
![Tags](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/tags.jpg)
### Categories
![Categories](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/categories.jpg)
### 404
![404](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/404.jpg)
### Mobile rendering
![Web App](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/web-app.jpg)
### Web App mode

![iOS](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/ios.jpg)

![Android](https://dl.dropboxusercontent.com/u/8522559/personal-jekyll-theme/pinned.jpg)

## How to run locally

First, you need to install jekyll and the dependencies of { Personal } by running:

````
./scripts/install
````

Then, you can build and serve your website by simply running:

````
./scripts/serve-production
````

## Wiki

Don't forget to list your { Personal } blog in the [Blogs using { Personal }](https://github.com/PanosSakkos/personal-jekyll-theme/wiki/Blogs-using-%7B-Personal-%7D) wiki page in order to drive some traffic to your website :wink:

## Integrating bug fixes and features into your old fork

Have you published your own website by forking { Personal } and now you want to get the latest bug fixes and features from this repo into your website?
Then check [this](https://github.com/PanosSakkos/personal-jekyll-theme/wiki/Upgrading-your-%7B-Personal-%7D-website-with-our-latest-bug-fixes-and-features) out.

## OSS used in { Personal }

One of the reasons { Personal } is real is the following OSS projects:

  1. [Grayscale](http://startbootstrap.com/template-overviews/grayscale/)
  2. [hammer.js](https://hammerjs.github.io/)
  3. [highlightjs](https://highlightjs.org/)
  4. [RRSSB](https://github.com/kni-labs/rrssb)
  5. [Timeline](https://github.com/kirbyt/timeline-jekyll-theme)
  6. [typed.js](https://github.com/mattboldt/typed.js/)

## Supporting the repo

Proposals, pull requests and issues are more than welcome, let's make the web a bit more beautiful and secure :wink:

In case you want to say thank you by donating Bitcoins to all the contributors, [this](https://blockchain.info/address/1LHuKC9Em3KA5yoZaf7nngnNdf9K7s2gSi) is our address.
