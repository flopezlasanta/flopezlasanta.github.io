---
layout: post
title: "Blog with GitHub Pages and Jekyll"
date: 2016-06-27
categories: github jekyll blog
---

I always wanted to create a blog about **software development**. Initially I explored [WordPress](https://wordpress.com/), [Tumblr](http://www.tumblr.com/), and [Ghost](https://ghost.org/).

However I ended up choosing the combination [Github Pages](https://pages.github.com/) plus [Jekyll](https://jekyllrb.com/):

- Github Pages is a hosting service provided by [GitHub](https://github.com/)
- Jekyll is a [Ruby](https://www.ruby-lang.org/) gem that renders [Markdown](https://guides.github.com/features/mastering-markdown/) templates to produce a complete, static website

Together they make easy to create and maintain a website:

- The hosting site is provided automatically
- Contents are based on Markdown rather than HTML
- Contents are transferred to the site updating your GitHub repository with ```git``` commands

The **development environment** used to create this site is based on:

- OS: OS X 10.11.5 El Capitan
- Package Manager: [Homebrew](http://brew.sh/)
- Editor: [Sublime Text 3](https://www.sublimetext.com/3)
- Terminal: [iTerm2](https://www.iterm2.com/)

The **initial steps** followed to create this site were the following:

- Create a GitHub repository according to the guidelines mentioned in [Github Pages](https://pages.github.com/)
- Install Jekyll in local: ```gem install jekyll```
- Create a new site based on the GitHub repository name: ```jekyll new flopezlasanta.github.io```
  - Information about files and folders automatically created is available at [Jekyll > Directory Structure](https://jekyllrb.com/docs/structure/)
- Modify the file ```_config.yml``` with the site name and contact information (email address, GitHub username, ...)
- Modify the file ```about.md``` with an introduction about you (areas of interest, [LinkedIn](https://www.linkedin.com/) profile, ...)
- Run ```jekyll server``` and then ```open http://127.0.0.1:4000/``` to check there are no errors and everything looks OK locally
- Push the Jekyll site to the GitHub repository as explained in [Github > Add Project to Repository](https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/)
- Wait a few minutes and then browse to the public URL: ```open https://flopezlasanta.github.io```

Some additional changes to address **site identity and browsing** were the following:

- Add a file ```robots.txt``` to give instructions about the site to web robots (see [robotstxt.org](http://www.robotstxt.org/robotstxt.html))
- Add a file ```keybase.txt```, obtained from [keybase.io](https://keybase.io/), to confirm the digital identity of the site owner
- Add a file ```googleXXX.html```, obtained from [Google Webmaster Central](https://www.google.com/webmasters/verification), to tell Google of the site ownership

<strong>Note: this post will be extended with information about the way to create a post and to customize the theme</strong>