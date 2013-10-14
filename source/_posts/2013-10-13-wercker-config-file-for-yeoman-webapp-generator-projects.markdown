---
layout: post
title: "Wercker config file for Yeoman Webapp generator projects"
date: 2013-10-13 21:02
comments: true
categories:
- Continuous Integration
- Node.js
- Yeoman
- Grunt
- Bower
- Mocha
- JavaScript
---

### Getting Wercker to test your Yeoman Webapp
[Wercker](http://wercker.com/) is a great continuous integration service that works well with just about any stack or application, including apps built with [Yeoman](http://yeoman.io/)'s ubiquitous [Webapp Generator](https://github.com/yeoman/generator-webapp). I've been using Wercker for about 3 months now and have loved it. The Wercker team is very friendly and has been helpful on numerous occasions.

<!-- more -->

As their platform is new, writing config files can be a little vague. I thought I'd share the `wercker.yml` file needed to test a vanilla app created with the Yeoman Webapp Generator. Bear in mind, you'll need to run `npm install --save bower` to make sure that Bower is installed on the test server's VM. After that, just drop this in the root of your repo, push it, and add your repo to Wercker at https://app.wercker.com

<script src="https://gist.github.com/masondesu/6969216.js"> </script>