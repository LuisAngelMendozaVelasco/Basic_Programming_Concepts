# Text

## Set the text color of different elements

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {color: blue;}
            h1 {color: green;}
        </style>
    </head>
    <body>
        <h1>This is heading 1</h1>
        <p>This is an ordinary paragraph. Notice that this text is blue. The default text color for a page is defined in the body selector.</p>
        <p>Another paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_1.html)

## Align the text

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {text-align: center;}
            h2 {text-align: left;}
            h3 {text-align: right;}
        </style>
    </head>
    <body>
        <h1>Heading 1 (center)</h1>
        <h2>Heading 2 (left)</h2>
        <h3>Heading 3 (right)</h3>

        <p>The three headings above are aligned center, left and right.</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_2.html)

## Remove the line under links

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a {text-decoration: none;}
        </style>
    </head>
    <body>
        <h1>Using text-decoration: none</h1>

        <p>A link with no underline: <a href="https://www.w3schools.com">W3Schools.com</a></p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_3.html)

## Decorate the text

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {text-decoration: underline;}
            h2 {text-decoration: underline red;}
            h3 {text-decoration: underline red double;}
            p {text-decoration: underline red double 5px;}
        </style>
    </head>
    <body>
        <h1>Heading 1</h1>
        <h2>Heading 2</h2>
        <h3>Heading 3</h3>
        <p>A paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_4.html)

## Control the letters in a text

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.uppercase {text-transform: uppercase;}
            p.lowercase {text-transform: lowercase;}
            p.capitalize {text-transform: capitalize;}
        </style>
    </head>
    <body>
        <h1>Using the text-transform property</h1>

        <p class="uppercase">This text is transformed to uppercase.</p>
        <p class="lowercase">This text is transformed to lowercase.</p>
        <p class="capitalize">This text is capitalized.</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_5.html)

## Indent text

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {text-indent: 50px;}
        </style>
    </head>
    <body>
        <h1>Using text-indent</h1>

        <p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my mind ever since. 'Whenever you feel like criticizing anyone,' he told me, 'just remember that all the people in this world haven't had the advantages that you've had.'</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_6.html)

## Specify the space between characters

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h2 {letter-spacing: 5px;}
            h3 {letter-spacing: -2px;}
        </style>
    </head>
    <body>
        <h1>Using letter-spacing</h1>

        <h2>This is heading 1</h2>
        <h3>This is heading 2</h3>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_7.html)

## Specify the space between lines

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.small {line-height: 0.7;}
            p.big {line-height: 1.8;}
        </style>
    </head>
    <body>
        <h1>Using line-height</h1>

        <p>
            This is a paragraph with a standard line-height.<br>
            The default line height in most browsers is about 110% to 120%.<br>
        </p>

        <p class="small">
            This is a paragraph with a smaller line-height.<br>
            This is a paragraph with a smaller line-height.<br>
        </p>

        <p class="big">
            This is a paragraph with a bigger line-height.<br>
            This is a paragraph with a bigger line-height.<br>
        </p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_8.html)

## Set the text direction of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.ex1 { direction: rtl;
                    unicode-bidi: bidi-override;}
        </style>
    </head>
    <body>
        <p>This is the default text direction.</p>

        <p class="ex1">This is right-to-left text direction.</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_9.html)

## Increase the white space between words

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.one {word-spacing: 10px;}
            p.two {word-spacing: -2px;}
        </style>
    </head>
    <body>
        <h1>Using word-spacing</h1>

        <p>This is a paragraph with normal word spacing.</p>

        <p class="one">This is a paragraph with larger word spacing.</p>

        <p class="two">This is a paragraph with smaller word spacing.</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_10.html)

## Specify a text shadow for an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {text-shadow: 3px 2px red;}
        </style>
    </head>
    <body>
        <h1>Text-shadow effect</h1>
        <p><b>Note:</b> Internet Explorer 9 and earlier do not support the text-shadow property.</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_11.html)

## Disable text wrapping inside an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {white-space: nowrap;}
        </style>
    </head>
    <body>
        <h1>Using white-space</h1>

        <p>
            This is some text that will not wrap.
            This is some text that will not wrap.
            This is some text that will not wrap.
            This is some text that will not wrap.
            This is some text that will not wrap.
            This is some text that will not wrap.
            This is some text that will not wrap.
            This is some text that will not wrap.
            This is some text that will not wrap.
        </p>

        <p>Try to remove the white-space property to see the difference!</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_12.html)

## Vertical alignment of an image inside text

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img.a {vertical-align: baseline;}
            img.b {vertical-align: text-top;}
            img.c {vertical-align: text-bottom;}
            img.d {vertical-align: sub;}
            img.e {vertical-align: super;}
        </style>
    </head>
    <body>
        <h1>The vertical-align Property</h1>

        <h2>vertical-align: baseline (default):</h2>
        <p>An <img class="a" src="../data/images/sqpurple.gif" width="9" height="9"> image with a default alignment.</p> 

        <h2>vertical-align: text-top:</h2>
        <p>An <img class="b" src="../data/images/sqpurple.gif" width="9" height="9"> image with a text-top alignment.</p> 

        <h2>vertical-align: text-bottom:</h2>
        <p>An <img class="c" src="../data/images/sqpurple.gif" width="9" height="9"> image with a text-bottom alignment.</p>

        <h2>vertical-align: sub:</h2>
        <p>An <img class="d" src="../data/images/sqpurple.gif" width="9" height="9"> image with a sub alignment.</p> 

        <h2>vertical-align: sup:</h2>
        <p>An <img class="e" src="../data/images/sqpurple.gif" width="9" height="9"> image with a super alignment.</p>
    </body>
</html>
```

Output:

[Click here!](./Text/Example_13.html)