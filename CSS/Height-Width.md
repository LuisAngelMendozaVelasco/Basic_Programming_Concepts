# Height/Width

## Set the height and width of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   height: 100px;
                    width: 500px;
                    background-color: powderblue;}
        </style>
    </head>
    <body>
        <h2>Set the height and width of an element</h2>

        <div>This div element has a height of 100px and a width of 500px.</div>
    </body>
</html>
```

Output:

[Click here!](./Height-Width/Example_1.html)

## Set max-width of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   max-width: 500px;
                    height: 100px;
                    background-color: powderblue;}
        </style>
    </head>
    <body>
        <h2>Set the max-width of an element</h2>

        <div>This div element has a height of 100px and a max-width of 500px.</div>

        <p>Resize the browser window to see the effect.</p>
    </body>
</html>
```

Output:

[Click here!](./Height-Width/Example_2.html)

## Set the height and width of different elements

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img.one {height: auto;}

            img.two {   height: 200px;
                        width: 200px;}

            div.three { height: 300px;
                        width: 300px;
                        background-color: powderblue;}
        </style>
    </head>
    <body>
        <h2>Set the height and width of elements</h2>

        <p>Original image:</p>
        <img class="one" src="../data/images/ocean.jpg" width="300" height="300"><br>

        <p>Sized image (200x200 pixels):</p>
        <img class="two" src="../data/images/ocean.jpg" width="300" height="300"><br>

        <p>The height and width of this div element is 300px:</p>
        <div class="three"></div>
    </body>
</html>
```

Output:

[Click here!](./Height-Width/Example_3.html)

## Set the height and width of an image using percent

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            html, body {height: 100%;}

            img.one {   height: auto;
                        width: auto;}

            img.two {   height: 50%;
                        width: 50%;}
        </style>
    </head>
    <body>
        <h2>Set the height and width in %</h2>
        <p>Resize the browser window to see the effect.</p>

        <p>Original image:</p>
        <img class="one" src="../data/images/ocean.jpg" width="300" height="300"><br>

        <p>Sized image (in %):</p>
        <img class="two" src="../data/images/ocean.jpg" width="300" height="300">
    </body>
</html>
```

Output:

[Click here!](./Height-Width/Example_4.html)

## Set min-width and max-width of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   max-width: 400px;
                    min-width: 100px;
                    background-color: powderblue;}
        </style>
    </head>
    <body>
        <h2>Set the max-width and min-width of an element</h2>
        <p>Resize the browser window to see the effect.</p>

        <div>
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Height-Width/Example_5.html)

## Set min-height and max-height of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   max-height: 600px;
                    min-height: 400px;
                    background-color: powderblue;}
        </style>
    </head>
    <body>
        <h2>Set the max-height and min-height of an element</h2>
        <p>Resize the browser window to see the effect.</p>

        <div>
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
            This is some text. This is some text. This is some text.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Height-Width/Example_6.html)