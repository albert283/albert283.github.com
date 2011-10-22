---
layout: post
title: "Script to get ip address"
date: 2011-10-22 19:10
comments: false
categories: [script, linux, shell]
---
``` bash Bash
ifconfig | grep 'inet addr:' | grep -v '127.0.0.1' | cut -d: -f2 | awk '{print $1}'
```