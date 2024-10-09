# Margins

## Specify different margins for each side of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    margin-top: 100px;
                    margin-bottom: 100px;
                    margin-right: 150px;
                    margin-left: 80px;
                    background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>Using individual margin properties</h2>

        <div>This div element has a top margin of 100px, a right margin of 150px, a bottom margin of 100px, and a left margin of 80px.</div>
    </body>
</html>
```

Output:

[Click here!](./Margins/Example_1.html)

## Use shorthand margin property with four values

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    margin: 25px 50px 75px 100px;
                    background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>The margin shorthand property - 4 values</h2>

        <div>This div element has a top margin of 25px, a right margin of 50px, a bottom margin of 75px, and a left margin of 100px.</div>
        <hr>
    </body>
</html>
```

Output:

[Click here!](./Margins/Example_2.html)

## Use shorthand margin property with three values

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    margin: 25px 50px 75px;
                    background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>The margin shorthand property - 3 values</h2>

        <div>This div element has a top margin of 25px, a right and left margin of 50px, and a bottom margin of 75px.</div>
        <hr>
    </body>
</html>
```

Output:

[Click here!](./Margins/Example_3.html)

## Use shorthand margin property with two values

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    margin: 25px 50px;
                    background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>The margin shorthand property - 2 values</h2>

        <div>This div element has a top and bottom margin of 25px, and a right and left margin of 50px.</div>
        <hr>
    </body>
</html>
```

Output:

[Click here!](./Margins/Example_4.html)

## Use shorthand margin property with one value

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid black;
                    margin: 25px;
                    background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>The margin shorthand property - 1 value</h2>

        <div>This div element has a top, bottom, left, and right margin of 25px.</div>
        <hr>
    </body>
</html>
```

Output:

[Click here!](./Margins/Example_5.html)

## Set margin to auto to center the element within its container

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   width: 300px;
                    margin: auto;
                    border: 1px solid red;}
        </style>
    </head>
    <body>
        <h2>Use of margin: auto</h2>
        <p>You can set the margin property to auto to horizontally center the element within its container. The element will then take up the specified width, and the remaining space will be split equally between the left and right margins:</p>

        <div>This div will be horizontally centered because it has margin: auto;</div>
    </body>
</html>
```

Output:

[Click here!](./Margins/Example_6.html)

## Let the left margin be inherited from the parent element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   border: 1px solid red;
                    margin-left: 100px;}

            p.ex1 {margin-left: inherit;}
        </style>
    </head>
    <body>
        <h2>Use of the inherit value</h2>
        <p>Let the left margin be inherited from the parent element:</p>

        <div>
            <p class="ex1">This paragraph has an inherited left margin (from the div element).</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Margins/Example_7.html)

## Margin collapse

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {margin: 0 0 50px 0;}
            h2 {margin: 20px 0 0 0;}
        </style>
    </head>
    <body>
        <p>In this example the h1 element has a bottom margin of 50px and the h2 element has a top margin of 20px. So, the vertical margin between h1 and h2 should have been 70px (50px + 20px). However, due to margin collapse, the actual margin ends up being 50px.</p>

        <h1>Heading 1</h1>
        <h2>Heading 2</h2>
    </body>
</html>
```

Output:

[Click here!](./Margins/Example_8.html)