# Responsive Webdesign

## Responsive grid view

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <style>
            * {box-sizing: border-box;}

            .row::after {   content: "";
                            clear: both;
                            display: table;}

            [class*="col-"] {   float: left;
                                padding: 15px;}

            .col-1 {width: 8.33%;}
            .col-2 {width: 16.66%;}
            .col-3 {width: 25%;}
            .col-4 {width: 33.33%;}
            .col-5 {width: 41.66%;}
            .col-6 {width: 50%;}
            .col-7 {width: 58.33%;}
            .col-8 {width: 66.66%;}
            .col-9 {width: 75%;}
            .col-10 {width: 83.33%;}
            .col-11 {width: 91.66%;}
            .col-12 {width: 100%;}

            html {font-family: "Lucida Sans", sans-serif;}

            .header {   background-color: #9933cc;
                        color: #ffffff;
                        padding: 15px;}

            .menu ul {  list-style-type: none;
                        margin: 0;
                        padding: 0;}

            .menu li {  padding: 8px;
                        margin-bottom: 7px;
                        background-color: #33b5e5;
                        color: #ffffff;
                        box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);}

            .menu li:hover {background-color: #0099cc;}
        </style>
    </head>
    <body>
        <div class="header">
            <h1>Chania</h1>
        </div>

        <div class="row">
            <div class="col-3 menu">
                <ul>
                    <li>The Flight</li>
                    <li>The City</li>
                    <li>The Island</li>
                    <li>The Food</li>
                </ul>
            </div>

            <div class="col-9">
                <h1>The City</h1>
                <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two parts, the old town and the modern city.</p>
                <p>Resize the browser window to see how the content respond to the resizing.</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Responsive_Webdesign/Example_1.html)

## Add breakpoints for desktops, laptops and phones

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <style>
            * {box-sizing: border-box;}

            .row::after {   content: "";
                            clear: both;
                            display: table;}

            [class*="col-"] {   float: left;
                                padding: 15px;}

            html {font-family: "Lucida Sans", sans-serif;}

            .header {   background-color: #9933cc;
                        color: #ffffff;
                        padding: 15px;}

            .menu ul {  list-style-type: none;
                        margin: 0;
                        padding: 0;}

            .menu li {  padding: 8px;
                        margin-bottom: 7px;
                        background-color: #33b5e5;
                        color: #ffffff;
                        box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);}

            .menu li:hover {background-color: #0099cc;}

            .aside {background-color: #33b5e5;
                    padding: 15px;
                    color: #ffffff;
                    text-align: center;
                    font-size: 14px;
                    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);}

            .footer {   background-color: #0099cc;
                        color: #ffffff;
                        text-align: center;
                        font-size: 12px;
                        padding: 15px;}

            /* For mobile phones: */
            [class*="col-"] {width: 100%;}

            @media only screen and (min-width: 600px) { /* For tablets: */
                                                        .col-s-1 {width: 8.33%;}
                                                        .col-s-2 {width: 16.66%;}
                                                        .col-s-3 {width: 25%;}
                                                        .col-s-4 {width: 33.33%;}
                                                        .col-s-5 {width: 41.66%;}
                                                        .col-s-6 {width: 50%;}
                                                        .col-s-7 {width: 58.33%;}
                                                        .col-s-8 {width: 66.66%;}
                                                        .col-s-9 {width: 75%;}
                                                        .col-s-10 {width: 83.33%;}
                                                        .col-s-11 {width: 91.66%;}
                                                        .col-s-12 {width: 100%;}}

            @media only screen and (min-width: 768px) { /* For desktop: */
                                                        .col-1 {width: 8.33%;}
                                                        .col-2 {width: 16.66%;}
                                                        .col-3 {width: 25%;}
                                                        .col-4 {width: 33.33%;}
                                                        .col-5 {width: 41.66%;}
                                                        .col-6 {width: 50%;}
                                                        .col-7 {width: 58.33%;}
                                                        .col-8 {width: 66.66%;}
                                                        .col-9 {width: 75%;}
                                                        .col-10 {width: 83.33%;}
                                                        .col-11 {width: 91.66%;}
                                                        .col-12 {width: 100%;}}
        </style>
    </head>
    <body>
        <div class="header">
            <h1>Chania</h1>
        </div>

        <div class="row">
            <div class="col-3 col-s-3 menu">
                <ul>
                    <li>The Flight</li>
                    <li>The City</li>
                    <li>The Island</li>
                    <li>The Food</li>
                </ul>
            </div>

            <div class="col-6 col-s-9">
                <h1>The City</h1>
                <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two parts, the old town and the modern city.</p>
            </div>

            <div class="col-3 col-s-12">
                <div class="aside">
                    <h2>What?</h2>
                    <p>Chania is a city on the island of Crete.</p>
                    <h2>Where?</h2>
                    <p>Crete is a Greek island in the Mediterranean Sea.</p>
                    <h2>How?</h2>
                    <p>You can reach Chania airport from all over Europe.</p>
                </div>
            </div>
        </div>

        <div class="footer">
            <p>Resize the browser window to see how the content respond to the resizing.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Responsive_Webdesign/Example_2.html)

## Typical breakpoints

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <style>
            .example {  padding: 20px;
                        color: white;}

            /* Extra small devices (phones, 600px and down) */
            @media only screen and (max-width: 600px) {.example {background: red;}}

            /* Small devices (portrait tablets and large phones, 600px and up) */
            @media only screen and (min-width: 600px) {.example {background: green;}}

            /* Medium devices (landscape tablets, 768px and up) */
            @media only screen and (min-width: 768px) {.example {background: blue;}} 

            /* Large devices (laptops/desktops, 992px and up) */
            @media only screen and (min-width: 992px) {.example {background: orange;}} 

            /* Extra large devices (large laptops and desktops, 1200px and up) */
            @media only screen and (min-width: 1200px) {.example {background: pink;}}
        </style>
    </head>
    <body>
        <h2>Typical Media Query Breakpoints</h2>
        <p class="example">Resize the browser window to see how the background color of this paragraph changes on different screen sizes.</p>
    </body>
</html>
```

Output:

[Click here!](./Responsive_Webdesign/Example_3.html)

## Responsive image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <style>
            img {   max-width: 100%;
                    height: auto;}
        </style>
    </head>
    <body>
        <img src="../data/images/img_chania.jpg" width="460" height="345">
        <p>Resize the browser window to see how the image will scale when the width is less than 460px.</p>
    </body>
</html>
```

Output:

[Click here!](./Responsive_Webdesign/Example_4.html)

## Responsive video

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <style>
            video { max-width: 100%;
                    height: auto;}
        </style>
    </head>
    <body>
        <video width="400" controls>
            <source src="../data/videos/mov_bbb.mp4" type="video/mp4">
            <source src="../data/videos/mov_bbb.ogg" type="video/ogg">
            Your browser does not support HTML5 video.
        </video>

        <p>Resize the browser window to see how the size of the video player will scale when the width is less than 400px.</p>
    </body>
</html>
```

Output:

[Click here!](./Responsive_Webdesign/Example_5.html)

## Responsive framework: W3.CSS

Code: 

```html
<!DOCTYPE html>
<html>
    <title>W3.CSS</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
    <body>
        <div class="w3-container w3-blue">
            <h1>W3Schools Demo</h1> 
            <p>Resize this responsive page!</p> 
        </div>

        <div class="w3-row-padding">
            <div class="w3-third">
                <h2>London</h2>
                <p>London is the capital city of England.</p>
                <p>It is the most populous city in the United Kingdom,
                with a metropolitan area of over 13 million inhabitants.</p>
            </div>

            <div class="w3-third">
                <h2>Paris</h2>
                <p>Paris is the capital of France.</p> 
                <p>The Paris area is one of the largest population centers in Europe,
                with more than 12 million inhabitants.</p>
            </div>

            <div class="w3-third">
                <h2>Tokyo</h2>
                <p>Tokyo is the capital of Japan.</p>
                <p>It is the center of the Greater Tokyo Area,
                and the most populous metropolitan area in the world.</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Responsive_Webdesign/Example_6.html)

## Responsive framework: Bootstrap

Code: 

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Bootstrap 5 Example</title>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet">
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"></script>
    </head>
    <body>
        <div class="container-fluid p-5 bg-primary text-white text-center">
            <h1>My First Bootstrap Page</h1>
            <p>Resize this responsive page to see the effect!</p> 
        </div>
        
        <div class="container mt-5">
            <div class="row">
                <div class="col-sm-4">
                    <h3>Column 1</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit...</p>
                    <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris...</p>
                </div>
                <div class="col-sm-4">
                    <h3>Column 2</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit...</p>
                    <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris...</p>
                </div>
                <div class="col-sm-4">
                    <h3>Column 3</h3>        
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit...</p>
                    <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris...</p>
                </div>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Responsive_Webdesign/Example_7.html)