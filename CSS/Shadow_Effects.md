# Shadow Effects

## Simple shadow effect

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {text-shadow: 2px 2px;}
        </style>
    </head>
    <body>
        <h1>Text-shadow effect!</h1>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_1.html)

## Add a color to the shadow

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {text-shadow: 2px 2px red;}
        </style>
    </head>
    <body>
        <h1>Text-shadow effect!</h1>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_2.html)

## Add a blur effect to the shadow

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {text-shadow: 2px 2px 5px red;}
        </style>
    </head>
    <body>
        <h1>Text-shadow effect!</h1>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_3.html)

## White text with black shadow

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {color: white;
                text-shadow: 2px 2px 4px #000000;}
        </style>
    </head>
    <body>
        <h1>Text-shadow effect!</h1>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_4.html)

## A red neon glow shadow

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {text-shadow: 0 0 3px #FF0000;}
        </style>
    </head>
    <body>
        <h1>Text-shadow with red neon glow!</h1>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_5.html)

## A red and blue neon glow shadow

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {text-shadow: 0 0 3px #FF0000, 0 0 5px #0000FF;}
        </style>
    </head>
    <body>
        <h1>Text-shadow with red and blue neon glow!</h1>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_6.html)

## White text with black, blue, and darkblue shadow

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {color: white;
                text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue;}
        </style>
    </head>
    <body>
        <h1>Text-shadow effect!</h1>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_7.html)

## Add a simple box-shadow to an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 300px;
                    height: 100px;
                    padding: 15px;
                    background-color: coral;
                    box-shadow: 10px 10px;}
        </style>
    </head>
    <body>
        <h1>The box-shadow Property</h1>

        <div>This is a div element with a box-shadow</div>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_8.html)

## Add color to box-shadow

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 300px;
                    height: 100px;
                    padding: 15px;
                    background-color: coral;
                    box-shadow: 10px 10px lightblue;}
        </style>
    </head>
    <body>
        <h1>The box-shadow Property</h1>

        <div>A div element with a lightblue box-shadow</div>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_9.html)

## Add color and blur effect to box-shadow

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 300px;
                    height: 100px;
                    padding: 15px;
                    background-color: coral;
                    box-shadow: 10px 10px 5px lightblue;}
        </style>
    </head>
    <body>
        <h1>The box-shadow Property</h1>

        <div>A div element with a 5px blurred, lightblue box-shadow.</div>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_10.html)

## Create paper-like cards (text)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div.card {  width: 250px;
                        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
                        text-align: center;}

            div.header {background-color: #4CAF50;
                        color: white;
                        padding: 10px;
                        font-size: 40px;}

            div.container {padding: 10px;}
        </style>
    </head>
    <body>
        <h1>Create Cards</h1>

        <p>The box-shadow property can be used to create paper-like cards:</p>

        <div class="card">
            <div class="header">
                <h1>1</h1>
            </div>

            <div class="container">
                <p>January 1, 2021</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_11.html)

## Create paper-like cards (polaroid images)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div.polaroid {  width: 250px;
                            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
                            text-align: center;}

            div.container {padding: 10px;}
        </style>
    </head>
    <body>
        <h1>Create Polaroid Images</h1>

        <p>The box-shadow property can be used to create polaroid images:</p>

        <div class="polaroid">
            <img src="../data/images/rock600x400.jpg" alt="Norway" style="width:100%">
            <div class="container">
                <p>Hardanger, Norway</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Shadow_Effects/Example_12.html)