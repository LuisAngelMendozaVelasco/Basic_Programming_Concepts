# Borders

## Set the width of the four borders

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.one { border-style: solid;
                    border-width: 5px;}

            p.two { border-style: solid;
                    border-width: medium;}

            p.three {   border-style: dotted;
                        border-width: 2px;}

            p.four {border-style: dotted;
                    border-width: thick;}

            p.five {border-style: double;
                    border-width: 15px;}

            p.six { border-style: double;
                    border-width: thick;}
        </style>
    </head>
    <body>
        <h2>The border-width Property</h2>
        <p>This property specifies the width of the four borders:</p>

        <p class="one">Some text.</p>
        <p class="two">Some text.</p>
        <p class="three">Some text.</p>
        <p class="four">Some text.</p>
        <p class="five">Some text.</p>
        <p class="six">Some text.</p>

        <p><b>Note:</b> The "border-width" property does not work if it is used alone. 
        Always specify the "border-style" property to set the borders first.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_1.html)

## Set the width of the top border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-top-width: 15px;}
        </style>
    </head>
    <body>
        <p><b>Note:</b> The "border-top-width" property does not work if it is used alone. Use the "border-style" property to set the borders first.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_2.html)

## Set the width of the bottom border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-bottom-width: 15px;}
        </style>
    </head>
    <body>
        <p><b>Note:</b> The "border-bottom-width" property does not work if it is used alone. Use the "border-style" property to set the borders first.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_3.html)

## Set the width of the left border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-left-width: 15px;}
        </style>
    </head>
    <body>
        <p><b>Note:</b> The "border-left-width" property does not work if it is used alone. Use the "border-style" property to set the borders first.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_4.html)

## Set the width of the right border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-right-width: 15px;}
        </style>
    </head>
    <body>
        <p><b>Note:</b> The "border-right-width" property does not work if it is used alone. Use the "border-style" property to set the borders first.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_5.html)

## Set the style of the four borders

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.dotted {border-style: dotted;}
            p.dashed {border-style: dashed;}
            p.solid {border-style: solid;}
            p.double {border-style: double;}
            p.groove {border-style: groove;}
            p.ridge {border-style: ridge;}
            p.inset {border-style: inset;}
            p.outset {border-style: outset;}
            p.none {border-style: none;}
            p.hidden {border-style: hidden;}
            p.mix {border-style: dotted dashed solid double;}
        </style>
    </head>
    <body>
        <h2>The border-style Property</h2>
        <p>This property specifies what kind of border to display:</p>

        <p class="dotted">A dotted border.</p>
        <p class="dashed">A dashed border.</p>
        <p class="solid">A solid border.</p>
        <p class="double">A double border.</p>
        <p class="groove">A groove border.</p>
        <p class="ridge">A ridge border.</p>
        <p class="inset">An inset border.</p>
        <p class="outset">An outset border.</p>
        <p class="none">No border.</p>
        <p class="hidden">A hidden border.</p>
        <p class="mix">A mixed border.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_6.html)

## Set the style of the top border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {border-style: solid;}
            p.none {border-top-style: none;}
            p.dotted {border-top-style: dotted;}
            p.dashed {border-top-style: dashed;}
            p.solid {border-top-style: solid;}
            p.double {border-top-style: double;}
            p.groove {border-top-style: groove;}
            p.ridge {border-top-style: ridge;}
            p.inset {border-top-style: inset;}
            p.outset {border-top-style: outset;}
        </style>
    </head>
    <body>
        <p class="none">No top border.</p>
        <p class="dotted">A dotted top border.</p>
        <p class="dashed">A dashed top border.</p>
        <p class="solid">A solid top border.</p>
        <p class="double">A double top border.</p>
        <p class="groove">A groove top border.</p>
        <p class="ridge">A ridge top border.</p>
        <p class="inset">An inset top border.</p>
        <p class="outset">An outset top border.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_7.html)

## Set the style of the bottom border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {border-style: solid;}
            p.none {border-bottom-style: none;}
            p.dotted {border-bottom-style: dotted;}
            p.dashed {border-bottom-style: dashed;}
            p.solid {border-bottom-style: solid;}
            p.double {border-bottom-style: double;}
            p.groove {border-bottom-style: groove;}
            p.ridge {border-bottom-style: ridge;}
            p.inset {border-bottom-style: inset;}
            p.outset {border-bottom-style: outset;}
        </style>
    </head>
    <body>
        <p class="none">No bottom border.</p>
        <p class="dotted">A dotted bottom border.</p>
        <p class="dashed">A dashed bottom border.</p>
        <p class="solid">A solid bottom border.</p>
        <p class="double">A double bottom border.</p>
        <p class="groove">A groove bottom border.</p>
        <p class="ridge">A ridge bottom border.</p>
        <p class="inset">An inset bottom border.</p>
        <p class="outset">An outset bottom border.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_8.html)

## Set the style of the left border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {border-style: solid;}
            p.none {border-left-style: none;}
            p.dotted {border-left-style: dotted;}
            p.dashed {border-left-style: dashed;}
            p.solid {border-left-style: solid;}
            p.double {border-left-style: double;}
            p.groove {border-left-style: groove;}
            p.ridge {border-left-style: ridge;}
            p.inset {border-left-style: inset;}
            p.outset {border-left-style: outset;}
        </style>
    </head>
    <body>
        <p class="none">No left border.</p>
        <p class="dotted">A dotted left border.</p>
        <p class="dashed">A dashed left border.</p>
        <p class="solid">A solid left border.</p>
        <p class="double">A double left border.</p>
        <p class="groove">A groove left border.</p>
        <p class="ridge">A ridge left border.</p>
        <p class="inset">An inset left border.</p>
        <p class="outset">An outset left border.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_9.html)

## Set the style of the right border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {border-style: solid;}
            p.none {border-right-style: none;}
            p.dotted {border-right-style: dotted;}
            p.dashed {border-right-style: dashed;}
            p.solid {border-right-style: solid;}
            p.double {border-right-style: double;}
            p.groove {border-right-style: groove;}
            p.ridge {border-right-style: ridge;}
            p.inset {border-right-style: inset;}
            p.outset {border-right-style: outset;}
        </style>
    </head>
    <body>
        <p class="none">No right border.</p>
        <p class="dotted">A dotted right border.</p>
        <p class="dashed">A dashed right border.</p>
        <p class="solid">A solid right border.</p>
        <p class="double">A double right border.</p>
        <p class="groove">A groove right border.</p>
        <p class="ridge">A ridge right border.</p>
        <p class="inset">An inset right border.</p>
        <p class="outset">An outset right border.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_10.html)

## Set the color of the four borders

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.one { border-style: solid;
                    border-color: #0000ff;}

            p.two { border-style: solid;
                    border-color: #ff0000 #0000ff;}

            p.three {   border-style: solid;
                        border-color: #ff0000 #00ff00 #0000ff;}

            p.four {border-style: solid;
                    border-color: #ff0000 #00ff00 #0000ff rgb(250,0,255);}
        </style>
    </head>
    <body>
        <p class="one">One-colored border!</p>
        <p class="two">Two-colored border!</p>
        <p class="three">Three-colored border!</p>
        <p class="four">Four-colored border!</p>
        <p><b>Note:</b> The "border-color" property does not work if it is used alone. Use the "border-style" property to set the borders first.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_11.html)

## Set the color of the top border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-top-color: #ff0000;}
        </style>
    </head>
    <body>
        <p>This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_12.html)

## Set the color of the bottom border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-bottom-color: #ff0000;}
        </style>
    </head>
    <body>
        <p>This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_13.html)

## Set the color of the left border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-left-color: #ff0000;}
        </style>
    </head>
    <body>
        <p>This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_14.html)

## Set the color of the right border

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-right-color: #ff0000;}
        </style>
    </head>
    <body>
        <p>This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_15.html)

## All the border properties in one declaration

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {border: 5px solid red;}
        </style>
    </head>
    <body>
        <h2>The border Property</h2>

        <p>This property is a shorthand property for border-width, border-style, and border-color.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_16.html)

## Add rounded borders to an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.normal {  border: 2px solid red;
                        padding: 5px;}

            p.round1 {  border: 2px solid red;
                        border-radius: 5px;
                        padding: 5px;}

            p.round2 {  border: 2px solid red;
                        border-radius: 8px;
                        padding: 5px;}

            p.round3 {  border: 2px solid red;
                        border-radius: 12px;
                        padding: 5px;}
        </style>
    </head>
    <body>
        <h2>The border-radius Property</h2>
        <p>This property is used to add rounded borders to an element:</p>

        <p class="normal">Normal border</p>
        <p class="round1">Round border</p>
        <p class="round2">Rounder border</p>
        <p class="round3">Roundest border</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_17.html)

## Set different borders on each side

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.one {border-style: dotted solid dashed double;}

            p.two {border-style: dotted solid dashed;}

            p.three {border-style: dotted solid;}

            p.four {border-style: dotted;}
        </style>
    </head>
    <body>
        <p class="one">This is some text in a paragraph.</p>
        <p class="two">This is some text in a paragraph.</p>
        <p class="three">This is some text in a paragraph.</p>
        <p class="four">This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_18.html)

## All the top border properties in one declaration

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-top: thick double #ff0000;}
        </style>
    </head>
    <body>
        <p>This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_19.html)

## All the bottom border properties in one declaration

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-bottom: thick dotted #ff0000;}
        </style>
    </head>
    <body>
        <p>This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_20.html)

## All the left border properties in one declaration

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-left: thick double #ff0000;}
        </style>
    </head>
    <body>
        <p>This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_21.html)

## All the right border properties in one declaration

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border-style: solid;
                border-right: thick double #ff0000;}
        </style>
    </head>
    <body>
        <p>This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Borders/Example_22.html)