---
layout: post
title:  "Why use Github Pages for a site?"
date:   2020-08-05 15:56:02 -0500
categories: jekyll update tech
---
This is now the third version of a personal site for me. Or is it the fourth? Either way I have thrown and built from scratch my personal website multiple times now.

The latest iteration of this site is reusing [Github Pages](https://pages.github.com/). This is a free resource that comes with having a [Github](https://github.com) account.

Previouly I have used Github Pages for hosting my personal site, but went away from it in favor of [Wordpress](https://wordpress.com/) using a hosted solution provided by [Namecheap](https://namecheap.com). Using Wordpress/Namecheap was _ok_, but at the end of the day I spent more time fiddling with the configuration/certificates/themes then I did actually writing anything meaningful.

The amount of "I have rebooted my blog to this new platform" type posts is really high. Those posts are usually the last thing that was written on the site too! For me this was because I would just get sucked into losing hours of setup with Wordpress. Anyway.. here is another "I have rebooted my blog to this new platform" type post

To start with it is a toolset that I am very familar with. Github/[`git`](https://git-scm.com/)/[markdown](https://www.markdownguide.org/)/[Ruby](https://www.ruby-lang.org/en/). These are all technologies that either have or do currently use in my day to day of work. Plus having the posts be in markdown means that it's just editing a text file and I am able to use [VSCode](https://code.visualstudio.com/) and [VIM](https://www.vim.org).

Being able to deploy an update by simply using `git push` is both natural and powerful. In addition to the familiarity I am able to easily roll back changes or revert to a previous version of the site (as long as I use good commits :D)

Having markdown be the underlaying technology for editing posts makes it easy and natural for sprinkling code snippets or adding **empathsis** to make a *meaningful* ***point***. Wordpress (or any other CMS) of course can can do the same things of markdown, but markdown at the end of the day is just a text file and not a blob in a database with proprietary synatax.

When I point out Ruby as a selling point for Github Pages I should be pointing out the power of [Jekyll](https://jekyllrb.com/) as that is really the backbone of a site deployed to Github Pages and Jekyll is built using Ruby. Being familiar with the underlying technology that powers Jekyll means I can get my hands dirty for making changes to the formatting or layout (maybe I can create my own theme!)

Finally being able to edit the markdown files using VSCode with the VIM plugin feels considerably faster and more powerfuly the usual text area editing that a typical CMS gives you.

Being able to reuse the tools of my day to day really lowers the friction to creating posts in my experience. This post honestly took less time then just figuring out how to get going on a new post with my old Wordpress site. Here's to hoping this isn't another stale personal site with only a "I have rebooted my blog to this new platform" post.
