# Arrays

## Create an array I

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Arrays</h2>

        <p id="demo"></p>

        <script>
            const cars = ["Saab", "Volvo", "BMW"];
            
            document.getElementById("demo").innerHTML = cars;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_1.html)

## Create an array II

Code: 

```html
<!DOCTYPE html>
<html>
    <body>

        <h2>JavaScript Arrays</h2>

        <p id="demo"></p>

        <script>
            const cars = [  "Saab",
                            "Volvo",
                            "BMW"];
                            
            document.getElementById("demo").innerHTML = cars;
        </script>

    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_2.html)

## Access an array element

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Arrays</h2>

        <p>JavaScript array elements are accessed using numeric indexes (starting from 0).</p>

        <p id="demo"></p>

        <script>
            const cars = ["Saab", "Volvo", "BMW"];
            
            document.getElementById("demo").innerHTML = cars[0];
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_3.html)

## Change an array element

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2>
        <p>Array elements are accessed using their index number:</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            
            document.getElementById("demo1").innerHTML = fruits;
            fruits[0] = "Kiwi";
            document.getElementById("demo2").innerHTML = fruits;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_4.html)

## Access a full array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Arrays</h2>

        <p id="demo"></p>

        <script>
            const cars = ["Saab", "Volvo", "BMW"];
            
            document.getElementById("demo").innerHTML = cars;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_5.html)

## Find the length of an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Arrays</h2>
        <p>The length property returns the length of an array.</p>

        <p id="demo"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            
            document.getElementById("demo").innerHTML = fruits.length;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_6.html)

## Loop through an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Arrays</h2>

        <p>The best way to loop through an array is using a standard for loop:</p>

        <p id="demo"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            let fLen = fruits.length;
            let text = "<ul>";

            for (let i = 0; i < fLen; i++) {
                text += "<li>" + fruits[i] + "</li>";
            }

            text += "</ul>";
            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_7.html)

## Add an element to an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Arrays</h2>

        <p>The length property provides an easy way to append new elements to an array without using the push() method.</p>

        <button onclick="myFunction()">Try it</button>

        <p id="demo"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple"];
            
            document.getElementById("demo").innerHTML = fruits;

            function myFunction() {
                fruits[fruits.length] = "Lemon";
                document.getElementById("demo").innerHTML = fruits;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_8.html)

## Add undefined "holes" to an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Arrays</h2>

        <p>Adding elements with high indexes can create undefined "holes" in an array.</p>

        <p id="demo"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple"];
            
            fruits[6] = "Lemon";

            let fLen = fruits.length;
            let text = "";
            
            for (i = 0; i < fLen; i++) {
                text += fruits[i] + "<br>";
            }

            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_9.html)

## How to recognize an array I

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Arrays</h2>

        <p>The instanceof operator returns true when used on an array:</p>

        <p id="demo"></p>

        <script>
            var fruits = ["Banana", "Orange", "Apple"];
            
            document.getElementById("demo").innerHTML = fruits instanceof Array;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_10.html)

## How to recognize an array II

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Arrays</h1>
        <h2>The isArray() Method</h2>

        <p id="demo"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple"];
            
            document.getElementById("demo").innerHTML = Array.isArray(fruits);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Arrays/Example_11.html)