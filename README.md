#abco.re [![Build Status](https://travis-ci.org/greenaddress/abcore.svg?branch=gh-pages)](https://travis-ci.org/greenaddress/abcore)

This repository is the source code of the ABCore project website built with Jekyll.

<<<<<<< HEAD
## Directory structure
=======
Warning: This app is still in a very Proof of Concept/Alpha stage.
If you want to try it get it from the Play Store (opt-in https://play.google.com/apps/testing/com.greenaddress.abcore) or directly from GitHub https://github.com/greenaddress/abcore/releases/tag/v0.23alphaPoC
>>>>>>> greenaddress/master

  - `_posts/<lang>/posts` for blog articles.
  - `_posts/<lang>/pages` for static pages.
  - `_posts/<lang>/releases` for Bitcoin Core release notes

File names *must* be in the format `Y/m/d-title.md`, e.g. `2015-12-31-title.md`. File names can be translated.

## Translations

Menu and miscellaneous translations can be found in:

  - `_data/lanaguges.yml`
  - `_data/navgation.yml`
  - `_data/translations.yml`
  
## Front Matter notes

The following `Front Matter` is required for the multilingual setup in all files. The required fields are as follows:

  - `name:`      group name for unique article. Each translation must share the same group name, e.g. `october15-report`
  - `id:`        each article translation must have a unique ID. Use the language code + `-name` field. e.g. `en-october15-report`
  - `permalink:` the ML permalink must include the language code, e.g. `/en/2015/12/31/report`. Permalinks should be translated.
  - `title:`     the translated title of the article

```
---
name: short-title
id: en-short-title
permalink: /en/2016/01/01/short-title
title: Short Title
---
```

## Building

This website is based on Jekyll. To build locally, [install Ruby 2.2.3](https://gorails.com/setup) or greater
and then run the following commands:

    gem install bundle
    bundle install
    
To preview the site (this will launch a tiny webserver on port 4000):

    bundle exec jekyll server

To simply build the site (output placed in the `_site` directory):

    bundle exec jekyll build
    
To test the site:

    bundle exec jekyll build && bundle exec htmlproof ./_site

<<<<<<< HEAD
## Contributing
=======
Icon & Web Design

Ottavio Fontolan otta88.box (at) gmail (dot) com

Testing & UX

Gabriele Domenichini twitter.com/gabridome

Special thanks to the Bitcoin Dev team, the Debian and Arch Linux teams and to github.com/Polve for JavaBitcoindRpcClient.
>>>>>>> greenaddress/master

Contributions welcome. Please see [CONTRIBUTING.md](/CONTRIBUTING.md) for details.

