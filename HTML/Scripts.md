# Scripts

## Insert a script

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Use JavaScript to Change Text</h2>
        <p>This example writes "Hello JavaScript!" into an HTML element with id="demo":</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "Hello JavaScript!";
        </script> 
    </body>
</html>
```

Output:

[Click here!](./Scripts/Example_1.html)

## Use of the `<noscript>` tag

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "Hello JavaScript!";
        </script>

        <noscript>Sorry, your browser does not support JavaScript!</noscript>

        <p>A browser without support for JavaScript will show the text written inside the noscript element.</p>
    </body>
</html>
```

Output:

[Click here!](./Scripts/Example_2.html)