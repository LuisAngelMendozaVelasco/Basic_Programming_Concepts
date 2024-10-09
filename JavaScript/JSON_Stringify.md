# JSON Stringify

## Use JSON stringify

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Create a JSON string from a JavaScript object.</h2>
        <p id="demo"></p>

        <script>
            const obj = {name: "John", age: 30, city: "New York"};
            const myJSON = JSON.stringify(obj);
            
            document.getElementById("demo").innerHTML = myJSON;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Stringify/Example_1.html)

## Using JSON stringify on an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Create a JSON string from a JavaScript array.</h2>
        <p id="demo"></p>

        <script>
            const arr = ["John", "Peter", "Sally", "Jane"];
            const myJSON = JSON.stringify(arr);
            
            document.getElementById("demo").innerHTML = myJSON;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Stringify/Example_2.html)

## Stringify dates

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JSON.stringify() converts date objects into strings.</h2>
        <p id="demo"></p>

        <script>
            const obj = {name: "John", today: new Date(), city: "New York"};
            const myJSON = JSON.stringify(obj);
            
            document.getElementById("demo").innerHTML = myJSON;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Stringify/Example_3.html)

## Stringify functions

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JSON.stringify() will remove any functions from an object.</h2>
        <p id="demo"></p>

        <script>
            const obj = {name: "John", age: function () {return 30;}, city: "New York"};
            const myJSON = JSON.stringify(obj);
            
            document.getElementById("demo").innerHTML = myJSON;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Stringify/Example_4.html)

## Stringify functions using the toString() method

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JSON.stringify() will remove any functions from an object.</h2>
        <p>Convert functions into strings to keep them in the JSON object.</p>

        <p id="demo"></p>

        <script>
            const obj = {name: "John", age: function () {return 30;}, city: "New York"};
            obj.age = obj.age.toString();
            const myJSON = JSON.stringify(obj);
            
            document.getElementById("demo").innerHTML = myJSON;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Stringify/Example_5.html)