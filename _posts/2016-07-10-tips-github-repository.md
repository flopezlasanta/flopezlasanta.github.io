---
layout: post
title: "Tips for GitHub Repositories"
date: 2016-07-10
categories: github
---

[GitHub](https://github.com/) is awesome for publishing code. This post shares some common steps to consider when creating a development project / repository in there.

- Initialize with a README so that the repository can be cloned immediately
- Add ```.gitignore``` according to the technologies to be used
- Add a license according to the scope of the project (for instance [MIT](https://opensource.org/licenses/MIT))
- Follow the standard directory layout based on the programming language used (for instance [Maven](https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html)'s for Java projects)
- Configure CI for your project with one of the proper [GitHub integrations](https://github.com/integrations/) (for instance [TravisCI](https://travis-ci.com/)
- Update ```README.md``` with the project description and getting started material (and use [Markdown](https://help.github.com/articles/github-flavored-markdown/) for that)
- Update ```README.md``` with images from [shields.io](http://shields.io/) reporting about the CI status, license used, etc

For a very complete list of cool hacks, check out [this](https://github.com/tiimgreen/github-cheat-sheet).

