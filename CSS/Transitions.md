# Transitions

## Transition - change width of an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background: red;
                    transition: width 2s;}

            div:hover {width: 300px;}
        </style>
    </head>
    <body>
        <h1>The transition Property</h1>

        <p>Hover over the div element below, to see the transition effect:</p>
        <div></div>
    </body>
</html>
```

Output:

[Click here!](./Transitions/Example_1.html)

## Transition - change width and height of an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background: red;
                    transition: width 2s, height 4s;}

            div:hover { width: 300px;
                        height: 300px;}
        </style>
    </head>
    <body>
        <h1>The transition Property</h1>

        <p>Hover over the div element below, to see the transition effect:</p>

        <div></div>
    </body>
</html>
```

Output:

[Click here!](./Transitions/Example_2.html)

## Specify different speed curves for a transition

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background: red;
                    transition: width 2s;}

            #div1 {transition-timing-function: linear;}
            #div2 {transition-timing-function: ease;}
            #div3 {transition-timing-function: ease-in;}
            #div4 {transition-timing-function: ease-out;}
            #div5 {transition-timing-function: ease-in-out;}

            div:hover {width: 300px;}
        </style>
    </head>
    <body>
        <h1>The transition-timing-function Property</h1>

        <p>Hover over the div elements below, to see the different speed curves:</p>

        <div id="div1">linear</div><br>
        <div id="div2">ease</div><br>
        <div id="div3">ease-in</div><br>
        <div id="div4">ease-out</div><br>
        <div id="div5">ease-in-out</div><br>
    </body>
</html>
```

Output:

[Click here!](./Transitions/Example_3.html)

## Specify a delay for a transition effect

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background: red;
                    transition: width 3s;
                    transition-delay: 1s;}

            div:hover {width: 300px;}
        </style>
    </head>
    <body>
        <h1>The transition-delay Property</h1>

        <p>Hover over the div element below, to see the transition effect:</p>

        <div></div>

        <p><b>Note:</b> The transition effect has a 1 second delay before starting.</p>
    </body>
</html>
```

Output:

[Click here!](./Transitions/Example_4.html)

## Add a transformation to a transition effect

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background: red;
                    transition: width 2s, height 2s, transform 2s;}

            div:hover { width: 300px;
                        height: 300px;
                        transform: rotate(180deg);}
        </style>
    </head>
    <body>
        <h1>Transition + Transform</h1>

        <p>Hover over the div element below:</p>

        <div></div>
    </body>
</html>
```

Output:

[Click here!](./Transitions/Example_5.html)

## Specify all transition properties in one shorthand property

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background: red;
                    transition: width 2s linear 1s;}

            div:hover {width: 300px;}
        </style>
    </head>
    <body>
        <h1>Using The transition Shorthand Property</h1>

        <p>Hover over the div element below, to see the transition effect:</p>

        <div></div>

        <p><b>Note:</b> The transition effect has a 1 second delay before starting.</p>
    </body>
</html>
```

Output:

[Click here!](./Transitions/Example_6.html)