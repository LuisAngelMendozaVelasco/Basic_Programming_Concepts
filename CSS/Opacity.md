# Opacity

## Creating transparent images

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {opacity: 0.5;}
        </style>
    </head>
    <body>
        <h1>Image Transparency</h1>
        <p>The opacity property specifies the transparency of an element. The lower the value, the more transparent:</p>

        <p>Image with 50% opacity:</p>
        <img src="../data/images/img_forest.jpg" alt="Forest" width="170" height="100">
    </body>
</html>
```

Output:

[Click here!](./Opacity/Example_1.html)

## Creating transparent images - mouseover effect

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {opacity: 0.5;}
            img:hover {opacity: 1.0;}
        </style>
    </head>
    <body>
        <h1>Image Transparency</h1>
        <p>The opacity property is often used together with the :hover selector to change the opacity on mouse-over:</p>
        <img src="../data/images/img_forest.jpg" alt="Forest" width="170" height="100">
        <img src="../data/images/img_mountains.jpg" alt="Mountains" width="170" height="100">
        <img src="../data/images/img_5terre.jpg" alt="Italy" width="170" height="100">
    </body>
</html>
```

Output:

[Click here!](./Opacity/Example_2.html)

## Reversed mouseover effect for transparent images

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img:hover {opacity: 0.5;}
        </style>
    </head>
    <body>
        <h1>Image Transparency</h1>
        <p>The opacity property is often used together with the :hover selector to change the opacity on mouse-over:</p>
        <img src="../data/images/img_forest.jpg" alt="Forest" width="170" height="100">
        <img src="../data/images/img_mountains.jpg" alt="Mountains" width="170" height="100">
        <img src="../data/images/img_5terre.jpg" alt="Italy" width="170" height="100">
    </body>
</html>
```

Output:

[Click here!](./Opacity/Example_3.html)

## Transparent box/div

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   background-color: #4CAF50;
                    padding: 10px;}

            div.first {opacity: 0.1;}

            div.second {opacity: 0.3;}

            div.third {opacity: 0.6; }
        </style>
    </head>
    <body>
        <h1>Transparent Box</h1>
        <p>When using the opacity property to add transparency to the background of an element, all of its child elements become transparent as well. This can make the text inside a fully transparent element hard to read:</p>

        <div class="first"><p>opacity 0.1</p></div>
        <div class="second"><p>opacity 0.3</p></div>
        <div class="third"><p>opacity 0.6</p></div>
        <div><p>opacity 1 (default)</p></div>
    </body>
</html>
```

Output:

[Click here!](./Opacity/Example_4.html)

## Transparent box/div with RGBA values

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   background: rgb(76, 175, 80);
                    padding: 10px;}

            div.first {background: rgba(76, 175, 80, 0.1);}

            div.second {background: rgba(76, 175, 80, 0.3);}

            div.third {background: rgba(76, 175, 80, 0.6);}
        </style>
    </head>
    <body>
        <h1>Transparent Box</h1>
        <p>With opacity:</p>
        <div style="opacity:0.1;"><p>10% opacity</p></div>
        <div style="opacity:0.3;"><p>30% opacity</p></div>
        <div style="opacity:0.6;"><p>60% opacity</p></div>
        <div><p>opacity 1</p></div>

        <p>With RGBA color values:</p>
        <div class="first"><p>10% opacity</p></div>
        <div class="second"><p>30% opacity</p></div>
        <div class="third"><p>60% opacity</p></div>
        <div><p>default</p></div>

        <p>Notice how the text gets transparent as well as the background color when using the opacity property.</p>
    </body>
</html>
```

Output:

[Click here!](./Opacity/Example_5.html)

## Creating a transparent box with text on a background image

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div.background {background: url(../data/images/klematis.jpg) repeat;
                            border: 2px solid black;}

            div.transbox {  margin: 30px;
                            background-color: #ffffff;
                            border: 1px solid black;
                            opacity: 0.6;}

            div.transbox p {margin: 5%;
                            font-weight: bold;
                            color: #000000;}
        </style>
    </head>
    <body>
        <div class="background">
            <div class="transbox">
                <p>This is some text that is placed in the transparent box.</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Opacity/Example_6.html)