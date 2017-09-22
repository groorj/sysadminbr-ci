---
id: 919
title: Linux::History com datetime
date: 2016-02-19T16:41:34+00:00
author: Luiz Fernando Mascarenhas
layout: post
guid: http://www.sysadmin.com.br/?p=919
permalink: /linuxhistory-com-datetime/
sj-html-to-post-shortcode:
  - ""
sj-css-to-post:
  - ""
sj-js-to-post:
  - ""
ipt_kb_like_article:
  - "0"
tags:
  - linux
---
Basta criar o seguinte script

`/etc/profile.d/history_timestamp.sh<br />
` 
  
Com o conteúdo abaixo:
  
`#/bin/bash<br />
## This is a customization to allow to show timestamp when using history<br />
export HISTTIMEFORMAT='%F %T '`

Ex:
  
  `998  2016-02-19 18:34:15 history<br />
  999  2016-02-19 18:39:45 ps aux<br />
 1000  2016-02-19 18:39:52 cd /var/log`