---
layout: post
title: Try This out
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

# run locally

	bundle exec jekyll serve

# commit changes and update site

    git add .
    git commit -am 'update'
    git push origin master


