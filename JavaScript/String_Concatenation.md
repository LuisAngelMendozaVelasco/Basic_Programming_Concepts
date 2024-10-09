# String Concatenation

## Adding two strings together using the concatenating (+) operator

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Operators</h1>

        <p>The + operator concatenates (adds) strings.</p>

        <p id="demo"></p>

        <script>
            var txt1 = "What a very";
            var txt2 = "nice day!";

            document.getElementById("demo").innerHTML = txt1 + txt2;
        </script>
    </body>
</html>
```

Output:

[Click here!](./String_Concatenation/Example_1.html)

## Adding two strings together with a space in the first string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Operators</h2>

        <p>The + operator concatenates (adds) strings.</p>

        <p id="demo"></p>

        <script>
            var txt1 = "What a very ";
            var txt2 = "nice day!";
            
            document.getElementById("demo").innerHTML = txt1 + txt2;
        </script>
    </body>
</html>
```

Output:

[Click here!](./String_Concatenation/Example_2.html)

## Adding two strings together with a space in between

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Operators</h1>

        <p>The + operator concatenates (adds) strings.</p>

        <p id="demo"></p>

        <script>
            var txt1 = "What a very";
            var txt2 = "nice day!";

            document.getElementById("demo").innerHTML = txt1 + " " + txt2;
        </script>
    </body>
</html>
```

Output:

[Click here!](./String_Concatenation/Example_3.html)

## Adding two strings together using using the += operator

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Operators</h1>

        <p>The assignment operator += can concatenate strings.</p>

        <p id="demo"></p>

        <script>
            let text1 = "What a very ";
            text1 += "nice day!";
            
            document.getElementById("demo").innerHTML = text1;
        </script>
    </body>
</html>
```

Output:

[Click here!](./String_Concatenation/Example_4.html)

## Adding strings and numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Operators</h1>

        <p>Adding a number and a string, returns a string.</p>

        <p id="demo"></p>

        <script>
            let x = 5 + 5;
            let y = "5" + 5;
            let z = "Hello" + 5;
            
            document.getElementById("demo").innerHTML = x + "<br>" + y + "<br>" + z;
        </script>
    </body>
</html>
```

Output:

[Click here!](./String_Concatenation/Example_5.html)