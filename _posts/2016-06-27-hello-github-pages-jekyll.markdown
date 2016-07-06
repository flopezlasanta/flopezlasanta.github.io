---
layout: post
title: "Create blog with GitHub Pages and Jekyll"
date: 2016-06-27
categories: github jekyll blog
comments: false
---

Creating (and maintaining) a blog about technical stuff is something I wanted to do since a long time ago. There are multiple options to do that: [WordPress](https://wordpress.com/), [Tumblr](http://www.tumblr.com/), [Ghost](https://ghost.org/)... However lately I am using [GitHub](https://github.com/) quite a lot and because of that I ended up choosing [Github Pages](https://pages.github.com/) and [Jekyll](https://jekyllrb.com/). The learning curve is really simple and they provide pretty much everything needed (to start with). 

In this post, my first one, I'll share the steps followed to create this blog using such tools. It's in a very early stage thus (constructive) comments to make it better are more than welcome.

Environment
-----------

- OS: OS X 10.11.5 El Capitan
- Editor: [Sublime Text 3](https://www.sublimetext.com/3)
- Package Manager: [Homebrew](http://brew.sh/)


Basics
------

1. Create a new git repository according to the guidelines mentioned in GitHub Pages _(tip: set .gitignore for Jekyll contents)_.
2. Install Jekyll in local.
3. Create a new Jekyll site using as site name the repository name.
4. Modify the file **_config.yml** with the site name and with your contact information.
5. Modify the file **about.md** with an introduction about you.
6. Add the Jekyll site to the repository following the steps mentioned in [Github > Add Project to Repository](https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/).
6. Enjoy your recently created site browsing to its public URL.

Identity
--------
1. Add a file **robots.txt** to give instructions about the site to web robots, see [robotstxt.org](http://www.robotstxt.org/robotstxt.html).
2. Add a file **keybase.txt** obtained from [keybase.io](https://keybase.io/) _(requires to login with a Keybase account)_ to confirm the digital identity of the site owner.
3. Add a file **google65fe8dc7fdb34030.html** _(file name should be a different one)_ obtained from [Google Webmaster Central](https://www.google.com/webmasters/verification) _(requires to login with a Google account)_ to tell Google of the site ownership.

**TO BE COMPLETED**