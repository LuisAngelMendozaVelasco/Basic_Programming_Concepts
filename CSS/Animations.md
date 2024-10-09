# Animations

## Bind an animation to an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background-color: red;
                    animation-name: example;
                    animation-duration: 4s;}

            @keyframes example {from {background-color: red;}
                                to {background-color: yellow;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <div></div>

        <p><b>Note:</b> When an animation is finished, it goes back to its original style.</p>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_1.html)

## Animation - change background-color of an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div {   width: 100px;
                    height: 100px;
                    background-color: red;
                    animation-name: example;
                    animation-duration: 4s;}

            @keyframes example {0%   {background-color: red;}
                                25%  {background-color: yellow;}
                                50%  {background-color: blue;}
                                100% {background-color: green;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <div></div>

        <p><b>Note:</b> When an animation is finished, it goes back to its original style.</p>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_2.html)

## Animation - change background-color and position of an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background-color: red;
                    position: relative;
                    animation-name: example;
                    animation-duration: 4s;}

            @keyframes example {0%   {background-color:red; left:0px; top:0px;}
                                25%  {background-color:yellow; left:200px; top:0px;}
                                50%  {background-color:blue; left:200px; top:200px;}
                                75%  {background-color:green; left:0px; top:200px;}
                                100% {background-color:red; left:0px; top:0px;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <div></div>

        <p><b>Note:</b> When an animation is finished, it goes back to its original style.</p>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_3.html)

## Delay an animation

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background-color: red;
                    position: relative;
                    animation-name: example;
                    animation-duration: 4s;
                    animation-delay: 2s;}

            @keyframes example {0%   {background-color:red; left:0px; top:0px;}
                                25%  {background-color:yellow; left:200px; top:0px;}
                                50%  {background-color:blue; left:200px; top:200px;}
                                75%  {background-color:green; left:0px; top:200px;}
                                100% {background-color:red; left:0px; top:0px;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <p>The animation-delay property specifies a delay for the start of an animation. The following example has a 2 seconds delay before starting the animation:</p>

        <div></div>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_4.html)

## Run animation 3 times before it stops

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background-color: red;
                    position: relative;
                    animation-name: example;
                    animation-duration: 4s;
                    animation-iteration-count: 3;}

            @keyframes example {0%   {background-color:red; left:0px; top:0px;}
                                25%  {background-color:yellow; left:200px; top:0px;}
                                50%  {background-color:blue; left:200px; top:200px;}
                                75%  {background-color:green; left:0px; top:200px;}
                                100% {background-color:red; left:0px; top:0px;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <p>The animation-iteration-count property specifies the number of times an animation should run. The following example will run the animation 3 times before it stops:</p>

        <div></div>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_5.html)

## Run animation for ever

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background-color: red;
                    position: relative;
                    animation-name: example;
                    animation-duration: 4s;
                    animation-iteration-count: infinite;}

            @keyframes example {0%   {background-color:red; left:0px; top:0px;}
                                25%  {background-color:yellow; left:200px; top:0px;}
                                50%  {background-color:blue; left:200px; top:200px;}
                                75%  {background-color:green; left:0px; top:200px;}
                                100% {background-color:red; left:0px; top:0px;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <p>The animation-iteration-count property can be set to infinite to let the animation run for ever:</p>

        <div></div>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_6.html)

## Run animation in reverse direction

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background-color: red;
                    position: relative;
                    animation-name: example;
                    animation-duration: 4s;
                    animation-direction: reverse;}

            @keyframes example {0%   {background-color:red; left:0px; top:0px;}
                                25%  {background-color:yellow; left:200px; top:0px;}
                                50%  {background-color:blue; left:200px; top:200px;}
                                75%  {background-color:green; left:0px; top:200px;}
                                100% {background-color:red; left:0px; top:0px;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <p>The animation-direction property specifies whether an animation should be played forwards, backwards or in alternate cycles. The following example will run the animation in reverse direction (backwards):</p>

        <div></div>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_7.html)

## Run animation in alternate cycles

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background-color: red;
                    position: relative;
                    animation-name: example;
                    animation-duration: 4s;
                    animation-iteration-count: 2;
                    animation-direction: alternate;}

            @keyframes example {0%   {background-color:red; left:0px; top:0px;}
                                25%  {background-color:yellow; left:200px; top:0px;}
                                50%  {background-color:blue; left:200px; top:200px;}
                                75%  {background-color:green; left:0px; top:200px;}
                                100% {background-color:red; left:0px; top:0px;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <p>The animation-direction property specifies whether an animation should be played forwards, backwards or in alternate cycles. The following example uses the value "alternate" to make the animation run forwards first, then backwards:</p>

        <div></div>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_8.html)

## Speed curves for animations

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 50px;
                    background-color: red;
                    font-weight: bold;
                    position: relative;
                    animation: mymove 5s infinite;}

            #div1 {animation-timing-function: linear;}
            #div2 {animation-timing-function: ease;}
            #div3 {animation-timing-function: ease-in;}
            #div4 {animation-timing-function: ease-out;}
            #div5 {animation-timing-function: ease-in-out;}

            @keyframes mymove { from {left: 0px;}
                                to {left: 300px;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <p>The animation-timing-function property specifies the speed curve of the animation. The following example shows some of the different speed curves that can be used:</p>

        <div id="div1">linear</div>
        <div id="div2">ease</div>
        <div id="div3">ease-in</div>
        <div id="div4">ease-out</div>
        <div id="div5">ease-in-out</div>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_9.html)

## Animation shorthand property

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   width: 100px;
                    height: 100px;
                    background-color: red;
                    position: relative;
                    animation: myfirst 5s linear 2s infinite alternate;}

            @keyframes myfirst {0%   {background-color:red; left:0px; top:0px;}
                                25%  {background-color:yellow; left:200px; top:0px;}
                                50%  {background-color:blue; left:200px; top:200px;}
                                75%  {background-color:green; left:0px; top:200px;}
                                100% {background-color:red; left:0px; top:0px;}}
        </style>
    </head>
    <body>
        <h1>CSS Animation</h1>

        <p>This example uses the shorthand animation property:</p>

        <div></div>
    </body>
</html>
```

Output:

[Click here!](./Animations/Example_10.html)