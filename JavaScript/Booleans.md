# Booleans

## Display the value of Boolean(10 > 9)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p>Display the value of Boolean(10 > 9):</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Boolean(10 > 9);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_1.html)

## Display the value of 10 > 9

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p>Display the value of 10 > 9:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = 10 > 9;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_2.html)

## Everything with a real value is true

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "100 is " + Boolean(100) + "<br>" +
                                                        "3.14 is " + Boolean(3.14) + "<br>" +
                                                        "-15 is " + Boolean(-15) + "<br>" +
                                                        "Any (not empty) string is " + Boolean("Hello") + "<br>" +
                                                        "Even the string 'false' is " + Boolean('false') + "<br>" +
                                                        "Any expression (except zero) is " + Boolean(1 + 7 + 3.14);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_3.html)

## The Boolean value of zero is false

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p>Display the Boolean value of 0:</p>

        <p id="demo"></p>

        <script>
            let x = 0;
            
            document.getElementById("demo").innerHTML = Boolean(x);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_4.html)

## The Boolean value of minus zero is false

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p>Display the Boolean value of -0:</p>

        <p id="demo"></p>

        <script>
            let x = -0;

            document.getElementById("demo").innerHTML = Boolean(x);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_5.html)

## The Boolean value of an empty string is false

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p>Display the Boolean value of "":</p>

        <p id="demo"></p>

        <script>
            let x = "";
            
            document.getElementById("demo").innerHTML = Boolean("");
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_6.html)

## The Boolean value of undefined is false

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p>Display the Boolean value of undefined:</p>

        <p id="demo"></p>

        <script>
            let x;
            
            document.getElementById("demo").innerHTML = Boolean(x);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_7.html)

## The Boolean value of null is false

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p>Display the Boolean value of null:</p>

        <p id="demo"></p>

        <script>
            let x = null;
            
            document.getElementById("demo").innerHTML = Boolean(x);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_8.html)

## The Boolean value of false is false

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p>Display the Boolean value of false:</p>

        <p id="demo"></p>

        <script>
            let x = false;
            
            document.getElementById("demo").innerHTML = Boolean(x);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_9.html)

## The Boolean value of NaN is false

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Booleans</h2>
        <p>Display the Boolean value of NaN:</p>

        <p id="demo"></p>

        <script>
            let x = 10 / "Hello";
            
            document.getElementById("demo").innerHTML = Boolean(x);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Booleans/Example_10.html)