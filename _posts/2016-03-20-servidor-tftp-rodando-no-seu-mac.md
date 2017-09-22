---
id: 921
title: Servidor TFTP rodando no seu Mac!
date: 2016-03-20T09:50:35+00:00
author: Gustavo Aguiar
layout: post
guid: http://www.sysadmin.com.br/?p=921
permalink: /servidor-tftp-rodando-no-seu-mac/
sj-html-to-post-shortcode:
  - ""
sj-css-to-post:
  - ""
sj-js-to-post:
  - ""
ipt_kb_like_article:
  - "0"
tags:
  - cisco
  - macos
  - network
---
Hummmm&#8230; então você precisa de um servidor TFTP para transferir arquivos (digamos que imagens de um roteador Cisco)&#8230; qual seria a maneira mais fácil/rápida de fazer isso ? Instalar um tftpd em um servidor ? Ou quem sabe rodar isso localmente no seu Mac ?

O Mac tem um servidor built-in e basta inicia-lo&#8230; rapido e limpo. Como fazer isso ?

`sudo launchctl load -F /System/Library/LaunchDaemons/tftp.plist<br />
sudo launchctl start com.apple.tftpd`

A pasta padrão é **/private/tftpboot** mas você pode muda-la em **/System/Library/LaunchDaemons/tftp.plist**.

Espero que ajude! <img src="http://www.sysadmin.com.br/wp-includes/images/smilies/icon_wink.gif" alt=";-)" class="wp-smiley" />
