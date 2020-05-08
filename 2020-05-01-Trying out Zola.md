---
layout: post
title:  "Trying out Zola"
date:   2020-05-01 00:01:00 +0800
categories: it
draft: true
---

This article is about:
* Testing the Open Source Static Site Generator Zola

Structure of Blog Article:
...

# Intro

So far I have used several technical solutions to set up a blog on my homepage. Unfortunately I am still not satisified with it. A rough overview about the solutions that I have tried:

### Classic CMS:
* Wordpress
* Mezzanine
* Ghost

### Static Site Engines:
* Jekyll

In general I like the idea of the Static Site Engines, to host a blog. It gives you full control of the content. Perfect for savvy people like me. [TODO]

# A new try - Zola

So today I will try Zola. On this [Github-Repo](https://github.com/getzola/zola) you can find some advantages and disadvantages. The fact that Jekyll is not even mentioned there gives me some hint, that maybe Jekyll was really not the best choice to go on anymore. On the website https://www.getzola.org/ you can read some more details about it. The point that there are no dependencies catched my attention and is for me the unique selling point of it. The fact that it is written in Rust also raised my attention as I am thinking of trying out Rust soon for a networking tool that I thought of would be handy for my work. 

As it says that it has no dependancies I am curious to install Zola on a Linux Alpine (which is under 10MB):

Let's start a fresh new Linux Docker Container via `docker run --rm -it --name=zola alpine sh`

Inside this container I am running 

```bash
apk add curl # tar # download curl to download the zola binary
mkdir /home/testingzola/; cd /home/testingzola/
curl -o zola.tar.gz -L https://github.com/getzola/zola/releases/download/v0.10.1/zola-v0.10.1-x86_64-unknown-linux-gnu.tar.gz
tar -zxvf zola.tar.gz
rm zola.tar.gz
```


