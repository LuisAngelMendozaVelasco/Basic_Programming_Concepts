# Display

## How to hide an element (visibility:hidden)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1.hidden {visibility: hidden;}
        </style>
    </head>
    <body>
        <h1>This is a visible heading</h1>
        <h1 class="hidden">This is a hidden heading</h1>
        <p>Notice that the hidden heading still takes up space.</p>
    </body>
</html>
```

Output:

[Click here!](./Display/Example_1.html)

## How to not display an element (display:none)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1.hidden {display: none;}
        </style>
    </head>
    <body>
        <h1>This is a visible heading</h1>
        <h1 class="hidden">This is a hidden heading</h1>
        <p>Notice that the h1 element with display: none; does not take up any space.</p>
    </body>
</html>
```

Output:

[Click here!](./Display/Example_2.html)

## How to display a block-level element as an inline element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {display: inline;}
        </style>
    </head>
    <body>
        <p>These two paragraphs generates inline boxes, and it results in</p>

        <p>no distance between the two elements.</p>
    </body>
</html>
```

Output:

[Click here!](./Display/Example_3.html)

## How to display an inline element as a block-level element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            span {display: block;}
        </style>
    </head>
    <body>
        <h1>Display span elements as block elements</h1>

        <span>A display property with</span> <span>a value of "block" results in</span> <span>a line break between each span elements.</span>
    </body>
</html>
```

Output:

[Click here!](./Display/Example_4.html)

## How to to use CSS together with JavaScript to show hidden content

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #panel, .flip { font-size: 16px;
                            padding: 10px;
                            text-align: center;
                            background-color: #4CAF50;
                            color: white;
                            border: solid 1px #a6d8a8;
                            margin: auto;}

            #panel {display: none;}
        </style>
    </head>
    <body>
        <p class="flip" onclick="myFunction()">Click to show panel</p>

        <div id="panel">
            <p>This panel contains a div element, which is hidden by default (display: none).</p>
            <p>It is styled with CSS and we use JavaScript to show it (display: block).</p>
            <p>How it works: Notice that the p element with class="flip" has an onclick attribute attached to it. When the user clicks on the p element, a function called myFunction() is executed, which changes the style of the div with id="panel" from display:none (hidden) to display:block (visible).</p>
            <p>You will learn more about JavaScript in our JavaScript Tutorial.</p>
        </div>

        <script>
            function myFunction() {
                document.getElementById("panel").style.display = "block";
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Display/Example_5.html)