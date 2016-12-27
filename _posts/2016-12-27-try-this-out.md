---
layout: post
title: Try This out
published: true
---
# make a folder

    mkdir jekyll

# move into the folder

    cd jekyll

# clone my example

    git clone git@github.com:jayCorp/jaycorp.github.io.git
    
    cd jaycorp.github.io

# install dependencies

    bundle install

# add new post

    bundle exec jekyll post 'a new post for the blog'
    
# edit post

	_posts/2016-12-27-try-this-out.md
    
Edit in wysiyg editor
[http://prose.io/#jayCorp/jaycorp.github.io/edit/master/_posts/2016-12-27-try-this-out.md](http://prose.io/#jayCorp/jaycorp.github.io/edit/master/_posts/2016-12-27-try-this-out.md)


# run locally

	bundle exec jekyll serve

# commit changes and update site

    git add .
    git commit -am 'update'
    git push origin master
