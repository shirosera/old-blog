---
title: "Support Multi language in Hugo Blog"
date: 2024-02-25T22:05:27+09:00
draft: false
toc: true
images:
categories: ["Tech"]
tags:
  - Hugo
  - Tech
  - Web
  - i18n
---

## TL;DR

Support multi language in Hugo
Change default language  
  
## Background

When I was creating a blog with Hugo, I saw that it was multilingual and wanted to make it compatible. that's all.

## Let's do 

Located in `./hugo.toml`
```toml 
enableGlobalLanguageMenu = true
```
Set this to true. That's all. 

## Change Default display language

Apparently, if this continues, English will be displayed by default.  
To fix this, in `./hugo.toml`
```toml
hasCJKLanguage = true defaultContentLanguage = "ja" 
```
This will allow you to set the language counter and Japanese as the default.  
  
This took all of 2 hours.  
That's end!  
:wq
