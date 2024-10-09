# Gradients

## Linear Gradient - top to bottom

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(red, yellow);}
        </style>
    </head>
    <body>
        <h1>Linear Gradient - Top to Bottom</h1>
        <p>This linear gradient starts red at the top, transitioning to yellow at the bottom:</p>

        <div id="grad1"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_1.html)

## Linear Gradient - left to right

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(to right, red , yellow);}
        </style>
    </head>
    <body>
        <h1>Linear Gradient - Left to Right</h1>
        <p>This linear gradient starts red at the left, transitioning to yellow (to the right):</p>

        <div id="grad1"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_2.html)

## Linear Gradient - diagonal

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(to bottom right, red, yellow);}
        </style>
    </head>
    <body>
        <h1>Linear Gradient - Diagonal</h1>
        <p>This linear gradient starts red at top left, transitioning to yellow (at bottom right):</p>

        <div id="grad1"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_3.html)

## Linear Gradient - with a specified angle

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 100px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(0deg, red, yellow);}

            #grad2 {height: 100px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(90deg, red, yellow);}

            #grad3 {height: 100px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(180deg, red, yellow);}

            #grad4 {height: 100px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(-90deg, red, yellow);}
        </style>
    </head>
    <body>
        <h1>Linear Gradients - Using Different Angles</h1>

        <div id="grad1" style="text-align:center;">0deg</div><br>
        <div id="grad2" style="text-align:center;">90deg</div><br>
        <div id="grad3" style="text-align:center;">180deg</div><br>
        <div id="grad4" style="text-align:center;">-90deg</div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_4.html)

## Linear Gradient - with multiple color stops

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(red, yellow, green);}

            #grad2 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(red, orange, yellow, green, blue, indigo, violet);}

            #grad3 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(red 10%, green 85%, blue 90%);}
        </style>
    </head>
    <body>
        <h1>Linear Gradients - Multiple Color Stops</h1>
        <p><strong>Note:</strong> Color stops are spaced evenly when no percents are specified.</p>

        <h2>3 Color Stops (evenly spaced):</h2>
        <div id="grad1"></div>

        <h2>7 Color Stops (evenly spaced):</h2>
        <div id="grad2"></div>

        <h2>3 Color Stops (not evenly spaced):</h2>
        <div id="grad3"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_5.html)

## Linear Gradient - color of a rainbow + text

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 55px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: linear-gradient(to right, red, orange, yellow, green, blue, indigo, violet);}
        </style>
    </head>
    <body>
        <div id="grad1" style="text-align:center;margin:auto;color:#888888;font-size:40px;font-weight:bold">
            Rainbow Background
        </div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_6.html)

## Linear Gradient - with transparency

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 200px;
                    background-image: linear-gradient(to right, rgba(255,0,0,0), rgba(255,0,0,1));}
        </style>
    </head>
    <body>
        <h1>Linear Gradient - Transparency</h1>
        <p>To add transparency, we use the rgba() function to define the color stops. The last parameter in the rgba() function can be a value from 0 to 1, and it defines the transparency of the color: 0 indicates full transparency, 1 indicates full color (no transparency).</p>

        <div id="grad1"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_7.html)

## Linear Gradient - a repeating linear gradient

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: repeating-linear-gradient(red, yellow 10%, green 20%);}

            #grad2 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: repeating-linear-gradient(45deg,red,yellow 7%,green 10%);}

            #grad3 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: repeating-linear-gradient(190deg,red,yellow 7%,green 10%);}

            #grad4 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: repeating-linear-gradient(90deg,red,yellow 7%,green 10%);}

            #grad5 {height: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: repeating-linear-gradient(45deg, red 0px, red 10px, red 10px, yellow 10px, yellow 20px);}
        </style>
    </head>
    <body>
        <h1>Repeating Linear Gradient</h1>

        <div id="grad1"></div>

        <p>A repeating gradient on 45deg axe starting red and finishing green:</p>
        <div id="grad2"></div>

        <p>A repeating gradient on 190deg axe starting red and finishing green:</p>
        <div id="grad3"></div>

        <p>A repeating gradient on 90deg axe starting red and finishing green:</p>
        <div id="grad4"></div>

        <p>A repeating linear gradient with solid stripes:</p>
        <div id="grad5"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_8.html)

## Radial Gradient - evenly spaced color stops

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 150px;
                    width: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: radial-gradient(red, yellow, green);}
        </style>
    </head>
    <body>
        <h1>Radial Gradient - Evenly Spaced Color Stops</h1>

        <div id="grad1"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_9.html)

## Radial Gradient - differently spaced color stops

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 150px;
                    width: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: radial-gradient(red 5%, yellow 15%, green 60%);}
        </style>
    </head>
    <body>
        <h1>Radial Gradient - Differently Spaced Color Stops</h1>

        <div id="grad1"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_10.html)

## Radial Gradient - set shape

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 150px;
                    width: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: radial-gradient(red, yellow, green);}

            #grad2 {height: 150px;
                    width: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: radial-gradient(circle, red, yellow, green);}
        </style>
    </head>
    <body>
        <h1>Radial Gradient - Shapes</h1>

        <h2>Ellipse (this is default):</h2>
        <div id="grad1"></div>

        <h2><strong>Circle:</strong></h2>
        <div id="grad2"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_11.html)

## Radial Gradient - different size keywords

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 150px;
                    width: 150px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: radial-gradient(closest-side at 60% 55%, red, yellow, black);}

            #grad2 {height: 150px;
                    width: 150px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: radial-gradient(farthest-side at 60% 55%, red, yellow, black);}

            #grad3 {height: 150px;
                    width: 150px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: radial-gradient(closest-corner at 60% 55%, red, yellow, black);}

            #grad4 {height: 150px;
                    width: 150px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: radial-gradient(farthest-corner at 60% 55%, red, yellow, black);}
        </style>
    </head>
    <body>
        <h1>Radial Gradients - Different size keywords</h1>

        <h2>closest-side:</h2>
        <div id="grad1"></div>

        <h2>farthest-side:</h2>
        <div id="grad2"></div>

        <h2>closest-corner:</h2>
        <div id="grad3"></div>

        <h2>farthest-corner (default):</h2>
        <div id="grad4"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_12.html)

## Radial Gradient - a repeating radial gradient

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #grad1 {height: 150px;
                    width: 200px;
                    background-color: red; /* For browsers that do not support gradients */
                    background-image: repeating-radial-gradient(red, yellow 10%, green 15%);}
        </style>
    </head>
    <body>
        <h1>Repeating Radial Gradient</h1>

        <div id="grad1"></div>
    </body>
</html>
```

Output:

[Click here!](./Gradients/Example_13.html)