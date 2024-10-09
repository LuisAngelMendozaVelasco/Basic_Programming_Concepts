# Colors

## Set the background color of an element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1 style="background-color:DodgerBlue;">Hello World</h1>

        <p style="background-color:Tomato;">
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.
            Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.
        </p>
    </body>
</html>
```

Output:

[Click here!](./Colors/Example_1.html)

## Set the text color

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h3 style="color:Tomato;">Hello World</h3>

        <p style="color:DodgerBlue;">Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>

        <p style="color:MediumSeaGreen;">Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
    </body>
</html>
```

Output:

[Click here!](./Colors/Example_2.html)

## Set the border color

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1 style="border: 2px solid Tomato;">Hello World</h1>

        <h1 style="border: 2px solid DodgerBlue;">Hello World</h1>

        <h1 style="border: 2px solid Violet;">Hello World</h1>
    </body>
</html>
```

Output:

[Click here!](./Colors/Example_3.html)

## Set different color values

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Same as color name "Tomato":</p>

        <h1 style="background-color:rgb(255, 99, 71);">rgb(255, 99, 71)</h1>
        <h1 style="background-color:#ff6347;">#ff6347</h1>
        <h1 style="background-color:hsl(9, 100%, 64%);">hsl(9, 100%, 64%)</h1>

        <p>Same as color name "Tomato", but 50% transparent:</p>
        <h1 style="background-color:rgba(255, 99, 71, 0.5);">rgba(255, 99, 71, 0.5)</h1>
        <h1 style="background-color:hsla(9, 100%, 64%, 0.5);">hsla(9, 100%, 64%, 0.5)</h1>

        <p>In addition to the predefined color names, colors can be specified using RGB, HEX, HSL, or even transparent colors using RGBA or HSLA color values.</p>
    </body>
</html>
```

Output:

[Click here!](./Colors/Example_4.html)

## Set RGB values

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Specify colors using RGB values</h1>

        <h2 style="background-color:rgb(255, 0, 0);">rgb(255, 0, 0)</h2>
        <h2 style="background-color:rgb(0, 0, 255);">rgb(0, 0, 255)</h2>
        <h2 style="background-color:rgb(60, 179, 113);">rgb(60, 179, 113)</h2>
        <h2 style="background-color:rgb(238, 130, 238);">rgb(238, 130, 238)</h2>
        <h2 style="background-color:rgb(255, 165, 0);">rgb(255, 165, 0)</h2>
        <h2 style="background-color:rgb(106, 90, 205);">rgb(106, 90, 205)</h2>
    </body>
</html>
```

Output:

[Click here!](./Colors/Example_5.html)

## Set HEX values

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Shades of gray</h1>

        <p>By using equal values for red, green, and blue, you will get different shades of gray:</p>

        <h2 style="background-color:#3c3c3c;">#3c3c3c</h2>
        <h2 style="background-color:#616161;">#616161</h2>
        <h2 style="background-color:#787878;">#787878</h2>
        <h2 style="background-color:#b4b4b4;">#b4b4b4</h2>
        <h2 style="background-color:#f0f0f0;">#f0f0f0</h2>
        <h2 style="background-color:#f9f9f9;">#f9f9f9</h2>
    </body>
</html>
```

Output:

[Click here!](./Colors/Example_6.html)

## Set HSL values

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Specify colors using HSL values</h1>

        <h2 style="background-color:hsl(0, 100%, 50%);">hsl(0, 100%, 50%)</h2>
        <h2 style="background-color:hsl(240, 100%, 50%);">hsl(240, 100%, 50%)</h2>
        <h2 style="background-color:hsl(147, 50%, 47%);">hsl(147, 50%, 47%)</h2>
        <h2 style="background-color:hsl(300, 76%, 72%);">hsl(300, 76%, 72%)</h2>
        <h2 style="background-color:hsl(39, 100%, 50%);">hsl(39, 100%, 50%)</h2>
        <h2 style="background-color:hsl(248, 53%, 58%);">hsl(248, 53%, 58%)</h2>
    </body>
</html>
```

Output:

[Click here!](./Colors/Example_7.html)