## Header Name

To use the power of CSS Content and media query, the header name is defined on [src/styl/_header.styl](src/styl/_header.styl). Change to your prefered name.

## Color customization

All color variables are in [src/styl/_variables.styl](src/styl/_variables.styl). To change the main color, just set the new value at `main` assignment. Another colors are for texts and the code background color.

## Theme Colors

Every post has a main color that is defined on [src/styl/_theme-colors.styl](src/styl/_theme-colors.styl). Just create a new color with the prefix `post-` and define your main-class: 'css' and color: '#2DA0C3' on every post you create.

## Creating posts

You can use the `initpost.sh` to create your new posts. Just follow the command:

```
./initpost.sh -c Post Title
```

The new file will be created at `_posts` with this format `date-title.md`.

## Front-matter 

When you create a new post, you need to fill the post information in the front-matter, follow this example:

```
---
layout: post
title: "Falando sobre RSCSS"
date: 2016-02-07 18:48:16
image: '/assets/img/rscss/rscss.png'
description: 'Escrevendo CSS sem perder a sanidade. Aprenda uma metodologia que pode salvar muitas dores de cabeça.'
main-class: 'css'
color: '#2DA0C3'
tags:
- css
- metodologia
- frontend
categories:
twitter_text: 'Escrevendo CSS sem perder a sanidade.'
introduction: 'Escrevendo CSS sem perder a sanidade. Com essa introdução, Rico St. Cruz o criador chama a atenção de todos sobre uma metodologia melhor para se escrever CSS.'
---
```

## Running the blog in local

In order to compile the assets and run Jekyll on local you need to follow those steps:

- Install [NodeJS](https://nodejs.org/) (remember to use the latest version)
- Run `npm install`
- Run `npm install -g gulp gulp-cli`
- Run `gulp`
