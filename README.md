# JSON-to-JS-Presentation
A small HTML5 app that takes JSON\* and makes a swooshy full screen presentation with it using arrow keys

\* It's really just an array of JS objects, but it looks JSON-y enough...

## What
In the `bin` folder you will find a file called `index.html`. If you look at the code, and know how to edit JSON/JavaScript objects, there should be enough in there to get you started for making a multimedia slide presentation, where the slides comes _swooshing_ towards you in 3D on the Z-axis. (OOoh, aaah, wow!) CSS transitions are really neat!

## How
I used mostly CSS3 transforms while manipulating HTML-element DOM objects with JavaScript to make it happen.

In order to use it, grab `index.html` and put it into its own folder, then make a directory called `media` next to the HTML-file. That's where you should put your images, videos and sound, and stuff. Then edit the HTML-file to put more JSON-slides into the `slides` array.

## Why
I just had to do this because MS PowerPoint made the sound lag on videos in the presentation. Can't have that when my pupils want their local equivalent of the Oscar's!

## To Do
This is pretty dirty code, and there's still a lot of work to be done on this project. For instance the design really only works in full screen on a big computer monitor. :p For one, a way to make fonts scale in a polite manner is badly needed. Also some of the object sizes are wonky and could need a fix. This may be due to timing, or how CSS is generated (or maybe not). In any case it works well enough as a proof of concept, though it needs (a lot) more work.

If you want to use or modify this code for your own projects, you're free to do so per MIT license, so just go ahead!
