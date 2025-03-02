# How to write a guide

## Dictionary

[Find the dictionary here](./dictionary.md)

## Intro

In order to write a guide in the [guide section](https://www.kaiden.gg/tribe-nine/guides/) of Kaiden.gg, you'll need to create:

* A markdown file `my-guide-name.md` ([what is a markdown file?](https://www.markdownguide.org/basic-syntax/)) which will contain all the text, links to all the assets used in the guide (images, videos, etc). The filename should be a slug and it will be important as the URl created on the website will contain the same name of this file (ex: in this case: `kaiden.gg/game/guides/my-guide-name/`. From now on, `{guide-name}` is exactly this filename.
* An `assets/my-guide-name` folder containing all the assets

## Markdown file

The markdown file is composed by two main components. The front matter and the body.

### Front matter

```yaml
---
title: Tribe Nine Reroll guide
description: Guide on how to reroll in Tribe Nine
h1: Reroll Guide
subtitle: Guide on how to reroll in Tribe Nine
icon: /img/tribe-nine/guides/stripes/reroll-guide.webp
author: gooseofsiliness
showHeading: true
eleventyNavigation:
  key: t9-guides-reroll
  parent: t9-guides
  url: /tribe-nine/guide/reroll-guide/
  title: Reroll Guide
---
```

In particular:

`---` Start delimiter of the front matter

`title` HTML title of the webpage. It should contain the name of the game you're writing a guide to and the name of the guide. ex: *Tribe Nine The best guide in the world* (try to be quite concise here) ~60 chars

`description` HTML description meta tag of the webpage. Here you can be more descriptive and less concise, so write a quick summary ~200 chars

`h1` Similar to title, it's the heading 1 (main heading) of the page. It should be similar to the tile, but without the game name as it'll be displayed this time on the webpage

`subtitle` Similar to description meta tag, but it's showed on the webpage. Could be really similar if not the same as description

`icon` The icon/image that will be displayed on the main Guide index. It should have this format `/img/{game-name}/guides/stripes/{guide-name}.webp` (ex: `/img/tribe-nine/guides/stripes/my-guide-name.webp`). Don't care about uploading or providing an image. The staff will create one for you

`author` Your name. it should be in kaiden's format, so if you don't know it, ask to the staff!

`showHeading` Either `true` or `false`. It should be always true with few exceptions (for example the guide have it's own particular header) ([see image](./img/heading.png))

`eleventyNavigation` Main tag to configure to properly see the breadcrumb in the webpage ([see image](./img/heading.png)). The tab (teo whitespaces) you find on the next properties SHOULD remain, of the webpage could have problems to render.

`eleventyNavigation.key` Your own UNIQUE identified. Uses a prefix related to the `parent` property, an it will contain the name of the guide in slug format (ex: t9-guides-my-guide-name)

`eleventyNavigation.parent` Guide index identifier for the related game. If unsure, ask the staff

`eleventyNavigation.url` URL of thebreadcrumb. SHOULD be: `/{game-name}/guides/{guide-name}`

`eleventyNavigation.title` Title of the breadcrumb. Really short (ex: `My Guide`)

`---` End delimiter of the front matter

### Body
