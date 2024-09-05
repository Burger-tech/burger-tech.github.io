---
title: A Game Website Page With A Java Fullscreen button
date: 2024-9-4
categories: [Projects, Game Site]
tags: [gaming,website,gamesite]
toc: false
---





![pic of bergsmaservers game page](https://i.ibb.co/tKVM8qs/Screenshot-2024-09-04-203823.png)
<br>The Page You Will Make




# How To Code It!

This guide is the first one in a series of many on how to to make a fully functuional games website with CSS & HTML!

In this guide, you will learn:
* How to code a navigation bar to go to the various pages of your site
* How to code an iframe for your game
* How to make a fullscreen button for your game with java


## The Code

The actual code to be able to write this (I'm pulling some of these references from other files on my website - bergsmaservers.win)

```html

<head>
<link rel="stylesheet" href="../css/styles.css">
</head>


<b>
<h2>
<div>
<ul>

<li><a href="../index.html">Home</a></li>
<li><a href="../Help.html">Help</a></li>
<li><a href="../Games.html">Games</a></li>


</ul>
</div>
</h2>


  <button id= "togglebutton" onclick="goFullscreen('iframe'); return false">Fullscreen</button>
 
<script>
function goFullscreen(id) {
    var element = document.getElementById(id);
    if (element.mozRequestFullScreen) {
      element.mozRequestFullScreen();
    } else if (element.webkitRequestFullScreen) {
      element.webkitRequestFullScreen();
    }
}
</script>


<h5>
1v1.lol
</h5>
<iframe id= "iframe" src="<game_site>" width="1000" height="600" allowfullscreen > </iframe>
  
</b>

```

## That Was A Lot....

If you're kinda confused right now, you are human. Lets start explaining this from the top! 


First, we see the link for the css stylesheet, which is holding all of the fonts and styles that make our website look the way it does. When it mentions the folder structer where the file is located, it also has those 3 little dots, which means that it is located in the parent directory (the one above) of the directory we are in right now (/Games). We have to go to the parent directory to access the folder in which our css file is (/css).


Next, we see a div, which in html is a banner that stretches across the length of the page. Inside of this div is an unordered list, or ul. this means that our links to the other pages of our website are listed without bullet points or numbers, and the div means they will be going horizontally. This creates a nice bar at the top of our game's page from which we can get to the other pages on the website. Mine has the home page, the games page (the page that has all of the game pages listed on it), and the help page, but you can put any link or local html file on yours.


The next part that we see  going down may look confusing at first, but is actually ridiculously simple. You see, this is the code that makes the fullscreen toggle button above our game. The "button id" code is whats giving out button an identifier, namely togglebutton. After that, we see 

```html
onclick="goFullscreen('iframe'); return false"
````

This is the part of the button that is actually java. All it is saying is that when the button is clicked, it will trigger the function "goFullscreen" on iframe, which is the identifier of our iframe with the game in it. After this, we see "return: false", which means that the script will not tell us anything after executing.


This part is likely going to be the most challenging if you're just trying to learn html, but stick with me:

```html
<script>
function goFullscreen(id) {
    var element = document.getElementById(id);
    if (element.mozRequestFullScreen) {
      element.mozRequestFullScreen();
    } else if (element.webkitRequestFullScreen) {
      element.webkitRequestFullScreen();
    }
}
</script>
```

This part of the code is actually java, kind of like the codw we just went over, but this is just a million times longer (or at least it feels that way!). At the top of this, we see the html tag script, which means we are telling it that anything in this tag is javascript (unless another code language is specified). Next, we see the function id of goFullscreen. Remember that? Well, it was the function that we called to happen when you click the fullscreen button above. All of the following code is just different lines that are there so that every major browser framework will know to make the iframe fullscreen.



The only thing that we still have to go over is arguably the most fundamental part - the iframe. The iframe is what is actually displaying out game. It is calling a url, and displaying the contents of that page in a box. To change the outline, color, and shape of an iframe, you can change the css for that iframe tag. The only technical parts of this are the src properity, which is where you put the desired url, and the heith and width, which specifies how large the iframe will be. You can also ad an id, as we have done here, so that our fullscreen button makes this iframe fullscreen when clicked. You also have to have "allowfullscreen", so that it can be fullscreen.


 
## Well, there ya go!

Thanks for reading my guide, and I hope you learned a lot and come back to read the rest of the gamesite series. If you want to read more, you can look on this site for documents with the tag "gamesite". See you next time!!
