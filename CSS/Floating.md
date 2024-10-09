# Floating

## A simple use of the float property

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {float: right;}
        </style>
    </head>
    <body>
        <p>In the paragraph below, we have added an image with style <b>float:right</b>. The result is that the image will float to the right in the paragraph.</p>
        <p><img src="../data/images/w3css.gif" width="100" height="140">
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
        </p>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_1.html)

## An image with border and margins that floats to the right in a paragraph

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   float: right;
                    border: 1px dotted black;
                    margin: 0px 0px 15px 20px;}
        </style>
    </head>
    <body>
        <h2>Let an image float to the right in a paragraph</h2>

        <p>In the paragraph below, the image will float to the right. A dotted black border is added to the image. 
        We have also added margins to the image to push the text away from the image:
        0 px margin on the top and right side, 15 px margin on the bottom, and 20 px margin on the left side of the image.</p>

        <p><img src="../data/images/w3css.gif" width="100" height="140">
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
        </p>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_2.html)

## An image with a caption that floats to the right

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   float: right;
                    width: 120px;
                    margin: 0 0 15px 20px;
                    padding: 15px;
                    border: 1px solid black;
                    text-align: center;}
        </style>
    </head>
    <body>
        <h2>Let an image with a caption float to the right</h2>

        <p>In the paragraph below, the div element is 120 pixels wide and it contains the image. The div element will float to the right. Margins are added to the div to push the text away from the div. Borders and padding are added to the div to frame in the picture and the caption.</p>

        <div>
            <img src="../data/images/w3css.gif" width="100" height="140"><br>CSS is fun!
        </div>

        <p>
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
        </p>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_3.html)

## Let the first letter of a paragraph float to the left

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            span {  float: left;
                    width: 0.7em;
                    font-size: 400%;
                    font-family: algerian, courier;
                    line-height: 80%;}
        </style>
    </head>
    <body>
        <h2>Style the first letter of a paragraph and let it float left</h2>

        <p>
            <span>H</span>ere, the first letter of this text is embedded in a span element. The span element has a width that is 0.7 times the size of the current font. The font-size of the span element is 400% (quite large) and the line-height is 80%. The font of the letter in the span will be in "Algerian".
        </p>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_4.html)

## Turning off float (using the clear property)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .div1 { float: left;
                    width: 100px;
                    height: 50px;
                    margin: 10px;
                    border: 3px solid #73AD21;}

            .div2 {border: 1px solid red;}

            .div3 { float: left;
                    width: 100px;
                    height: 50px;
                    margin: 10px;
                    border: 3px solid #73AD21;}

            .div4 { border: 1px solid red;
                    clear: left;}
        </style>
    </head>
    <body>
        <h2>Without clear</h2>
        <div class="div1">div1</div>
        <div class="div2">div2 - Notice that the div2 element is after div1, in the HTML code. However, since div1 is floated to the left, this happens: the text in div2 is floated around div1, and div2 surrounds the whole thing.</div>

        <h2>Using clear</h2>
        <div class="div3">div3</div>
        <div class="div4">div4 - Using clear moves div4 down below the floated div3. The value "left" clears elements floated to the left. You can also clear "right" and "both".</div>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_5.html)

## Turning off float (using the "clearfix" hack)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 3px solid #4CAF50;
                    padding: 5px;}

            .img1 {float: right;}

            .img2 {float: right;}

            .clearfix::after {  content: "";
                                clear: both;
                                display: table;}
        </style>
    </head>
    <body>
        <h2>Without Clearfix</h2>

        <p>This image is floated to the right. It is also taller than the element containing it, so it overflows outside of its container:</p>

        <div>
            <img class="img1" src="../data/images/pineapple.jpg" alt="Pineapple" width="170" height="170">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...
        </div>

        <h2 style="clear:right">With New Modern Clearfix</h2>
        <p>Add the clearfix hack to the containing element, to fix this problem:</p>

        <div class="clearfix">
            <img class="img2" src="../data/images/pineapple.jpg" alt="Pineapple" width="170" height="170">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...
        </div>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_6.html)

## Create floating boxes

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            * {box-sizing: border-box;}

            .box {  float: left;
                    width: 33.33%;
                    padding: 50px;}

            .clearfix::after {  content: "";
                                clear: both;
                                display: table;}
        </style>
    </head>
    <body>
        <h2>Grid of Boxes</h2>
        <p>Float boxes side by side:</p>

        <div class="clearfix">
            <div class="box" style="background-color:#bbb">
                <p>Some text inside the box.</p>
            </div>
            <div class="box" style="background-color:#ccc">
                <p>Some text inside the box.</p>
            </div>
            <div class="box" style="background-color:#ddd">
                <p>Some text inside the box.</p>
            </div>
        </div>

        <p>
            <strong>Note:</strong> Here, we use the clearfix hack to take care of the layout flow. 
            We also use the box-sizing property to make sure that the box doesn't break due to extra padding. Try to remove this code to see the effect.
        </p>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_7.html)

## Create side-by-side images

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            * {box-sizing: border-box;}

            .img-container {float: left;
                            width: 33.33%;
                            padding: 5px;}

            .clearfix::after {  content: "";
                                clear: both;
                                display: table;}
        </style>
    </head>
    <body>
        <h2>Images Side by Side</h2>
        <p>Float images side by side:</p>

        <div class="clearfix">
            <div class="img-container">
                <img src="../data/images/img_5terre.jpg" alt="Italy" style="width:100%">
            </div>
            <div class="img-container">
                <img src="../data/images/img_forest.jpg" alt="Forest" style="width:100%">
            </div>
            <div class="img-container">
                <img src="../data/images/img_mountains.jpg" alt="Mountains" style="width:100%">
            </div>
        </div>

        <p>Note that we also use the clearfix hack to take care of the layout flow, and that we add the box-sizing property to make sure that the image container doesn't break due to extra padding. Try to remove this code to see the effect.</p>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_8.html)

## Create equal-height boxes (with flexbox)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .flex-container {   display: flex;
                                flex-wrap: nowrap;
                                background-color: DodgerBlue;}

            .flex-container .box {  background-color: #f1f1f1;
                                    width: 50%;
                                    margin: 10px;
                                    text-align: center;
                                    line-height: 75px;
                                    font-size: 30px;}
        </style>
    </head>
    <body>
        <h1>Flexible Boxes</h1>

        <div class="flex-container">
            <div class="box">Box 1 - This is some text to make sure that the content gets really tall. This is some text to make sure that the content gets really tall.</div>
            <div class="box">Box 2 - My height will follow Box 1.</div>
        </div>

        <p>Try to resize the browser window to see the flexible layout.</p>
        <p><strong>Note:</strong> Flexbox is not supported in Internet Explorer 10 or earlier versions.</p>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_9.html)

## Creating a horizontal menu

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ul {list-style-type: none;
                margin: 0;
                padding: 0;
                overflow: hidden;
                background-color: #333;}

            li {float: left;}

            li a {  display: inline-block;
                    color: white;
                    text-align: center;
                    padding: 14px 16px;
                    text-decoration: none;}

            li a:hover {background-color: #111;}

            .active {background-color: red;}
        </style>
    </head>
    <body>
        <ul>
            <li><a href="#home" class="active">Home</a></li>
            <li><a href="#news">News</a></li>
            <li><a href="#contact">Contact</a></li>
            <li><a href="#about">About</a></li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_10.html)

## Create a web layout example

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            * {box-sizing: border-box;}
            
            body {background-color: white;}

            .header, .footer {  background-color: grey;
                                color: white;
                                padding: 15px;}

            .column {   float: left;
                        padding: 15px;}

            .clearfix::after {  content: "";
                                clear: both;
                                display: table;}

            .menu {width: 25%;}

            .content {width: 75%;}

            .menu ul {  list-style-type: none;
                        margin: 0;
                        padding: 0;}

            .menu li {  padding: 8px;
                        margin-bottom: 8px;
                        background-color: #33b5e5;
                        color: #ffffff;}

            .menu li:hover {background-color: #0099cc;}
        </style>
    </head>
    <body>
        <div class="header">
            <h1>Chania</h1>
        </div>

        <div class="clearfix">
            <div class="column menu">
                <ul>
                    <li>The Flight</li>
                    <li>The City</li>
                    <li>The Island</li>
                    <li>The Food</li>
                </ul>
            </div>

            <div class="column content">
                <h1>The City</h1>
                <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two parts, the old town and the modern city.</p>
                <p>You will learn more about web layout and responsive web pages in a later chapter.</p>
            </div>
        </div>

        <div class="footer">
            <p>Footer Text</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Floating/Example_11.html)