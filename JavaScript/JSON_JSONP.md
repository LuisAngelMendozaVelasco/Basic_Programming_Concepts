# JSON JSONP

## Simple JSONP example

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Request JSON using the script tag</h2>
        <p>The PHP file returns a call to a function that will handle the JSON data.</p>
        <p id="demo"></p>

        <script>
            function myFunc(myObj) {
                document.getElementById("demo").innerHTML = myObj.name;
            }
        </script>

        <script src="https://www.w3schools.com/js/demo_jsonp.php"></script>
    </body>
</html>
```

Output:

[Click here!](./JSON_JSONP/Example_1.html)

## Create a dynamic script tag

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Click the Button.</h2>
        <p>A script tag with a src attribute is created and placed in the document.</p>
        <p>The PHP file returns a call to a function with the JSON object as a parameter.</p>

        <button onclick="clickButton()">Click me!</button>

        <p id="demo"></p>

        <script>
            function clickButton() {
                let s = document.createElement("script");
                
                s.src = "https://www.w3schools.com/js/demo_jsonp.php";
                document.body.appendChild(s);
            }

            function myFunc(myObj) {
                document.getElementById("demo").innerHTML = myObj.name;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_JSONP/Example_2.html)

## JSONP example with dynamic result

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p>A script tag with a src attribute is created and placed in the document.</p>
        <p>The PHP file returns a call to a function with an object as a parameter.</p>
        <p id="demo"></p>

        <p>Try changing the table property from "customers" to "products".</p>

        <script>
            const obj = {table: "customers", limit: 10};
            let s = document.createElement("script");

            s.src = "https://www.w3schools.com/js/jsonp_demo_db.php?x=" + JSON.stringify(obj);
            document.body.appendChild(s);

            function myFunc(myObj) {
                let txt = "";
                
                for (let x in myObj) {
                    txt += myObj[x].name + "<br>";
                }

                document.getElementById("demo").innerHTML = txt;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_JSONP/Example_3.html)

## JSONP example with a callback function

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Request With a Callback Function</h2>
        <p>The PHP file returns a call to the function you send as a callback.</p>
        <p id="demo"></p>

        <script>
            let s = document.createElement("script");
            
            s.src = "https://www.w3schools.com/js/demo_jsonp2.php?callback=myDisplayFunction";
            document.body.appendChild(s);

            function myDisplayFunction(myObj) {
                document.getElementById("demo").innerHTML = myObj.name;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_JSONP/Example_4.html)