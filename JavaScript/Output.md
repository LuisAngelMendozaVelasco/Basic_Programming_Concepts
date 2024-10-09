# Output

## Writing into the HTML output

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>My First Web Page</h2>
        <p>My first paragraph.</p>

        <p>Never call document.write after the document has finished loading.
        It will overwrite the whole document.</p>

        <script>
            document.write(5 + 6);
        </script>
    </body>
</html> 
```

Output:

[Click here!](./Output/Example_1.html)

## Writing into an HTML element

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>My First Web Page</h2>
        <p>My First Paragraph.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = 5 + 6;
        </script>
    </body>
</html> 
```

Output:

[Click here!](./Output/Example_2.html)

## Writing into an window alert box

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>My First Web Page</h2>
        <p>My first paragraph.</p>

        <script>
            window.alert(5 + 6);
        </script>
    </body>
</html> 
```

Output:

[Click here!](./Output/Example_3.html)

## Writing into the browser console

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Activate Debugging</h2>

        <p>F12 on your keyboard will activate debugging.</p>
        <p>Then select "Console" in the debugger menu.</p>
        <p>Then click Run again.</p>

        <script>
            console.log(5 + 6);
        </script>
    </body>
</html> 
```

Output:

[Click here!](./Output/Example_4.html)