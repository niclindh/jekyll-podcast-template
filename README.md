# Jekyll podcast template

As the name implies, this is a Jekyll template for creating a podcast site.

It is based on the standard Jekyll template and lifted many ideas from [Kinoskopie.de](https://github.com/lnwdr/kinoskopie.de)—thanks for sharing!

## What’s new
**Apr. 24, 2018:**
* Add compatibility with new Google Search podcast functionality
* Add optional Apple Splash Banner on iOS
* Update Jekyll to 3.8.0
* Add Bundler

## Features

* Includes [MediaElement][me] out of the box for playing each podcast on its own page
* iTunes-compatible RSS feed
* Responsive design
* One-stop shop for configuration

As much configuration as possible is located in the ```_config.yml``` file, so you should be able to get your site running by simply editing that file with your own information.

The included podcast has more instructions, so fire it up and listen.

## Site setup

* Edit ```_config.yml``` with your own information
* Change ```img/hero.jpg``` to your own hero image. (Though you have permission to use the included file if you want.)
* Change ```img/generic-2000.png``` to your own podcast art and tell ```_config.yml``` the name. (iTunes requires this image at 2,000 pixels square)
* Edit ```about.md``` to make it your own about page
* (Optional) If you want to use Google Analytics, uncomment those lines in ```_includes/head.html``` and put in your own code

## Episode setup

Podcasts live, creatively enough, in the ```podcasts``` directory. Make sure they are tagged mp3s.

Each podcast is a Jekyll post with extra metadata:

```yaml
layout: post
permalink: episodes/X/ #X is the episode number
title: "Title of the episode"
excerpt: "The excerpts show up on the front page list."
date: 2015-02-07 12:00:00 #Make sure to include the hour stamp
media: episode-file.mp3 #Lives in the podcasts folder
length: 7552715 #Mp3 file length in bytes. Easiest to do a Get Info in the Finder if you're on a Mac
duration: "00:14:56" #Podcast length in hour:minute:second. Make sure to put the quotes
explicit: "no" #Gives you a chance to override the explicit rating by episode
```


[me]:http://mediaelementjs.com
