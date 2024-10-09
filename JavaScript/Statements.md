# Statements

## JavaScript statements are commands to the browser

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Statements</h2>

        <p>In HTML, JavaScript statements are executed by the browser.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "Hello Dolly.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Statements/Example_1.html)

## JavaScript code is a sequence of statements

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Statements</h2>

        <p>A <b>JavaScript program</b> is a list of <b>statements</b> to be executed by a computer.</p>

        <p id="demo"></p>

        <script>
            let x, y, z;  // Statement 1
            x = 5;        // Statement 2
            y = 6;        // Statement 3
            z = x + y;    // Statement 4

            document.getElementById("demo").innerHTML = "The value of z is " + z + ".";  
        </script>
    </body>
</html>
```

Output:

[Click here!](./Statements/Example_2.html)

## JavaScript statements are separated with semicolon

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Statements</h2>

        <p>JavaScript statements are separated by semicolons.</p>

        <p id="demo1"></p>

        <script>
            let a, b, c;
            a = 5;
            b = 6;
            c = a + b;

            document.getElementById("demo1").innerHTML = c;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Statements/Example_3.html)

## Multiple statement on one line is allowed

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Statements</h2>

        <p>Multiple statements on one line are allowed.</p>

        <p id="demo1"></p>

        <script>
            let a, b, c;
            a = 5; b = 6; c = a + b;
            
            document.getElementById("demo1").innerHTML = c;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Statements/Example_4.html)

## JavaScript statements can be grouped together in code blocks

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Statements</h2>

        <p>JavaScript code blocks are written between { and }</p>

        <button type="button" onclick="myFunction()">Click Me!</button>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            function myFunction() {
                document.getElementById("demo1").innerHTML = "Hello Dolly!";
                document.getElementById("demo2").innerHTML = "How are you?";
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Statements/Example_5.html)

## You can break a code line after an operator or a comma

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Statements</h2>

        <p>
            The best place to break a code line is after an operator or a comma.
        </p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML =
            "Hello Dolly!";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Statements/Example_6.html)