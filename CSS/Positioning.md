# Positioning

## Position an element relative to the browser window

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div.fixed { position: fixed;
                        bottom: 0;
                        right: 0;
                        width: 300px;
                        border: 3px solid #73AD21;}
        </style>
    </head>
    <body>
        <h2>position: fixed;</h2>

        <p>An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled:</p>

        <div class="fixed">
            This div element has position: fixed;
        </div>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_1.html)

## Position an element relative to its normal position

Code:

```html
<!--------------------------------------------------------->
<!-- Position an element relative to its normal position -->
<!--------------------------------------------------------->

<!DOCTYPE html>
<html>
    <head>
        <style>
            div.relative {  position: relative;
                            left: 30px;
                            border: 3px solid #73AD21;}
        </style>
    </head>
    <body>
        <h2>position: relative;</h2>

        <p>An element with position: relative; is positioned relative to its normal position:</p>

        <div class="relative">
            This div element has position: relative;
        </div>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_2.html)

## Position an element with an absolute value

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div.relative {  position: relative;
                            width: 400px;
                            height: 200px;
                            border: 3px solid #73AD21;} 

            div.absolute {  position: absolute;
                            top: 80px;
                            right: 0;
                            width: 200px;
                            height: 100px;
                            border: 3px solid #73AD21;}
        </style>
    </head>
    <body>
        <h2>position: absolute;</h2>

        <p>An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed):</p>

        <div class="relative">This div element has position: relative;
            <div class="absolute">This div element has position: absolute;</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_3.html)

## Sticky positioning

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div.sticky {position: -webkit-sticky;
                        position: sticky;
                        top: 0;
                        padding: 5px;
                        background-color: #cae8ca;
                        border: 2px solid #4CAF50;}
        </style>
    </head>
    <body>
        <p>Try to <b>scroll</b> inside this frame to understand how sticky positioning works.</p>

        <div class="sticky">I am sticky!</div>

        <div style="padding-bottom:2000px">
            <p>In this example, the sticky element sticks to the top of the page (top: 0), when you reach its scroll position.</p>
            <p>Scroll back up to remove the stickyness.</p>
            <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
            <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_4.html)

## Overlapping elements

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   position: absolute;
                    left: 0px;
                    top: 0px;
                    z-index: -1;}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <img src="../data/images/img_tree.png">
        <p>Because the image has a z-index of -1, it will be placed behind the text.</p>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_5.html)

## Set the shape of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   position: absolute;
                    clip: rect(0px, 60px, 200px, 0px);}
        </style>
    </head>
    <body>
        <img src="../data/images/w3css.gif" width="100" height="140">
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_6.html)

## Set the top edge of an image using a pixel value

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   position: absolute;
                    top: 0px;}
        </style>
    </head>
    <body>
        <img src="../data/images/smiley.gif" width="42" height="42">
        <h1>This is a heading</h1>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_7.html)

## Set the bottom edge of an image using a pixel value

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img.ex1 {   position: absolute;
                        bottom: 0px;}

            img.ex2 {   position: relative;
                        bottom: -100px;}
        </style>
    </head>
    <body>
        <img class="ex1" src="../data/images/smiley.gif" width="42" height="42">
        <h1>This is a heading</h1>
        <img class="ex2" src="../data/images/smiley.gif" width="42" height="42">
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_8.html)

## Set the left edge of an image using a pixel value

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   position: absolute;
                    left: 50px;}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <img src="../data/images/smiley.gif" width="42" height="42">
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_9.html)

## Set the right edge of an image using a pixel value

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   position: absolute;
                    right: 50px;}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <img src="../data/images/smiley.gif" width="42" height="42">
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_10.html)

## Position image text (top left corner)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .topleft {  position: absolute;
                        top: 8px;
                        left: 16px;
                        font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>
        <p>Add some text to an image in the top left corner:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="topleft">Top Left</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_11.html)

## Position image text (top right corner)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .topright { position: absolute;
                        top: 8px;
                        right: 16px;
                        font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>
        <p>Add some text to an image in the top right corner:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="topright">Top Right</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_12.html)

## Position image text (bottom left corner)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .bottomleft {   position: absolute;
                            bottom: 8px;
                            left: 16px;
                            font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>
        <p>Add some text to an image in the bottom left corner:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="bottomleft">Bottom Left</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_13.html)

## Position image text (bottom right corner)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .bottomright {  position: absolute;
                            bottom: 8px;
                            right: 16px;
                            font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>
        <p>Add some text to an image in the bottom right corner:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="bottomright">Bottom Right</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_14.html)

## Position image text (centered)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .center {   position: absolute;
                        top: 50%;
                        width: 100%;
                        text-align: center;
                        font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>

        <p>Center text in image:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="center">Centered</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Positioning/Example_15.html)