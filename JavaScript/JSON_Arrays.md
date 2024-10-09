# JSON Arrays

## Accessing array values

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Access Array Values</h2>
        <p id="demo"></p>

        <script>
            const myJSON = '{"name":"John", "age":30, "cars":["Ford", "BMW", "Fiat"]}';
            const myObj = JSON.parse(myJSON);
            
            console.log(myObj);
            document.getElementById("demo").innerHTML = myObj.cars[0];
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Arrays/Example_1.html)

## Looping through an array using for-in

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Looping an Array</h2>
        <p id="demo"></p>

        <script>
            const myJSON = '{"name":"John", "age":30, "cars":["Ford", "BMW", "Fiat"]}';
            const myObj = JSON.parse(myJSON);
            let text = "";
            
            for (let i in myObj.cars) {
                text += myObj.cars[i] + ", ";
            }

            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Arrays/Example_2.html)

## Looping through an array using for

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Looping an Array</h2>
        <p id="demo"></p>

        <script>
            const myJSON = '{"name":"John", "age":30, "cars":["Ford", "BMW", "Fiat"]}';
            const myObj = JSON.parse(myJSON);
            let text = "";
            
            for (let i = 0; i < myObj.cars.length; i++) {
                text += myObj.cars[i] + ", ";
            }

            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Arrays/Example_3.html)

## Access nested JSON arrays

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Looping through arrays inside arrays.</p>
        <p id="demo"></p>

        <script>
            let x = "";
            const myObj = { "name": " John",
                            "age": 30,
                            "cars": [   {"name": "Ford", "models": ["Fiesta", "Focus", "Mustang"]},
                                        {"name": "BMW", "models": ["320", "X3", "X5"]},
                                        {"name": "Fiat", "models": ["500", "Panda"] }]}

            for (let i in myObj.cars) {
                x += "<h2>" + myObj.cars[i].name + "</h2>";
                
                for (let j in myObj.cars[i].models) {
                    x += myObj.cars[i].models[j] + "<br>";
                }
            }

            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Arrays/Example_4.html)

## Modify array values

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Modify an array value of an object.</p>
        <p id="demo"></p>

        <script>
            let x = "";
            const myObj = { "name": "John",
                            "age": 30,
                            "cars": ["Ford", "BMW", "Fiat"]};

            myObj.cars[1] = "Mercedes";

            for (let i in myObj.cars) {
                x += myObj.cars[i] + "<br>";
            }

            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Arrays/Example_5.html)

## Delete array items

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Delete array properties:</p>
        <p id="demo"></p>

        <script>
            let x = "";
            const myObj = { "name": "John",
                            "age": 30,
                            "cars": ["Ford", "BMW", "Fiat"]}

            delete myObj.cars[1];

            for (let i in myObj.cars) {
                x += myObj.cars[i] + "<br>";
            }

            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Arrays/Example_6.html)