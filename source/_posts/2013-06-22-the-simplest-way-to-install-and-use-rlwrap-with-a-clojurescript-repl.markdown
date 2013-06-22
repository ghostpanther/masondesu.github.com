---
layout: post
title: "The simplest way to install and use rlwrap with a ClojureScript repl"
date: 2013-06-22 18:05
comments: true
categories: 
- Lisp
- Clojure
- ClojureScript
- rlwrap
---

### Arrow keys not working in your ClojureScript repl?
For some reason, whenever I would run `lein trampoline cljsbuild repl-listen` while setting up a ClojureScript browser repl, all arrow keys, Emacs style navigation (`ctrl-p`, etc.), and history were not working. They worked fine in the normal `lein repl`, but something went wrong either with trampoline, cljsbuild, or both. Either way, Google informed me that I should probably be using a tool called rlwrap to fix it. 

### Installing rlwrap on OSX
There are lots of articles about installing rlwrap into your clojure folder and running some awful looking Java commands, but there's a much easier way: just use Homebrew to install it. `brew install rlwrap` will get you set up, and then you'll be able to run `rlwrap lein trampoline cljsbuild repl-listen` with fully functional arrow keys and history. You'll even get back the old-school flashing cursor when you match parens. Righteous!