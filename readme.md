[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/owner/my-element)
# TypeWriter:

### What is it?
type-writer is a text effect web component (block element). Whatever you put in the innerText will look like
its being type out. There are four types of cursors that can be set and two types of typing effects.  You can set 
the font-size but at the moment it only uses the Source Code Pro font but in the future I will add support
whatever font a user would like to use.

![Alt text](https://github.com/mmgrant73/revealbox/blob/master/typewriter.png?raw=true "Image-TypeWriter")

[Click here for Demo](https://mmgrant73.github.io/revealbox/typewriter.html) 

### How to use it?
It is quite easy to use it on your webpage. Just follow the below steps:

1. Include the link to the script file that holds the this custom web component (reveal-box.js) near the bottom of 
   the body section of your webpage.  See below
   
```
    <script src="./typewriter.js"></script>
```

2.  Then use the custom element tags on your webpage.

```
    <type-writer cursor="underline" effect="standard" align="left" fontsize="28px">
        This is a typewriter effect
    </type-writer>
```

Note: That is all you have to do to use this custom element.  There is an example HTML page (acronym.html) that shows how to use it.

```
    <!DOCTYPE html>
    <html>
      <head>
        <title>Typewriter Web Component</title>
        <style>
       
            body {
                padding: 40px;
                background-color: #121212;
                color: white;
            }
            
        </style>
      </head>
      
      <body>
      
        <h1 style="padding: 10px, 0px, 0px, 25px; margin: 20px">Typewriter web component:</h1>

        <type-writer cursor="underline" effect="standard" align="left" fontsize="28px">
            This is a test.
        </type-writer>

        <script src="./typewriter.js"></script>

      </body>
      
    </html>
```

### There are only four properties that you can use to customize this element.

There are four attributes that you need to set:
1. cursor - the type of cursor that will be used for the typing effect
2. effect - the type of typing effect that will be used
3. align - is used to set how the text will be aligned in the DIV tag
4. fontsize - The font-size that the text will take

Note: The inner text within the type-writer tag will be the text used for the typing effect

### Type of Cursor (There are four types):
1. line
2. underline
3. block
4. none

### Type of effect (There are two):
1. standard - the cursor would jump in steps to make it look like the text is being typed
2. smooth - the cursor would travel smoothly across the screen without jumping.

### Types of aligment:
1. left
2. right
3. center

### To Do:
1. Add support for more fonts families

Note: The default attributes are (cursor: line, effect: standard. align: left and font-size: 28px)
