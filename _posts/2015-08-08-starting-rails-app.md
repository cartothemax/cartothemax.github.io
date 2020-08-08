---
layout: post
title:  "Starting Up a New Rails App"
date:   2014-08-08 13:08:02 -0500
categories: ruby rails archive update
---
## Install Ruby

First things first though. Do you have [Ruby](https://www.ruby-lang.org/en/) installed? If you are on a Mac then the answer is yes. Ruby comes shipped with Ruby 1.8.7.

It is highly recommended that you upgrade this version for a bunch of reasons. Just google and take my word for it though. 1.9.0 brought about some major upgrades to speed and functionality for the language while 2.0.0 brought some more of all that good stuff. If your not sure what version you have go ahead jump into the Terminal application and just type `ruby -v`. This will spit back a result with the version for you.

To go about upgrading your version of Ruby is really outside of the scope of “starting a new Rails app”, but I will say I personally use [RVM](https://rvm.io/rvm/install) and rather enjoy it. This tool can handle the install of new versions of Ruby for you no problem.
## Install Rails

So, you have Ruby that’s one half of the whole [‘Ruby on Rails’](https://rubyonrails.org/) thing. Time for the Rails part. What does that entail? Let’s do a gem install of Rails. [Ruby Gems](https://rubygems.org/) are the packages that you can insall in the Ruby ecosystem for package management. You will likely use this quite a bit in any future Ruby development that you do. I predict we will be using in the very near future… like right now to install Rails actually.

Still have the terminal open from before to check what version of Ruby you have? Great. Next we will be navigating to a place on your file system that you like to keep projects and make a directory to house our Rails project. Then go into the newly created folder.
```bash
cd ~/Documents
mkdir rails_application
cd rails_application
```

Now we do a little Rails magic.
```bash
gem install rails
```

This can take a little bit of time as it retrieves all of the necessary pieces that make up Rails. When that is all finished up though we have now installed the Rails half of ‘Ruby on Rails’ and that’s the whole shabang.
## Pulling it all together

Let’s get started then. We have Ruby installed and now have Rails installed. In the command prompt type the following.

```bash
rails new foo_bar
```

This is a built in command from Rails that will generate the basic pieces that we need in order to create our rails application. The ‘foo_bar’ part is the name of our newly created application. Feel free to do whatever you want.

If you do a quick `ls` command you will see that we have another newly created folder called `foo_bar` (unless of course you named yours something different!). `cd` into this newly created folder and issue another `ls` command.

This is loosely what you should see.

```bash
Gemfile README.rdoc app\ config\ db\ log\ test\ vendor\ Gemfile.lock Rakefile bin\ config.ru lib\ public\ tmp\
```

I highly recommend exploring a bit from here. The `/app` directory is where the pieces that make up your application will live. These pieces include the code that will make up your models, views, and controllers. The other folders are for various key components outside of what your application is.

Now the most powerful piece of Rails is that we have now ‘created’ a rails application. From the top level directory of our application `~/Documents/rails_application/foo_bar/` we can issue the command `rails server` and our Rails app is all started up and running locally. In the output after issuing that command look for the port=xxxx (mine is port 3000 yours likely will too). Open up your favorite web browser and go to `http://localhost:3000`.

Boom! We have ourselves the most basic rails app imagainable that does nothing, but hey, it’s a rails application none the less. Later we will explore the individual pieces that make up the a Rails application and discuss each.
