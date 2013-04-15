---
layout: post
title: "Enable wake_lock by manual"
date: 2013-04-15 12:04
comments: true
categories:
- Android
---

Enable wake_lock by manual to avoid android entering suspend mode

``` bash Bash
adb shell
echo mylock > sys/power/wake_lock
```
