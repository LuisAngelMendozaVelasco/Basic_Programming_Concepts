# Syntax

## JavaScript statements

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Statements</h2>

        <p>A <b>JavaScript program</b> is a list of <b>statements</b> to be executed by a computer.</p>

        <p id="demo"></p>

        <script>
            var x, y, z;    // Declare 3 variables
            x = 5;          // Assign the value 5 to x
            y = 6;          // Assign the value 6 to y
            z = x + y;      // Assign the sum of x and y to z

            document.getElementById("demo").innerHTML = "The value of z is " + z + ".";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_1.html)

## JavaScript numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Number can be written with or without decimals.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = 10.50;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_2.html)

## JavaScript strings

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Strings</h2>

        <p>Strings can be written with double or single quotes.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = 'John Doe';
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_3.html)

## JavaScript variables

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Variables</h2>

        <p>
            In this example, x is defined as a variable.
            Then, x is assigned the value of 6:
        </p>

        <p id="demo"></p>

        <script>
            let x;
            x = 6;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_4.html)

## JavaScript operators

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Operators</h2>

        <p>JavaScript uses arithmetic operators to compute values (just like algebra).</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = (5 + 6) * 10;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_5.html)

## JavaScript assignment

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Assigning JavaScript Values</h2>

        <p>In JavaScript the = operator is used to assign values to variables.</p>

        <p id="demo"></p>

        <script>
            let x, y;
            x = 5;
            y = 6;

            document.getElementById("demo").innerHTML = x + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_6.html)

## JavaScript expressions (using constants)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Expressions</h2>

        <p>Expressions compute to values.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = 5 * 10;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_7.html)

## JavaScript expressions (using strings)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Expressions</h2>

        <p>Expressions compute to values.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "John" + " "  + "Doe";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_8.html)

## JavaScript expressions (using variables)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Expressions</h2>

        <p>Expressions compute to values.</p>

        <p id="demo"></p>

        <script>
            var x;
            x = 5;
            
            document.getElementById("demo").innerHTML = x * 10;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_9.html)

## JavaScript keywords

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The var Keyword Creates Variables</h2>

        <p id="demo"></p>

        <script>
            var x, y;
            x = 5 + 6;
            y = x * 10;

            document.getElementById("demo").innerHTML = y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_10.html)

## JavaScript comments

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Comments are NOT Executed</h2>

        <p id="demo"></p>

        <script>
            let x;
            x = 5;
            // x = 6; I will not be executed
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_11.html)

## JavaScript is case sensitive

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript is Case Sensitive</h2>

        <p>Try to change lastName to lastname.</p>

        <p id="demo"></p>

        <script>
            let lastname, lastName;
            lastName = "Doe";
            lastname = "Peterson";
            
            document.getElementById("demo").innerHTML = lastName;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Syntax/Example_12.html)