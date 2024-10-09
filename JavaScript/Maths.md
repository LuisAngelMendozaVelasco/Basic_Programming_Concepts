# Maths

## Math.PI returns the value of PI

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.PI</h2>

        <p>Math.PI returns the ratio of a circle's circumference to its diameter:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.PI;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_1.html)

## Math.round(x) returns the rounded value of x

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.round()</h2>

        <p>Math.round(x) returns the value of x rounded to its nearest integer:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.round(4.5);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_2.html)

## Math.pow(x, y) returns the value of x to the power of y

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.pow()</h2>

        <p>Math.pow(x, y) returns the value of x to the power of y:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.pow(8, 2);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_3.html)

## Math.sqrt(x) returns the square root of x

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.sqrt()</h2>

        <p>Math.sqrt(x) returns the square root of x:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.sqrt(64);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_4.html)

## Math.abs(x) returns the absolute (positive) value of x

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.abs()</h2>

        <p>Math.abs(x) returns the absolute (positive) value of x:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.abs(-4.7);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_5.html)

## Math.ceil(x) returns the value of x rounded up

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.ceil()</h2>

        <p>Math.ceil() rounds a number <strong>up</strong> to its nearest integer:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.ceil(4.4);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_6.html)

## Math.floor(x) returns the value of x rounded down

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.floor()</h2>

        <p>Math.floor(x) returns the value of x rounded <strong>down</strong> to its nearest integer:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.floor(4.7);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_7.html)

## Math.sin(x) returns the sin of the angle x (given in radians)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.sin()</h2>

        <p>Math.sin(x) returns the sin of x (given in radians):</p>
        <p>Angle in radians = (angle in degrees) * PI / 180.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "The sine value of 90 degrees is " + Math.sin(90 * Math.PI / 180);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_8.html)

## Math.cos(x) returns the cosin of the angle x (given in radians)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.cos()</h2>

        <p>Math.cos(x) returns the cosine of x (given in radians):</p>
        <p>Angle in radians = (angle in degrees) * PI / 180.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "The cosine value of 0 degrees is " + Math.cos(0 * Math.PI / 180);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_9.html)

## Math.max() return the number with the highest value from a list of arguments

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.max()</h2>

        <p>Math.max() returns the highest value in a list of arguments.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.max(0, 150, 30, 20, -8, -200);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_10.html)

## Math.min() to return the number with the lowest value from a list of arguments

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.min()</h2>

        <p>Math.min() returns the lowest value in a list of arguments:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.min(0, 150, 30, 20, -8, -200);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_11.html)

## Converting Celsius to Fahrenheit

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Celcius to Fahrenhet</h2>

        <p>Insert a number into one of the input fields below:</p>

        <p><input id="c" onkeyup="convert('C')"> degrees Celsius</p>

        <p><input id="f" onkeyup="convert('F')"> degrees Fahrenheit</p> 

        <p>Note that the <b>Math.round()</b> method is used, so that the result will be returned as an integer.</p>

        <script>
            function convert(degree) {
                var x;
                
                if (degree == "C") {
                    x = document.getElementById("c").value * 9 / 5 + 32;
                    document.getElementById("f").value = Math.round(x);
                } 
                else {
                    x = (document.getElementById("f").value - 32) * 5 / 9;
                    document.getElementById("c").value = Math.round(x);
                }
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Maths/Example_12.html)