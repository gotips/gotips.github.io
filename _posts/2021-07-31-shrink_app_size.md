---
layout: post
title: SHRINK your Go application 🚀️ build size by ~30% just by adding a flag to build command
date: 2021-07-31 10:20:58 +0530
tags: build
---

Go provides a linker flag to eliminate debug information and DWARF tables while building executables.

Have a look at this minimal web server and observe the build size. The build size reduces to 4.4M from 6.2M. [This blog explains it in detail.](https://blog.filippo.io/shrink-your-go-binaries-with-this-one-weird-trick/)

This does not affect the stack trace.

PS: I know binary size does not matter these days, but this information is worth knowing.

Driver code -
![IMAGE](/images/shrink_size_1.jpg)

Result -
![IMAGE](/images/shrink_size_2.jpg)
