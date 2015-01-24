---
layout: post
title:  "Bower exit code of #69"
date:   2014-02-23
categories:
  - front-end
tags:
  - xcode
  - mavericks
  - bower
---
I'm trying out Bower today, but I ran into an issue where it didn't want to install any package: exit code of #69.

If you run into the same issue, you should run Xcode and accept the user agreement.

`$ bower install bootstrap`

`bower not-cached    git://github.com/twbs/bootstrap.git#*`

`bower resolve       git://github.com/twbs/bootstrap.git#* `

`bower ECMDERR       Failed to execute "git ls-remote --tags --heads git://github.com/twbs/bootstrap.git", exit code of #69`

`Additional error details:`

`Agreeing to the Xcode/iOS license requires admin privileges, please re-run as root via sudo.`

In some way the description describes what the problem is, but since I never really use Xcode and I don't know anything about an iOS license it kind of looks like gibberish to me.

Since I happened to update my Macbook to Mavericks yesterday, Xcode also got an update and that's where the issue originates.

To solve it just open Xcode and accept the user agreement. After that Xcode installs a bunch of packages. When it's done you're allowed to install Bower packages again.

Pretty easy, right?
