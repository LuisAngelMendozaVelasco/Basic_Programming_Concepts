# Random

## Math.random() returns a random number between 0 (included) and 1 (excluded)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.random()</h2>

        <p>Math.random() returns a random number between 0 (included) and 1 (excluded):</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.random();
        </script>
    </body>
</html>
```

Output:

[Click here!](./Random/Example_1.html)

## How to return a random integer between 0 and 9 (both included)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math</h2>

        <p>Math.floor(Math.random() * 10) returns a random integer between 0 and 9 (both included):</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.floor(Math.random() * 10);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Random/Example_2.html)

## How to return a random integer between 0 and 10 (both included)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math</h2>

        <p>Math.floor(Math.random() * 11) returns a random integer between 0 and 10 (both included):</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.floor(Math.random() * 11);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Random/Example_3.html)

## How to return a random integer between 0 and 99 (both included)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math</h2>

        <p>Math.floor(Math.random() * 100)) returns a random integer between 0 and 99 (both included):</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.floor(Math.random() * 100);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Random/Example_4.html)

## How to return a random integer between 0 and 100 (both included)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math</h2>

        <p>Math.floor() used with Math.random() * 101 returns a random integer between 0 and 100 (both included):</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.floor(Math.random() * 101);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Random/Example_5.html)

## How to return a random integer between 1 and 10 (both included)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math</h2>

        <p>Math.floor(Math.random() * 10) + 1) returns a random integer between 1 and 10 (both included):</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.floor(Math.random() * 10) + 1;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Random/Example_6.html)

## How to return a random integer between 1 and 100 (both included)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math</h2>

        <p>Math.floor(Math.random() * 100) + 1) returns a random integer between 1 and 100 (both included):</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Math.floor(Math.random() * 100) + 1;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Random/Example_7.html)

## How to return a random integer between x (included) and y (excluded)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.random()</h2>

        <p>Every time you click the button, getRndInteger(min, max) returns a random number between 0 and 9 (both included):</p>

        <button onclick="document.getElementById('demo').innerHTML = getRndInteger(0, 10)">Click Me</button>

        <p id="demo"></p>

        <script>
            function getRndInteger(min, max) {
                return Math.floor(Math.random() * (max - min)) + min;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Random/Example_8.html)

## How to return a random integer between x and y (both included)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.random()</h2>

        <p>Every time you click the button, getRndInteger(min, max) returns a random number between 1 and 10 (both included):</p>

        <button onclick="document.getElementById('demo').innerHTML = getRndInteger(1, 10)">Click Me</button>

        <p id="demo"></p>

        <script>
            function getRndInteger(min, max) {
                return Math.floor(Math.random() * (max - min + 1)) + min;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Random/Example_9.html)