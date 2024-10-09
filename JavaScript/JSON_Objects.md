# JSON Objects

## Accessing properties using .property

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Access a JavaScript Object</h2>
        <p id="demo"></p>

        <script>
            const myJSON = '{"name": "John", "age": 30, "car": null}';
            const myObj = JSON.parse(myJSON);
            
            document.getElementById("demo").innerHTML = myObj.name;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Objects/Example_1.html)

## Accessing properties using [property]

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Access a JavaScript Object</h2>
        <p id="demo"></p>

        <script>
            const myJSON = '{"name": "John", "age": 30, "car": null}';
            const myObj = JSON.parse(myJSON);
            
            document.getElementById("demo").innerHTML = myObj["name"];
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Objects/Example_2.html)

## Looping through properties

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Looping Object Properties</h2>
        <p id="demo"></p>

        <script>
            const myJSON = '{"name": "John", "age": 30, "car": null}';
            const myObj = JSON.parse(myJSON);
            let text = "";

            for (const x in myObj) {
                text += x + ", ";
            }
            
            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Objects/Example_3.html)

## Looping through property values

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Looping JavaScript Object Values</h2>
        <p id="demo"></p>

        <script>
            const myJSON = '{"name": "John", "age": 30, "car": null}';
            const myObj = JSON.parse(myJSON);
            let text = "";

            for (const x in myObj) {
                text += myObj[x] + ", ";
            }
            
            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Objects/Example_4.html)

## Access nested JSON objects

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Access Nested JavaScript Objects</h2>
        <p id="demo"></p>

        <script>
            const myObj = { "name": "John",
                            "age": 30,
                            "cars": {   "car1": "Ford",
                                        "car2": "BMW",
                                        "car3": "Fiat"}}

            document.getElementById("demo").innerHTML = myObj.cars.car2;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Objects/Example_5.html)

## Modify values using the dot notation

Code: 

```html
<!DOCTYPE html>
<html>
    <body>

        <p>Modify object values:</p>

        <p id="demo"></p>

        <script>
            let x = "";
            let myObj = {   "name": "John",
                            "age": 30,
                            "cars": {   "car1": "Ford",
                                        "car2": "BMW",
                                        "car3": "Fiat"}}

            myObj.cars.car2 = "Mercedes";

            for (let i in myObj.cars) {
                x += myObj.cars[i] + "<br>";
            }

            document.getElementById("demo").innerHTML = x;
        </script>

    </body>
</html>
```

Output:

[Click here!](./JSON_Objects/Example_6.html)

## Modify values using the bracket notation

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Modify object values using bracket notation:</p>

        <p id="demo"></p>

        <script>
            let x = "";
            let myObj = {   "name": "John",
                            "age": 30,
                            "cars": {   "car1": "Ford",
                                        "car2": "BMW",
                                        "car3": "Fiat"}}
                                        
            myObj.cars["car2"] = "Mercedes";

            for (let i in myObj.cars) {
                x += myObj.cars[i] + "<br>";
            }

            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Objects/Example_7.html)

## Delete object properties

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Delete JavaScript Object Properties</h2>

        <p id="demo"></p>

        <script>
            let x = "";
            let myObj = {   "name": "John",
                            "age": 30,
                            "cars": {   "car1": "Ford",
                                        "car2": "BMW",
                                        "car3": "Fiat"}}
                                        
            delete myObj.cars.car2;

            for (let i in myObj.cars) {
                x += myObj.cars[i] + "<br>";
            }

            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Objects/Example_8.html)