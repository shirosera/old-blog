---
title: "Hugoを多言語対応させた話"
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

Hugoで複数言語対応にした。  
元々複数言語対応のテーマを使っていたので簡単に実装できた。  
デフォルト言語設定を忘れていた。  
  
## 背景

Hugoでブログ作成中に多言語対応というのを見て対応させたくなった。以上。 

## とりあえずやってみる

`./hugo.toml`内にある


```toml
enableGlobalLanguageMenu = true
```

これをtrueにする。  
それだけの話。  

## デフォルト表示の変更

どうやらこのままだと英語がデフォルトで表示されてしまう。  
これを修正するには`./hugo.toml`内の

```toml
hasCJKLanguage = true
defaultContentLanguage = "ja"
```
これで言語カウンターと日本語のデフォルト化ができる。  
  
これに2時間取られたよ全く。  
おわり！:wq
