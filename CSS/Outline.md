# Outline

## Draw a line around an element (outline)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { border: 2px solid black;
                outline: #4CAF50 solid 10px;
                margin: auto;  
                padding: 20px;
                text-align: center;}
        </style>
    </head>
    <body>
        <h2>CSS Outline</h2>
        <p>This element has a 2px black border and a green outline with a width of 10px.</p>
    </body>
</html>
```

Output:

[Click here!](./Outline/Example_1.html)

## Set the style of an outline

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {outline-color:red;}
            p.dotted {outline-style: dotted;}
            p.dashed {outline-style: dashed;}
            p.solid {outline-style: solid;}
            p.double {outline-style: double;}
            p.groove {outline-style: groove;}
            p.ridge {outline-style: ridge;}
            p.inset {outline-style: inset;}
            p.outset {outline-style: outset;}
        </style>
    </head>
    <body>
        <h2>The outline-style Property</h2>

        <p class="dotted">A dotted outline</p>
        <p class="dashed">A dashed outline</p>
        <p class="solid">A solid outline</p>
        <p class="double">A double outline</p>
        <p class="groove">A groove outline. The effect depends on the outline-color value.</p>
        <p class="ridge">A ridge outline. The effect depends on the outline-color value.</p>
        <p class="inset">An inset outline. The effect depends on the outline-color value.</p>
        <p class="outset">An outset outline. The effect depends on the outline-color value.</p>
    </body>
</html>
```

Output:

[Click here!](./Outline/Example_2.html)

## Set the color of an outline

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.ex1 { border: 2px solid black;
                    outline-style: solid;
                    outline-color: red;}

            p.ex2 { border: 2px solid black;
                    outline-style: dotted;
                    outline-color: blue;}

            p.ex3 { border: 2px solid black;
                    outline-style: outset;
                    outline-color: grey;}
        </style>
    </head>
    <body>
        <h2>The outline-color Property</h2>
        <p>The outline-color property is used to set the color of the outline.</p>

        <p class="ex1">A solid red outline.</p>
        <p class="ex2">A dotted blue outline.</p>
        <p class="ex3">An outset grey outline.</p>
    </body>
</html>
```

Output:

[Click here!](./Outline/Example_3.html)

## Set the width of an outline

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.ex1 { border: 1px solid black;
                    outline-style: solid;
                    outline-color: red;
                    outline-width: thin;}

            p.ex2 { border: 1px solid black;
                    outline-style: solid;
                    outline-color: red;
                    outline-width: medium;}

            p.ex3 { border: 1px solid black;
                    outline-style: solid;
                    outline-color: red;
                    outline-width: thick;}

            p.ex4 { border: 1px solid black;
                    outline-style: solid;
                    outline-color: red;
                    outline-width: 4px;}
        </style>
    </head>
    <body>
        <h2>The outline-width Property</h2>

        <p class="ex1">A thin outline.</p>
        <p class="ex2">A medium outline.</p>
        <p class="ex3">A thick outline.</p>
        <p class="ex4">A 4px thick outline.</p>
    </body>
</html>
```

Output:

[Click here!](./Outline/Example_4.html)

## Use the shorthand outline property

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.ex1 {outline: dashed;}
            p.ex2 {outline: dotted red;}
            p.ex3 {outline: 5px solid yellow;}
            p.ex4 {outline: thick ridge pink;}
        </style>
    </head>
    <body>
        <h2>The outline Property</h2>

        <p class="ex1">A dashed outline.</p>
        <p class="ex2">A dotted red outline.</p>
        <p class="ex3">A 5px solid yellow outline.</p>
        <p class="ex4">A thick ridge pink outline.</p>
    </body>
</html>
```

Output:

[Click here!](./Outline/Example_5.html)

## Add space between an outline and the edge/border of an element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p { margin: 30px;
                border: 1px solid black;
                outline: 1px solid red;
                outline-offset: 15px;}
        </style>
    </head>
    <body>
        <h2>The outline-offset Property</h2>

        <p>This paragraph has an outline 15px outside the border edge.</p>
    </body>
</html>
```

Output:

[Click here!](./Outline/Example_6.html)