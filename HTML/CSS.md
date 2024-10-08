# CSS

## HTML with inline CSS

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1 style="color:blue;">A Blue Heading</h1>
        <p style="color:red;">A red paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_1.html)

## HTML with internal CSS

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {background-color: powderblue;}
            h1   {color: blue;}
            p    {color: red;}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_2.html)

## HTML with external CSS

Code:

```css
body {background-color: powderblue;}
h1 {color: blue;}
p {color: red;}
```

```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="./styles.css">
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_3.html)

## HTML with CSS fonts

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {color: blue;
                font-family: verdana;
                font-size: 300%;}
            p { color: red;
                font-family: courier;
                font-size: 160%;}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_4.html)

## HTML with CSS using the id attribute

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #p01 {color: blue;}
        </style>
    </head>
    <body>
        <p>This is a paragraph.</p>
        <p>This is a paragraph.</p>
        <p id="p01">I am different.</p>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_5.html)

## HTML with CSS using the class attribute

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.error {color: red;}
        </style>
    </head>
    <body>
        <p>This is a paragraph.</p>
        <p>This is a paragraph.</p>
        <p class="error">I am different.</p>
        <p>This is a paragraph.</p>
        <p class="error">I am different too.</p>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_6.html)

## HTML and CSS borders

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {border: 2px solid powderblue;}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
        <p>This is a paragraph.</p>
        <p>This is a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_7.html)

## HTML and CSS padding

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border: 2px solid powderblue;
                padding: 30px;}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
        <p>This is a paragraph.</p>
        <p>This is a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_8.html)

## HTML and CSS margin

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border: 2px solid powderblue;
                margin: 50px;}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
        <p>This is a paragraph.</p>
        <p>This is a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_9.html)

## HTML and CSS full demo

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <div style="position:relative;">
            <div style="opacity:0.5;position:absolute;left:50px;top:-30px;width:300px;height:150px;background-color:#40B3DF"></div>
            <div style="opacity:0.3;position:absolute;left:120px;top:20px;width:100px;height:170px;background-color:#73AD21"></div>
            <div style="margin-top:30px;width:360px;height:130px;padding:20px;border-radius:10px;border:10px solid #EE872A;font-size:120%;">
                <h1>CSS = Styles and Colors</h1>
                <div style="letter-spacing:12px;font-size:15px;position:relative;left:25px;top:25px;">Manipulate Text</div>
                <div style="color:#40B3DF;letter-spacing:12px;font-size:15px;position:relative;left:25px;top:30px;">
                    Colors,
                    <span style="background-color:#B4009E;color:#ffffff;"> Boxes</span>
                </div>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./CSS/Example_10.html)