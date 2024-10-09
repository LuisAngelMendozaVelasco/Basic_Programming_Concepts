# Error Handling

## The try...catch statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Error Handling</h2>

        <p>How to use <b>catch</b> to display an error.</p>

        <p id="demo"></p>

        <script>
            try {
                adddlert("Welcome guest!");
            }
            catch(err) {
                document.getElementById("demo").innerHTML = err.message;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Error_Handling/Example_1.html)

## The try...catch statement with a confirm box

Code: 

```html
<!DOCTYPE html>
<html>
    <script>
        var txt = "";

        function message() {
            try {
                adddlert("Welcome guest!");
            }
            catch(err) {
                txt = "There was an error on this page.\n\n";
                txt += "Click OK to continue viewing this page,\n";
                txt += "or Cancel to return to the home page.\n\n";
                
                if(!confirm(txt)) {
                    document.location.href = "https://www.w3schools.com/";
                }
            }
        }
    </script>
    <body>
        <h2>JavaScript Error Handling</h2>

        <input type="button" value="View message" onclick="message()" />
    </body>
</html>
```

Output:

[Click here!](./Error_Handling/Example_2.html)

## The onerror event

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <script>
            onerror = handleErr;
            var txt = "";

            function handleErr(msg, url, l) {
                txt = "There was an error on this page.\n\n";
                txt += "Error: " + msg + "\n";
                txt += "URL: " + url + "\n";
                txt += "Line: " + l + "\n\n";
                txt += "Click OK to continue.\n\n";
                alert(txt);
                return true;
            }

            function message() {
                adddlert("Welcome guest!");
            }
        </script>
    </head>
    <body>
        <input type="button" value="View message" onclick="message()"/>
    </body>
</html>
```

Output:

[Click here!](./Error_Handling/Example_3.html)