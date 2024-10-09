# Pseudo-elements

## Make the first letter special in a text

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p::first-letter {color: #ff0000;
                            font-size: xx-large;}
        </style>
    </head>
    <body>
        <p>You can use the ::first-letter pseudo-element to add a special effect to the first character of a text!</p>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-elements/Example_1.html)

## Make the first line special in a text

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p::first-line { color: #ff0000;
                            font-variant: small-caps;}
        </style>
    </head>
    <body>
        <p>You can use the ::first-line pseudo-element to add a special effect to the first line of a text. Some more text. And even more, and more, and more, and more, and more, and more, and more, and more, and more, and more, and more, and more.</p>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-elements/Example_2.html)

## Make the first letter and first line special

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p::first-letter {   color: #ff0000;
                                font-size: xx-large;}

            p::first-line { color: #0000ff;
                            font-variant: small-caps;}
        </style>
    </head>
    <body>
        <p>You can combine the ::first-letter and ::first-line pseudo-elements to add a special effect to the first letter and the first line of a text!</p>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-elements/Example_3.html)

## Use :before to insert some content before an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1::before {content: url(../data/images/smiley.gif);}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>The ::before pseudo-element inserts content before the content of an element.</p>

        <h1>This is a heading</h1>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-elements/Example_4.html)

## Use :after to insert some content after an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1::after {content: url(../data/images/smiley.gif);}
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>The ::after pseudo-element inserts content after the content of an element.</p>

        <h1>This is a heading</h1>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-elements/Example_5.html)