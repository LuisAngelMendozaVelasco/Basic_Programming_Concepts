# JSON Parse

## Use JSON parse

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Creating an Object from a JSON String</h2>

        <p id="demo"></p>

        <script>
            const txt = '{"name":"John", "age":30, "city":"New York"}'
            const obj = JSON.parse(txt);
            
            document.getElementById("demo").innerHTML = obj.name + ", " + obj.age;
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Parse/Example_1.html)

## Using JSON parse in an AJAX example

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Fetch a JSON file with XMLHttpRequest</h2>
        <p id="demo"></p>

        <script>
            const xmlhttp = new XMLHttpRequest();

            xmlhttp.onload = function() {
                const myObj = JSON.parse(this.responseText);
                
                document.getElementById("demo").innerHTML = myObj.name;
            }

            xmlhttp.open("GET", "./json_demo.txt");
            xmlhttp.send();
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Parse/Example_2.html)

## Using JSON parse on an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Fetch a JSON file with XMLHttpRequest</h2>
        <p>Content written as an JSON array will be converted into a JavaScript array.</p>
        <p id="demo"></p>

        <script>
            const xmlhttp = new XMLHttpRequest();

            xmlhttp.onload = function() {
                const myArr = JSON.parse(this.responseText);
                
                document.getElementById("demo").innerHTML = myArr[0];
            }

            xmlhttp.open("GET", "./json_demo_array.txt", true);
            xmlhttp.send();
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Parse/Example_3.html)

## Parsing dates

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Convert a string into a date object.</h2>
        <p id="demo"></p>

        <script>
            const text = '{"name":"John", "birth":"1986-12-14", "city":"New York"}';
            const obj = JSON.parse(text);
            
            obj.birth = new Date(obj.birth);
            document.getElementById("demo").innerHTML = obj.name + ", " + obj.birth; 
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Parse/Example_4.html)

## Parsing dates using the reviver function

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Convert a string into a date object.</h2>

        <p id="demo"></p>

        <script>
            const text = '{"name":"John", "birth":"1986-12-14", "city":"New York"}';
            const obj = JSON.parse(text, function (key, value) {if (key == "birth") {
                                                                    return new Date(value);
                                                                } 
                                                                else {
                                                                    return value;
                                                                }});

            document.getElementById("demo").innerHTML = obj.name + ", " + obj.birth; 
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Parse/Example_5.html)

## Parsing functions

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Convert a string into a function.</h2>
        <p id="demo"></p>

        <script>
            const text = '{"name":"John", "age":"function() {return 30;}", "city":"New York"}';
            const obj = JSON.parse(text);
            
            obj.age = eval("(" + obj.age + ")");
            document.getElementById("demo").innerHTML = obj.name + ", " + obj.age(); 
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_Parse/Example_6.html)