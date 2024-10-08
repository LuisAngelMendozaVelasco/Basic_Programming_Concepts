# Computercode Elements

## Keyboard input formatting using the `<kbd>` element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The kbd Element</h2>

        <p>The kbd element is used to define keyboard input:</p>

        <p>Save the document by pressing <kbd>Ctrl + S</kbd></p>
    </body>
</html>
```

Output:

[Click here!](./Computercode_Elements/Example_1.html)

## Computer output formatting using the `<samp>` element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The samp Element</h2>

        <p>The samp element is used to define sample output from a computer program.</p>

        <p>Message from my computer:</p>
        <p><samp>
            File not found.
            <br>
            Press F1 to continue
        </samp></p>
    </body>
</html>     
```

Output:

[Click here!](./Computercode_Elements/Example_2.html)

## Programming code formatting using the `<code>` element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The code Element</h2>
        <p>Programming code example:</p>

        <code>
            x = 5;
            y = 6;
            z = x + y;
        </code>
    </body>
</html>
```

Output:

[Click here!](./Computercode_Elements/Example_3.html)

## Programming code formatting preserving whitespace and line-breaks

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            pre, code {white-space: pre-line;}
        </style>
    </head>
    <body>
        <p>The code element does not preserve whitespace and line-breaks.</p>
        <p>To fix this, you can put the code element inside a pre element:</p>

        <pre>
            <code>
                x = 5;
                y = 6;
                z = x + y;
            </code>
        </pre>
    </body>
</html>
```

Output:

[Click here!](./Computercode_Elements/Example_4.html)

## Variable formatting using the `<var>` element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The var Element</h2>

        <p>The area of a triangle is: 1/2 x <var>b</var> x <var>h</var>, where <var>b</var> is the base, and <var>h</var> is the vertical height.</p>
    </body>
</html>   
```

Output:

[Click here!](./Computercode_Elements/Example_5.html)