# Comments

## Single line comments

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1 id="myH"></h1>
        <p id="myP"></p>

        <script>
            // Change heading:
            document.getElementById("myH").innerHTML = "JavaScript Comments";
            // Change paragraph:
            document.getElementById("myP").innerHTML = "My first paragraph.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Comments/Example_1.html)

## Single line comments at the end of a line

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Comments</h2>

        <p id="demo"></p>

        <script>
            let x = 5;      // Declare x, give it the value of 5
            let y = x + 2;  // Declare y, give it the value of x + 2 

            // Write y to demo:
            document.getElementById("demo").innerHTML = y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Comments/Example_2.html)

## Multiple lines comments

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1 id="myH"></h1>
        <p id="myP"></p>

        <script>
            /*
            The code below will change
            the heading with id = "myH"
            and the paragraph with id = "myP"
            */
            document.getElementById("myH").innerHTML = "JavaScript Comments";
            document.getElementById("myP").innerHTML = "My first paragraph.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Comments/Example_3.html)

## Single line comment to prevent execution

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Comments</h2>

        <h1 id="myH"></h1>

        <p id="myP"></p>

        <script>
            // document.getElementById("myH").innerHTML = "My First Page";
            document.getElementById("myP").innerHTML = "My first paragraph.";
        </script>

        <p>The line starting with // is not executed.</p>
    </body>
</html>
```

Output:

[Click here!](./Comments/Example_4.html)

## Multiple lines comment to prevent execution

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Comments</h2>

        <h1 id="myH"></h1>

        <p id="myP"></p>

        <script>
            /*
            document.getElementById("myH").innerHTML = "Welcome to my Homepage";
            document.getElementById("myP").innerHTML = "This is my first paragraph.";
            */
            document.getElementById("myP").innerHTML = "The comment-block is not executed.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Comments/Example_5.html)