# Data Types

## Declare (create) strings

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Strings</h2>

        <p>You can use quotes inside a string, as long as they don't match the quotes surrounding the string:</p>

        <p id="demo"></p>

        <script>
            let answer1 = "It's alright";
            let answer2 = "He is called 'Johnny'";
            let answer3 = 'He is called "Johnny"';

            document.getElementById("demo").innerHTML = answer1 + "<br>" + 
                                                        answer2 + "<br>" + 
                                                        answer3;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Data_Types/Example_1.html)

## Declare (create) numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Numbers can be written with, or without decimals:</p>

        <p id="demo"></p>

        <script>
            let x1 = 34.00;
            let x2 = 34;
            let x3 = 3.14;

            document.getElementById("demo").innerHTML = x1 + "<br>" + x2 + "<br>" + x3;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Data_Types/Example_2.html)

## Declare (create) an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Arrays</h2>

        <p>Array indexes are zero-based, which means the first item is [0].</p>

        <p id="demo"></p>

        <script>
            const cars = ["Saab", "Volvo", "BMW"];

            document.getElementById("demo").innerHTML = cars[0];
        </script>
    </body>
</html>
```

Output:

[Click here!](./Data_Types/Example_3.html)

## Declare (create) an object

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>

        <p id="demo"></p>

        <script>
            const person = {firstName   : "John",
                            lastName    : "Doe",
                            age         : 50,
                            eyeColor    : "blue"};

            document.getElementById("demo").innerHTML = person.firstName + " is " + person.age + " years old.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Data_Types/Example_4.html)

## Find the type of a variable

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Operators</h1>
        <h2>The typeof Operator</h2>
        <p>The typeof operator returns the type of a variable or an expression.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = typeof "" + "<br>" +
                                                        typeof "John" + "<br>" + 
                                                        typeof "John Doe" + "<br>" +
                                                        typeof 0 + "<br>" +
                                                        typeof 314 + "<br>" +
                                                        typeof 3.14 + "<br>" +
                                                        typeof (3.14);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Data_Types/Example_5.html)

## Adding two numbers and a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript</h2>

        <p>JavaScript evaluates expressions from left to right. Different sequences can produce different results:</p>

        <p id="demo"></p>

        <script>
            let x = 16 + 4 + "Volvo";
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Data_Types/Example_6.html)

## Adding a string and two numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript</h2>

        <p>JavaScript evaluates expressions from left to right. Different sequences can produce different results:</p>

        <p id="demo"></p>

        <script>
            let x = "Volvo" + 16 + 4;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Data_Types/Example_7.html)

## An undefined variable

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Operators</h1>
        <h2>The typeof Operator</h2>
        <p>The value (and the data type) of a variable with no value is <b>undefined</b>.</p>

        <p id="demo"></p>

        <script>
            let car;
            
            document.getElementById("demo").innerHTML = car + "<br>" + typeof car;
        </script>
    </body>
</html> 
```

Output:

[Click here!](./Data_Types/Example_8.html)

## An empty variable

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript</h2>

        <p>An empty string has both a legal value and a type:</p>

        <p id="demo"></p>

        <script>
            let car = "";
            
            document.getElementById("demo").innerHTML = "The value is: " +
                                                        car + "<br>" +
                                                        "The type is: " + typeof car;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Data_Types/Example_9.html)