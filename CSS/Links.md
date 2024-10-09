# Links

## Add different colors to visited/unvisited links

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            /* unvisited link */
            a:link {color: red;}

            /* visited link */
            a:visited {color: green;}

            /* mouse over link */
            a:hover {color: hotpink;}

            /* selected link */
            a:active {color: blue;}
        </style>
    </head>
    <body>
        <h2>Styling a link depending on state</h2>

        <p><b><a href="https://www.w3schools.com/css/default.asp" target="_blank">This is a link</a></b></p>
        <p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be effective.</p>
        <p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>
    </body>
</html>
```

Output:

[Click here!](./Links/Example_1.html)

## Use of text-decoration on links

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a:link {text-decoration: none;}
            a:visited {text-decoration: none;}
            a:hover {text-decoration: underline;}
            a:active {text-decoration: underline;}
        </style>
    </head>
    <body>
        <h2>Styling a link with text-decoration property</h2>

        <p><b><a href="https://www.w3schools.com/css/default.asp" target="_blank">This is a link</a></b></p>
        <p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be effective.</p>
        <p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>
    </body>
</html>
```

Output:

[Click here!](./Links/Example_2.html)

## Specify a background color for links

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a:link {background-color: yellow;}
            a:visited {background-color: cyan;}
            a:hover {background-color: lightgreen;}
            a:active {background-color: hotpink;} 
        </style>
    </head>
    <body>
        <h2>Styling a link with background-color property</h2>

        <p><b><a href="https://www.w3schools.com/css/default.asp" target="_blank">This is a link</a></b></p>
        <p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be effective.</p>
        <p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>
    </body>
</html>
```

Output:

[Click here!](./Links/Example_3.html)

## Add other styles to hyperlinks

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a.one:link {color:#ff0000;}
            a.one:visited {color:#0000ff;}
            a.one:hover {color:#ffcc00;}

            a.two:link {color:#ff0000;}
            a.two:visited {color:#0000ff;}
            a.two:hover {font-size:150%;}

            a.three:link {color:#ff0000;}
            a.three:visited {color:#0000ff;}
            a.three:hover {background:#66ff66;}

            a.four:link {color:#ff0000;}
            a.four:visited {color:#0000ff;}
            a.four:hover {font-family:monospace;}

            a.five:link {color:#ff0000;text-decoration:none;}
            a.five:visited {color:#0000ff;text-decoration:none;}
            a.five:hover {text-decoration:underline;}
        </style>
    </head>
    <body>
        <h2>Styling Links</h2>

        <p>Mouse over the links and watch them change layout:</p>

        <p><b><a class="one" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes color</a></b></p>
        <p><b><a class="two" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes font-size</a></b></p>
        <p><b><a class="three" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes background-color</a></b></p>
        <p><b><a class="four" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes font-family</a></b></p>
        <p><b><a class="five" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes text-decoration</a></b></p>
    </body>
</html>
```

Output:

[Click here!](./Links/Example_4.html)

## Different types of cursors

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The cursor Property</h2>

        <p>Mouse over the words to change the cursor.</p>
        <span style="cursor:auto">auto</span><br>
        <span style="cursor:crosshair">crosshair</span><br>
        <span style="cursor:default">default</span><br>
        <span style="cursor:e-resize">e-resize</span><br>
        <span style="cursor:help">help</span><br>
        <span style="cursor:move">move</span><br>
        <span style="cursor:n-resize">n-resize</span><br>
        <span style="cursor:ne-resize">ne-resize</span><br>
        <span style="cursor:nw-resize">nw-resize</span><br>
        <span style="cursor:pointer">pointer</span><br>
        <span style="cursor:progress">progress</span><br>
        <span style="cursor:s-resize">s-resize</span><br>
        <span style="cursor:se-resize">se-resize</span><br>
        <span style="cursor:sw-resize">sw-resize</span><br>
        <span style="cursor:text">text</span><br>
        <span style="cursor:w-resize">w-resize</span><br>
        <span style="cursor:wait">wait</span><br>
    </body>
</html>
```

Output:

[Click here!](./Links/Example_5.html)

## Advanced - Create link boxes

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a:link, a:visited { background-color: #f44336;
                                color: white;
                                padding: 14px 25px;
                                text-align: center;
                                text-decoration: none;
                                display: inline-block;}

            a:hover, a:active {background-color: red;}
        </style>
    </head>
    <body>
        <h2>Link Button</h2>

        <p>A link styled as a button:</p>
        <a href="https://www.w3schools.com/css/default.asp" target="_blank">This is a link</a>
    </body>
</html>
```

Output:

[Click here!](./Links/Example_6.html)

## Advanced - Create link boxes with borders

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a:link, a:visited { background-color: white;
                                color: black;
                                border: 2px solid green;
                                padding: 10px 20px;
                                text-align: center;
                                text-decoration: none;
                                display: inline-block;}

            a:hover, a:active { background-color: green;
                                color: white;}
        </style>
    </head>
    <body>
        <h2>Link Button</h2>

        <a href="https://www.w3schools.com/css/default.asp" target="_blank">This is a link</a>
    </body>
</html>
```

Output:

[Click here!](./Links/Example_7.html)