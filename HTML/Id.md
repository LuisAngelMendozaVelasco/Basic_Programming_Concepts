# Id

## Style an element with a specific id

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #myHeader { background-color: lightblue;
                        color: black;
                        padding: 40px;
                        text-align: center;} 
        </style>
    </head>
    <body>
        <h2>The id Attribute</h2>
        <p>Use CSS to style an element with the id "myHeader":</p>
        <h1 id="myHeader">My Header</h1>
    </body>
</html>
```

Output:

[Click here!](./Id/Example_1.html)

## Difference between class and id

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            /* Style the element with the id "myHeader" */
            #myHeader { background-color: lightblue;
                        color: black;
                        padding: 40px;
                        text-align: center;}

            /* Style all elements with the class name "city" */
            .city { background-color: tomato;
                    color: white;
                    padding: 10px;} 
        </style>
    </head>
    <body>
        <h2>Difference Between Class and ID</h2>
        <p>A class name can be used by multiple HTML elements, while an id name must only be used by one HTML element within the page:</p>

        <!-- An element with a unique id -->
        <h1 id="myHeader">My Cities</h1>

        <!-- Multiple elements with same class -->
        <h2 class="city">London</h2>
        <p>London is the capital of England.</p>

        <h2 class="city">Paris</h2>
        <p>Paris is the capital of France.</p>

        <h2 class="city">Tokyo</h2>
        <p>Tokyo is the capital of Japan.</p>
    </body>
</html>
```

Output:

[Click here!](./Id/Example_2.html)

## Access an element with a specific id, with JavaScript

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Using The id Attribute in JavaScript</h2>
        <p>JavaScript can access an element with a specified id by using the getElementById() method:</p>

        <h1 id="myHeader">Hello World!</h1>
        <button onclick="displayResult()">Change text</button>

        <script>
            function displayResult() {
                document.getElementById("myHeader").innerHTML = "Have a nice day!";
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Id/Example_3.html)