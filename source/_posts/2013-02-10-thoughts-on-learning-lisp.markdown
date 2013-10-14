---
layout: post
title: "Thoughts on Learning Lisp"
date: 2013-02-10 12:51
comments: true
categories:
- Lisp
- Common Lisp
- Game Programming 
---

### Were I not so lucky

Having been writing Clojure (my first Lisp) and Scheme (my second) regularly over the past year, I've often wondered what my experience would've been if I *hadn't* been introduced to Lisp by [Zachary Kim](http://twitter.com/heyzk), a friend and former co-worker whom I greatly respect.

It was easy to trust him that Clojure was worth learning, worth suffering through the absurd Emacs configuration on OS X, and worth learning Emacs. The keyword being **trust**. Would I (or others) have been able to trust that recommendation if it didn't come from a good friend?

<!-- more -->

I'd love to think that my love of learning and generally patient demeanor would have gotten me through it. However, I would wager that there are many brilliant potential Lispers out there who simply wouldn't have survived the alien world of Emacs, Slime, Swank, etc. long enough to get to the fun stuff. Don't get me wrong; I love Emacs. I feel strongly however that learning Lisp doesn't mean you should have to learn Emacs, too.

### Lowering the barrier

Conrad Barski's amazing book [Land of Lisp](http://landoflisp.com/) has you simply typing expressions into the REPL[^lolrepl]. At least to me, typing hundreds of lines of Common Lisp into the REPL wasn't really going to be easy, and that's probably true for many other people. What if your laptop battery runs out, or you accidentally close your REPL? Even if you're typing everything into a file and saving it, you'd still be tediously copy and pasting code over the REPL. Not a *terrible* solution, but surely there's something simpler.

I took the opportunity to put myself in others' shoes and ask, "What's the simplest way that someone with no programming experience could make it through this book?" The obvious answer seemed to be:

* Use [Sublime Text](http://www.sublimetext.com/), which comes with a Lisp syntax mode (though there are few problems with its indentation)
* Install [Package Control](http://wbond.net/sublime_packages/package_control) for Sublime
* Using Package Control, install [SublimeREPL](https://github.com/wuub/SublimeREPL), which has built-in support for [Clisp](http://www.clisp.org/) (though Clisp needs to be installed separately, a procedure which Conrad covers in the first chapter)
* UPDATE: Grab a copy of Jonathan Fischer Friberg's excellent [Sublime Paredit](https://github.com/odyssomay/paredit) and [Sublime Lisp Indent](https://github.com/odyssomay/sublime-lispindent) plugins. Literally a Sublime Lisper's dream come true
* **(optional)** Setup [more ergonomic keyboard shortcuts](https://gist.github.com/masondesu/4699970) for SublimeREPL's "Eval in REPL" command


### That was easy!

There are a few things that I really like about this setup: 

* In less than five minutes you've got a Common Lisp REPL running in a cross-platform editor that very new-user-friendly used daily by many, many programmers.
* You can save your code in files, and *very* easily send and re-send a block, line, selection, or entire file over to be evaluated in the REPL
* At any point you can jump over the REPL and type directly into it.
* At least on OS X, Sublime (and most any OS X program) supports Emacs style keyboard navigation (`ctrl + p`, `ctrl + n`, etc.) which is a Good Thing™. Only use the mouse if you want to.
* Automatic parentheses handling
* Automatic Lisp-friendly indentation

I'm interested to hear from programmers who are new to Lisp. What else could be done to make entry into the Lisp family easier?




[^lolrepl]: At least, the exclusive use of the REPL, rather than files, hasn't changed in the first 100 pages, which is as far as I have currently read.

