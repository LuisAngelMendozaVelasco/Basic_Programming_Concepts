# Padding

## Specify different padding for each side of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    background-color: lightblue;
                    padding-top: 50px;
                    padding-right: 30px;
                    padding-bottom: 50px;
                    padding-left: 80px;}
        </style>
    </head>
    <body>
        <h2>Using individual padding properties</h2>

        <div>This div element has a top padding of 50px, a right padding of 30px, a bottom padding of 50px, and a left padding of 80px.</div>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_1.html)

## Use shorthand padding property with four values

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    padding: 25px 50px 75px 100px;
                    background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>The padding shorthand property - 4 values</h2>

        <div>This div element has a top padding of 25px, a right padding of 50px, a bottom padding of 75px, and a left padding of 100px.</div>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_2.html)

## Use shorthand padding property with three values

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    padding: 25px 50px 75px;
                    background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>The padding shorthand property - 3 values</h2>

        <div>This div element has a top padding of 25px, a right and left padding of 50px, and a bottom padding of 75px.</div>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_3.html)

## Use shorthand padding property with two values

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    padding: 25px 50px;
                    background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>The padding shorthand property - 2 values</h2>

        <div>This div element has a top and bottom padding of 25px, and a right and left padding of 50px.</div>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_4.html)

## Use shorthand padding property with one value

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    padding: 25px;
                    background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>The padding shorthand property - 1 value</h2>

        <div>This div element has a top, bottom, left, and right padding of 25px.</div>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_5.html)

## Padding and element width (without box-sizing)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div.ex1 {   width: 300px;
                        background-color: yellow;}

            div.ex2 {   width: 300px;
                        padding: 25px;
                        background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>Padding and element width</h2>

        <div class="ex1">This div is 300px wide.</div><br>

        <div class="ex2">The width of this div is 350px, even though it is defined as 300px in the CSS.</div>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_6.html)

## Padding and element width (with box-sizing)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div.ex1 {   width: 300px;
                        background-color: yellow;}

            div.ex2 {   width: 300px;
                        padding: 25px;
                        box-sizing: border-box;
                        background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>Padding and element width - with box-sizing</h2>

        <div class="ex1">This div is 300px wide.</div>
        <br>
        <div class="ex2">The width of this div remains at 300px, in spite of the 50px of total left and right padding, because of the box-sizing: border-box property.</div>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_7.html)

## Set padding-left of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.padding {padding-left: 2cm;}
            p.padding2 {padding-left: 50%;}
        </style>
    </head>
    <body>
        <h1>The padding-left Property</h1>

        <p>This is a text with no left padding.</p>
        <p class="padding">This text has a left padding of 2 cm.</p>
        <p class="padding2">This text has a left padding of 50%.</p>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_8.html)

## Set padding-right of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.padding {padding-right: 2cm;}
            p.padding2 {padding-right: 50%;}
        </style>
    </head>
    <body>
        <h1>The padding-right Property</h1>

        <p>This is a text with no right padding. This is a text with no right padding. This is a text with no right padding.</p>
        <p class="padding">This text has a right padding of 2 cm. This text has a right padding of 2 cm. This text has a right padding of 2 cm.</p>
        <p class="padding2">This text has a right padding of 50%. This text has a right padding of 50%. This text has a right padding of 50%.</p>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_9.html)

## Set padding-top of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.padding {padding-top: 2cm;}
            p.padding2 {padding-top: 50%;}
        </style>
    </head>
    <body>
        <h1>The padding-top Property</h1>

        <p>This is a text with no top padding. This is a text with no top padding. This is a text with no top padding.</p>
        <p class="padding">This text has a top padding of 2 cm. This text has a top padding of 2 cm. This text has a top padding of 2 cm.</p>
        <p class="padding2">This text has a top padding of 50%. This text has a top padding of 50%. This text has a top padding of 50%.</p>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_10.html)

## Set padding-bottom of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.padding {padding-bottom:2cm;}
            p.padding2 {padding-bottom:50%;}
        </style>
    </head>
    <body>
        <h1>The padding-bottom Property</h1>

        <p>This is a text with no bottom padding. This is a text with no bottom padding. This is a text with no bottom padding.</p>
        <p class="padding">This text has a bottom padding of 2 cm. This text has a bottom padding of 2 cm. This text has a bottom padding of 2 cm.</p>
        <p class="padding2">This text has a bottom padding of 50%. This text has a bottom padding of 50%. This text has a bottom padding of 50%.</p>
    </body>
</html>
```

Output:

[Click here!](./Padding/Example_11.html)