# Flexbox

## Flexbox with three flex items

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_1.html)

## Flexbox with three flex items - rtl direction

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {direction: rtl;}

            .flex-container {   display: -webkit-flex;
                                display: flex;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_2.html)

## flex-direction - row-reverse

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-flex-direction: row-reverse;
                                flex-direction: row-reverse;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_3.html)

## flex-direction - column

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-flex-direction: column;
                                flex-direction: column;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_4.html)

## flex-direction - column-reverse

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-flex-direction: column-reverse;
                                flex-direction: column-reverse;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_5.html)

## justify-content - flex-end

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-justify-content: flex-end;
                                justify-content: flex-end;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_6.html)

## justify-content - center

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-justify-content: center;
                                justify-content: center;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_7.html)

## justify-content - space-between

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-justify-content: space-between;
                                justify-content: space-between;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_8.html)

## justify-content - space-around

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-justify-content: space-around;
                                justify-content: space-around;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_9.html)

## align-items - stretch

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-align-items: stretch;
                                align-items: stretch;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_10.html)

## align-items - flex-start

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-align-items: flex-start;
                                align-items: flex-start;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_11.html)

## align-items - flex-end

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-align-items: flex-end;
                                align-items: flex-end;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_12.html)

## align-items - center

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-align-items: center;
                                align-items: center;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_13.html)

## align-items - baseline

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-align-items: baseline;
                                align-items: baseline;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_14.html)

## flex-wrap - nowrap

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-flex-wrap: nowrap;
                                flex-wrap: nowrap;
                                width: 300px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_15.html)

## flex-wrap - wrap

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-flex-wrap: wrap;
                                flex-wrap: wrap;
                                width: 300px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_16.html)

## flex-wrap - wrap-reverse

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-flex-wrap: wrap-reverse;
                                flex-wrap: wrap-reverse;
                                width: 300px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_17.html)

## align-content - center

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                -webkit-flex-wrap: wrap;
                                flex-wrap: wrap;
                                -webkit-align-content: center;
                                align-content: center;
                                width: 300px;
                                height: 300px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_18.html)

## Order the flex items

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 100px;
                        height: 100px;
                        margin: 10px;}

            .first {-webkit-order: -1;
                    order: -1;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item first">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_19.html)

## Margin-right:auto;

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 75px;
                        height: 75px;
                        margin: 10px;}

            .flex-item:first-child {margin-right: auto;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">flex item 1</div>
            <div class="flex-item">flex item 2</div>
            <div class="flex-item">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_20.html)

## Margin:auto; = perfect centering

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 75px;
                        height: 75px;
                        margin: auto;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item">Perfect centering!</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_21.html)

## align-self on flex items

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        width: 60px;
                        min-height: 100px;
                        margin: 10px;}

            .item1 {-webkit-align-self: flex-start;
                    align-self: flex-start;}

            .item2 {-webkit-align-self: flex-end;
                    align-self: flex-end;}

            .item3 {-webkit-align-self: center;
                    align-self: center;}

            .item4 {-webkit-align-self: baseline;
                    align-self: baseline;}

            .item5 {-webkit-align-self: stretch;
                    align-self: stretch;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item item1">flex-start</div>
            <div class="flex-item item2">flex-end</div>
            <div class="flex-item item3">center</div>
            <div class="flex-item item4">baseline</div>
            <div class="flex-item item5">stretch</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_22.html)

## Specify the length of the flex item, relative to the rest of the flex items

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .flex-container {   display: -webkit-flex;
                                display: flex;
                                width: 400px;
                                height: 250px;
                                background-color: lightgrey;}

            .flex-item {background-color: cornflowerblue;
                        margin: 10px;}

            .item1 {-webkit-flex: 2;
                    flex: 2;}

            .item2 {-webkit-flex: 1;
                    flex: 1;}

            .item3 {-webkit-flex: 1;
                    flex: 1;}
        </style>
    </head>
    <body>
        <div class="flex-container">
            <div class="flex-item item1">flex item 1</div>
            <div class="flex-item item2">flex item 2</div>
            <div class="flex-item item3">flex item 3</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_23.html)

## Create a responsive image gallery with flexbox

Code: 

```html
<!DOCTYPE html>
<html>
    <style>
        * { box-sizing: border-box;}

        body {  margin: 0;
                font-family: Arial;}

        .header {   text-align: center;
                    padding: 32px;}

        .row {  display: flex;
                flex-wrap: wrap;
                padding: 0 4px;}

        /* Create four equal columns that sits next to each other */
        .column {   flex: 25%;
                    max-width: 25%;
                    padding: 0 4px;}

        .column img {   margin-top: 8px;
                        vertical-align: middle;}

        /* Responsive layout - makes a two column-layout instead of four columns */
        @media (max-width: 800px) {.column {flex: 50%;
                                            max-width: 50%;}}

        /* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
        @media (max-width: 600px) {.column {flex: 100%;
                                            max-width: 100%;}}
    </style>
    <body>
        <!-- Header -->
        <div class="header">
            <h1>Responsive Image Gallery</h1>
            <p>Resize the browser window to see the responsive effect.</p>
        </div>

        <!-- Photo Grid -->
        <div class="row"> 
            <div class="column">
                <img src="../data/images/wedding.jpg" style="width:100%">
                <img src="../data/images/rocks.jpg" style="width:100%">
                <img src="../data/images/falls2.jpg" style="width:100%">
                <img src="../data/images/paris.jpg" style="width:100%">
                <img src="../data/images/nature.jpg" style="width:100%">
                <img src="../data/images/mist.jpg" style="width:100%">
                <img src="../data/images/paris.jpg" style="width:100%">
            </div>
            
            <div class="column">
                <img src="../data/images/underwater.jpg" style="width:100%">
                <img src="../data/images/ocean2.jpg" style="width:100%">
                <img src="../data/images/wedding.jpg" style="width:100%">
                <img src="../data/images/mountainskies.jpg" style="width:100%">
                <img src="../data/images/rocks.jpg" style="width:100%">
                <img src="../data/images/underwater.jpg" style="width:100%">
            </div> 
            
            <div class="column">
                <img src="../data/images/wedding.jpg" style="width:100%">
                <img src="../data/images/rocks.jpg" style="width:100%">
                <img src="../data/images/falls2.jpg" style="width:100%">
                <img src="../data/images/paris.jpg" style="width:100%">
                <img src="../data/images/nature.jpg" style="width:100%">
                <img src="../data/images/mist.jpg" style="width:100%">
                <img src="../data/images/paris.jpg" style="width:100%">
            </div>
            
            <div class="column">
                <img src="../data/images/underwater.jpg" style="width:100%">
                <img src="../data/images/ocean2.jpg" style="width:100%">
                <img src="../data/images/wedding.jpg" style="width:100%">
                <img src="../data/images/mountainskies.jpg" style="width:100%">
                <img src="../data/images/rocks.jpg" style="width:100%">
                <img src="../data/images/underwater.jpg" style="width:100%">
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_24.html)

## Create a responsive website with flexbox

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <style>
            * {box-sizing: border-box;}

            /* Style the body */
            body {  font-family: Arial;
                    margin: 0;}

            /* Header/logo Title */
            .header {   padding: 60px;
                        text-align: center;
                        background: #1abc9c;
                        color: white;}

            /* Style the top navigation bar */
            .navbar {   display: flex;
                        background-color: #333;}

            /* Style the navigation bar links */
            .navbar a { color: white;
                        padding: 14px 20px;
                        text-decoration: none;
                        text-align: center;}

            /* Change color on hover */
            .navbar a:hover {   background-color: #ddd;
                                color: black;}

            /* Column container */
            .row {  display: flex;
                    flex-wrap: wrap;}

            /* Create two unequal columns that sits next to each other */
            /* Sidebar/left column */
            .side { flex: 30%;
                    background-color: #f1f1f1;
                    padding: 20px;}

            /* Main column */
            .main { flex: 70%;
                    background-color: white;
                    padding: 20px;}

            /* Fake image, just for this example */
            .fakeimg {  background-color: #aaa;
                        width: 100%;
                        padding: 20px;}

            /* Footer */
            .footer {   padding: 20px;
                        text-align: center;
                        background: #ddd;}

            /* Responsive layout - when the screen is less than 700px wide, make the two columns stack on top of each other instead of next to each other */
            @media screen and (max-width: 700px) {.row, .navbar {flex-direction: column;}}
        </style>
    </head>
    <body>
        <!-- Note -->
        <div style="background:yellow;padding:5px">
            <h4 style="text-align:center">Resize the browser window to see the responsive effect.</h4>
        </div>

        <!-- Header -->
        <div class="header">
            <h1>My Website</h1>
            <p>With a <b>flexible</b> layout.</p>
        </div>

        <!-- Navigation Bar -->
        <div class="navbar">
            <a href="#">Link</a>
            <a href="#">Link</a>
            <a href="#">Link</a>
            <a href="#">Link</a>
        </div>

        <!-- The flexible grid (content) -->
        <div class="row">
            <div class="side">
                <h2>About Me</h2>
                <h5>Photo of me:</h5>
                <div class="fakeimg" style="height:200px;">Image</div>
                <p>Some text about me in culpa qui officia deserunt mollit anim..</p>
                <h3>More Text</h3>
                <p>Lorem ipsum dolor sit ame.</p>
                <div class="fakeimg" style="height:60px;">Image</div><br>
                <div class="fakeimg" style="height:60px;">Image</div><br>
                <div class="fakeimg" style="height:60px;">Image</div>
            </div>
            <div class="main">
                <h2>TITLE HEADING</h2>
                <h5>Title description, Dec 7, 2017</h5>
                <div class="fakeimg" style="height:200px;">Image</div>
                <p>Some text..</p>
                <p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
                <br>
                <h2>TITLE HEADING</h2>
                <h5>Title description, Sep 2, 2017</h5>
                <div class="fakeimg" style="height:200px;">Image</div>
                <p>Some text..</p>
                <p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
            </div>
        </div>

        <!-- Footer -->
        <div class="footer">
            <h2>Footer</h2>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Flexbox/Example_25.html)