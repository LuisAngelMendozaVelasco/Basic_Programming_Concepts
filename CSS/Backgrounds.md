# Backgrounds

## Set the background color of a page

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {background-color: lightblue;}
        </style>
    </head>
    <body>
        <h1>Hello World!</h1>

        <p>This page has a light blue background color!</p>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_1.html)

## Set the background color of different elements

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {background-color: green;}
            div {background-color: lightblue;}
            p {background-color: yellow;}
        </style>
    </head>
    <body>
        <h1>CSS background-color example!</h1>
        <div>
            This is a text inside a div element.
            <p>This paragraph has its own background color.</p>
            We are still in the div element.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_2.html)

## Set an image as the background of a page

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {background-image: url("../data/images/paper.gif");}
        </style>
    </head>
    <body>
        <h1>Hello World!</h1>

        <p>This page has an image as the background!</p>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_3.html)

## How to repeat a background image only horizontally

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {  background-image: url("../data/images/gradient_bg.png");
                    background-repeat: repeat-x;}
        </style>
    </head>
    <body>
        <h1>Hello World!</h1>
        <p>Here, a background image is repeated only horizontally!</p>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_4.html)

## How to position a background image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {  background-image: url("../data/images/img_tree.png");
                    background-repeat: no-repeat;
                    background-position: right top;
                    margin-right: 200px;}
        </style>
    </head>
    <body>
        <h1>Hello World!</h1>
        <p>Here, the background image is only shown once. In addition it is positioned away from the text.</p>
        <p>In this example we have also added a margin on the right side, so that the background image will not disturb the text.</p>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_5.html)

## A fixed background image (this image will not scroll with the rest of the page)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {  background-image: url("../data/images/img_tree.png");
                    background-repeat: no-repeat;
                    background-position: right top;
                    margin-right: 200px;
                    background-attachment: fixed;}
        </style>
    </head>
    <body>
        <h1>The background-attachment Property</h1>

        <p>The background-attachment property specifies whether the background image should scroll or be fixed (will not scroll with the rest of the page).</p>

        <p><strong>Tip:</strong> If you do not see any scrollbars, try to resize the browser window.</p>

        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
        <p>The background-image is fixed. Try to scroll down the page.</p>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_6.html)

## All the background properties in one declaration

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {  background: #ffffff url("../data/images/img_tree.png") no-repeat right top;
                    margin-right: 200px;}
        </style>
    </head>
    <body>
        <h1>The background Property</h1>

        <p>The background property is a shorthand property for specifying all the background properties in one declaration.</p>

        <p>Here, the background image is only shown once, and it is also positioned in the top-right corner.</p>

        <p>We have also added a right margin, so that the text will not write over the background image.</p>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_7.html)

## Advanced background example

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {  margin-left: 200px;
                    background: #5d9ab2 url("../data/images/img_tree.png") no-repeat top left;}

            .center_div {   border: 1px solid gray;
                            margin-left: auto;
                            margin-right: auto;
                            width: 90%;
                            background-color: #d0f0f6;
                            text-align: left;
                            padding: 8px;}
        </style>
    </head>
    <body>
        <div class="center_div">
            <h1>Hello World!</h1>
            <p>This example contains some advanced CSS methods you may not have learned yet. But, we will explain these methods in a later chapter in the tutorial.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_8.html)

## Add multiple background images for an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            #example1 { background-image: url(../data/images/img_flwr.gif), url(../data/images/paper.gif);
                        background-position: right bottom, left top;
                        background-repeat: no-repeat, repeat;
                        padding: 15px;}
        </style>
    </head>
    <body>
        <h1>Multiple Backgrounds</h1>
        <p>The following div element has two background images:</p>

        <div id="example1">
            <h1>Lorem Ipsum Dolor</h1>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
            <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_9.html)

## Specify the size of a background image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #example1 { border: 1px solid black;
                        background: url(../data/images/img_flwr.gif);
                        background-size: 100px 80px;
                        background-repeat: no-repeat;
                        padding: 15px;}

            #example2 { border: 1px solid black;
                        background: url(../data/images/img_flwr.gif);
                        background-repeat: no-repeat;
                        padding: 15px;}
        </style>
    </head>
    <body>
        <h1>The background-size Property</h1>

        <p>Resized background-image:</p>
        <div id="example1">
            <h2>Lorem Ipsum Dolor</h2>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
            <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
        </div>

        <p>Original size of the background-image:</p>
        <div id="example2">
            <h2>Lorem Ipsum Dolor</h2>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
            <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_10.html)

## Scale a background image using "contain" and "cover"

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .div1 { border: 1px solid black;
                    height: 120px;
                    width: 150px;
                    background: url(../data/images/img_flwr.gif);
                    background-repeat: no-repeat;
                    background-size: contain;}

            .div2 { border: 1px solid black;
                    height: 120px;
                    width: 150px;
                    background: url(../data/images/img_flwr.gif);
                    background-repeat: no-repeat;
                    background-size: cover;}

            .div3 { border: 1px solid black;
                    height: 120px;
                    width: 150px;
                    background: url(../data/images/img_flwr.gif);
                    background-repeat: no-repeat;}
        </style>
    </head>
    <body>
        <h1>The background-size Property</h1>

        <h2>background-size: contain:</h2>
        <div class="div1">
            <p>Lorem ipsum dolor sit amet.</p>
        </div>

        <h2>background-size: cover:</h2>
        <div class="div2">
            <p>Lorem ipsum dolor sit amet.</p>
        </div>

        <h2>No background-size defined:</h2>
        <div class="div3">
            <p>Lorem ipsum dolor sit amet.</p>
        </div>

        <p>Original image:</p>
        <img src="../data/images/img_flwr.gif" alt="Flowers" width="224" height="162">
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_11.html)

## Define sizes of multiple background images

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            #example1 { background: url(../data/images/img_tree.gif) left top no-repeat, url(../data/images/img_flwr.gif) right bottom no-repeat, url(../data/images/paper.gif) left top repeat;
                        padding: 15px;
                        background-size: 50px, 130px, auto;}
        </style>
    </head>
    <body>
        <div id="example1">
            <h1>Lorem Ipsum Dolor</h1>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
            <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_12.html)

## Full-size background image (completely fill the content area)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            html {  background: url(../data/images/img_man.jpg) no-repeat center fixed; 
                    background-size: cover;}

            body {color: white;}
        </style>
    </head>
    <body>
        <h1>Full Page Background Image</h1>
        <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_13.html)

## Use background-origin to specify where the background image is positioned

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #example1 { border: 10px solid black;
                        padding: 35px;
                        background: url(../data/images/img_flwr.gif);
                        background-repeat: no-repeat;}

            #example2 { border: 10px solid black;
                        padding: 35px;
                        background: url(../data/images/img_flwr.gif);
                        background-repeat: no-repeat;
                        background-origin: border-box;}

            #example3 { border: 10px solid black;
                        padding: 35px;
                        background: url(../data/images/img_flwr.gif);
                        background-repeat: no-repeat;
                        background-origin: content-box;}
        </style>
    </head>
    <body>
        <h1>The background-origin Property</h1>

        <p>No background-origin (padding-box is default):</p>
        <div id="example1">
            <h2>Lorem Ipsum Dolor</h2>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
            <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
        </div>

        <p>background-origin: border-box:</p>
        <div id="example2">
            <h2>Lorem Ipsum Dolor</h2>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
            <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
        </div>

        <p>background-origin: content-box:</p>
        <div id="example3">
            <h2>Lorem Ipsum Dolor</h2>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
            <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_14.html)

## Use background-clip to specify the painting area of the background

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #example1 { border: 10px dotted black;
                        padding: 35px;
                        background: yellow;}

            #example2 { border: 10px dotted black;
                        padding: 35px;
                        background: yellow;
                        background-clip: padding-box;}

            #example3 { border: 10px dotted black;
                        padding: 35px;
                        background: yellow;
                        background-clip: content-box;}
        </style>
    </head>
    <body>
        <h1>The background-clip Property</h1>

        <p>No background-clip (border-box is default):</p>
        <div id="example1">
            <h2>Lorem Ipsum Dolor</h2>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
        </div>

        <p>background-clip: padding-box:</p>
        <div id="example2">
            <h2>Lorem Ipsum Dolor</h2>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
        </div>

        <p>background-clip: content-box:</p>
        <div id="example3">
            <h2>Lorem Ipsum Dolor</h2>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Backgrounds/Example_15.html)