# JSON-to-JS-Presentation
A small HTML5 app that takes JSON\* and makes a swooshy full screen presentation with it using arrow keys

\* It's really just an array of JS objects, but it looks JSON-y enough...

## What
In the `bin` folder you will find a file called `index.html`. If you look at the code, and know how to edit JSON/JavaScript objects, there should be enough in there to get you started for making a multimedia slide presentation, where the slides comes _swooshing_ towards you in 3D on the Z-axis. (OOoh, aaah, wow!) CSS transitions are really neat!

## Why
I just had to do this because MS PowerPoint made the sound lag on videos in the presentation. Can't have that when my pupils want their local equivalent of the Oscar's!

## How
I used mostly CSS3 transforms while manipulating HTML-element DOM objects with JavaScript to make it happen.

In order to use it, grab `index.html` and put it into its own folder, then make a directory called `media` next to the HTML-file. That's where you should put your images, videos and sound, and stuff. Then edit the HTML-file to put more JSON-slides into the `slides` array.

### Editing the HTML-file
The `slides[]` array contains each slide as a JavaScript object. 

The object has the following attributes:

`bg`, `category` and `html`.

The `bg` attribute is supposed to hold a background image. Whatever image you put there will be auto-sized to fit inside whatever screen size you're using. Depending on how you design your HTML, you can use this space either to showcase photographies or other artwork, or use it as a nice background for your HTML text.

The `category` corresponds to a few readymade CSS classes, bu you're free to make your own. The current classes are frontpage (the first slide), presentation (regular slide with bullet points), nominationPage (price nominees) and product (for showcasing the media products of the nominees). 

The `html` category holds simple HTML, meaning the content of each slide. This is also where you're supposed to put video and sound, you you've got it. As it is, videos are designed to swoosh in and auto-play in full screen without controls, thus only shorter films, or small pre-edited clips are advisable. In the finished "oscars" presentation for my school, I also had a slide containing just a background and some moody music for when the winner envelope was opened.

With the code done for the presentation and the slides, the real work is finding some content, and putting it together into a presentation with a nice dramatic curve.

## To Do
This is pretty dirty code, and there's still a lot of work to be done on this project. For instance the design really only works in full screen on a big computer monitor. :p For one, a way to make fonts scale in a polite manner is badly needed. Also some of the object sizes are wonky and could need a fix. This may be due to timing, or how CSS is generated (or maybe not). In any case it works well enough as a proof of concept, though it needs (a lot) more work.

If you want to use or modify this code for your own projects, you're free to do so per MIT license, so just go ahead!
