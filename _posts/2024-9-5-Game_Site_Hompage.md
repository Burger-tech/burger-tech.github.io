---
title: The Homepage For Our Game Site
date: 2024-9-5
categories: [Projects, Game Site]
tags: [gaming,website,gamesite]
toc: true
---

![pic of bergsmaservers homepage](https://i.ibb.co/JjkfHdF/Screenshot-2024-09-05-074738.png)
<br>The Homepage we will make by The end of The Tutorial


# The Code

So, we know what we will make, now how do we actually make it? 

```html
<head>
<link rel="stylesheet" href="css/styles.css">
</head>

<body>

<h2>
<div>
<ul>

<li><a href="index.html">Home</a></li>
<li><a href="Help.html">Help</a></li>
<li><a href="../Games.html">Games</a></li>


</ul>
</div>
</h2>


<p6>
An exclamation mark means the game isn't working!
</p6>
  
<p5>
<br>
<br>
<br>
<div>
<l>

<li><a href="Games/kourio.html">Kour.io</a></li>
<li><a href="Games/1v1lol.html">1v1.lol</a></li>
<li><a href="Games/slowroads.html">Slowroads.io</a></li> 
<li><a href="Games/diep.html">diep.io</a></li>
<li><a href="Games/shellshockers.html">shellshock.io</a></li>
<li><a href="Games/slither.html">slither.io</a></li>
<li><a href="Games/zombsroyale.html">zombsroyale.io</a></li>
<li><a href="Games/1v1school.html">1v1.school</a></li>
<li><a href="Games/lordzio.html">lordz.io</a></li>
<li><a href="Games/krunkerio.html">krunker.io</a></li>
<li><a href="Games/digdigio.html">digdig.io</a></li>
<li><a href="Games/voxiomio.html">voxiom.io</a></li>
<li><a href="Games/aquaparkio.html">aquapark.io</a></li>
<li><a href="Games/evowarsio.html">evowars.io</a></li>

</l>
</div>
</p5>
</body>
```


## So, what did all of that mean?

If you read my last tutorial on how to make a page with pur game imbeded in it, this code will undoubtedly look much simpler. The reason for this is the lack of iframes, java, and identifiers. These parts of the code are generaly the things that make the website more functional, but for this Game Homepage, we don't need that, as all it is displaying are liks to the game.

From the top, the first thing we see is the stylesheet link that is on all of the Game Site html files. The only thing this does is link our css (cascading style sheet) to our html code. You can also code the css directly in the html page if you want, but having a css sheet and linking it is generally better practice.

The next thing that we see is a div with the links to all of our pages in it. This functions as the website's navigation bar, so that we can get to all of the different pages on our site. Inside the div, we see links to all of the other html pages on our site.


After this, we see this huge block of links:
```html
<l>

<li><a href="Games/kourio.html">Kour.io</a></li>
<li><a href="Games/1v1lol.html">1v1.lol</a></li>
<li><a href="Games/slowroads.html">Slowroads.io</a></li> 
<li><a href="Games/diep.html">diep.io</a></li>
<li><a href="Games/shellshockers.html">shellshock.io</a></li>
<li><a href="Games/slither.html">slither.io</a></li>
<li><a href="Games/zombsroyale.html">zombsroyale.io</a></li>
<li><a href="Games/1v1school.html">1v1.school</a></li>
<li><a href="Games/lordzio.html">lordz.io</a></li>
<li><a href="Games/krunkerio.html">krunker.io</a></li>
<li><a href="Games/digdigio.html">digdig.io</a></li>
<li><a href="Games/voxiomio.html">voxiom.io</a></li>
<li><a href="Games/aquaparkio.html">aquapark.io</a></li>
<li><a href="Games/evowarsio.html">evowars.io</a></li>

</l>
```

As you can see, the code for these is very repetative. This is because the links are all basically the same. The link goes to one of our game pages on our website, and has text to tell the user what the game is. These are all inside of an "L" tag, which means they are in a bulleted list.

# That's Pretty Much It

This was by far one of the more simple tutorials on this site. If you also read the other tutorials on making a fully functional Game Site, then you're basically done! As always, thanks so much for reading this, and come back again some other time!
