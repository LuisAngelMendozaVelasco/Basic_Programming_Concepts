# Variables

## JavaScript variables

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>In this example, x, y, and z are variables.</p>

        <p id="demo"></p>

        <script>
            var x = 5;
            var y = 6;
            var z = x + y;
            
            document.getElementById("demo").innerHTML = "The value of z is: " + z;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_1.html)

## JavaScript variables as algebra

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>In this example, price1, price2, and total are variables.</p>

        <p id="demo"></p>

        <script>
            const price1 = 5;
            const price2 = 6;
            let total = price1 + price2;
            
            document.getElementById("demo").innerHTML = "The total is: " + total;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_2.html)

## JavaScript numbers and strings

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>Strings are written with quotes.</p>
        <p>Numbers are written without quotes.</p>

        <p id="demo"></p>

        <script>
            const pi = 3.14;
            let person = "John Doe";
            let answer = 'Yes I am!';

            document.getElementById("demo").innerHTML = pi + "<br>" + person + "<br>" + answer;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_3.html)

## JavaScript var keyword.

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>Create a variable, assign a value to it, and display it:</p>

        <p id="demo"></p>

        <script>
            let carName = "Volvo";
            
            document.getElementById("demo").innerHTML = carName;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_4.html)

## Declaring many variables in one statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>You can declare many variables in one statement.</p>

        <p id="demo"></p>

        <script>
            let person = "John Doe", carName = "Volvo", price = 200;
            
            document.getElementById("demo").innerHTML = carName;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_5.html)

## Declaring many variables multiline

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>You can declare many variables in one statement.</p>

        <p id="demo"></p>

        <script>
            let person = "John Doe",
            carName = "Volvo",
            price = 200;
            
            document.getElementById("demo").innerHTML = carName;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_6.html)

## A variable without a value returns the value undefined

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>A variable without a value has the value of:</p>
        <p id="demo"></p>

        <script>
            let carName;
            
            document.getElementById("demo").innerHTML = carName;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_7.html)

## Re-declaring a variable will not destroy the value

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>If you re-declare a JavaScript variable, it will not lose its value.</p>

        <p id="demo"></p>

        <script>
            var carName = "Volvo";
            var carName;
            
            document.getElementById("demo").innerHTML = carName;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_8.html)

## Adding JavaScript numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>The result of adding 5 + 2 + 3 is:</p>
        <p id="demo"></p>

        <script>
            let x = 5 + 2 + 3;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_9.html)

## Adding JavaScript strings

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>The result of adding "John" + " " + "Doe" is:</p>
        <p id="demo"></p>

        <script>
            let x = "John" + " " + "Doe";
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_10.html)

## Adding strings and numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Variables</h1>

        <p>The result of adding "5" + 2 + 3 is:</p>
        <p id="demo"></p>

        <script>
            let x = "5" + 2 + 3;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Variables/Example_11.html)