# Functions

## A simple function

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <script>
            function myFunction() {
                document.getElementById("demo").innerHTML = "Hello World!";
            }
        </script>
    </head>
    <body>
        <p>When you click "Try it", a function will be called.</p>
        <p>The function will display a message.</p>

        <button onclick="myFunction()">Try it</button>

        <p id="demo"></p>
    </body>
</html>
```

Output:

[Click here!](./Functions/Example_1.html)

## A function with an argument

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Click "Try it" to call a function with arguments</p>

        <button onclick="myFunction('Harry Potter', 'Wizard')">Try it</button>

        <p id="demo"></p>

        <script>
            function myFunction(name, job) {
                document.getElementById("demo").innerHTML = "Welcome " + name + ", the " + job + ".";
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Functions/Example_2.html)

## A function with an argument 2

Code: 

```html
<!DOCTYPE html>
<html> 
    <head> 
        <script> 
            function myfunction(txt) { 
                document.getElementById("demo").innerHTML = txt
            } 
        </script> 
    </head> 
    <body> 
        <p>When you click on one of the buttons, a function will be called. The function will display the argument that is passed to it.</p>

        <form> 
            <input type="button" onclick="myfunction('Good Morning!')" value="In the Morning"> 
            <input type="button" onclick="myfunction('Good Evening!')" value="In the Evening"> 
        </form> 

        <p id="demo"></p>
    </body> 
</html> 
```

Output:

[Click here!](./Functions/Example_3.html)

## A function that returns a value

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Functions</h2>

        <p>This example calls a function which performs a calculation and returns the result:</p>

        <p id="demo"></p>

        <script>
            var x = myFunction(4, 3);
            
            document.getElementById("demo").innerHTML = x;

            function myFunction(a, b) {
                return a * b;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Functions/Example_4.html)

## A function that converts Fahrenheit to Celsius

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Functions</h2>

        <p>This example calls a function to convert from Fahrenheit to Celsius:</p>
        <p id="demo"></p>

        <script>
            function toCelsius(f) {
                return (5/9) * (f-32);
            }
            document.getElementById("demo").innerHTML = toCelsius(77);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Functions/Example_5.html)

## A function call without ()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Functions</h2>

        <p>Accessing a function without () will return the function definition instead of the function result:</p>
        <p id="demo"></p>

        <script>
            function toCelsius(f) {
                return (5/9) * (f-32);
            }
            document.getElementById("demo").innerHTML = toCelsius;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Functions/Example_6.html)