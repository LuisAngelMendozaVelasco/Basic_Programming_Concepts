# Events

## An onclick event changes an HTML element

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <button onclick="document.getElementById('demo').innerHTML = Date()">The time is?</button>

        <p id="demo"></p>
    </body>
</html>
```

Output:

[Click here!](./Events/Example_1.html)

## An onclick event changes its own element

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript HTML Events</h2>
        <button onclick="this.innerHTML=Date()">The time is?</button>
    </body>
</html>
```

Output:

[Click here!](./Events/Example_2.html)

## An onclick event calls a function

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript HTML Events</h2>
        <p>Click the button to display the date.</p>

        <button onclick="displayDate()">The time is?</button>

        <script>
            function displayDate() {
                document.getElementById("demo").innerHTML = Date();
            }
        </script>

        <p id="demo"></p>
    </body>
</html> 
```

Output:

[Click here!](./Events/Example_3.html)