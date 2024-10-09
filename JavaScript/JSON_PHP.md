# JSON PHP

## Get JSON from a php file

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Get JSON Data from a PHP Server</h2>
        <p id="demo"></p>

        <script>
            const xmlhttp = new XMLHttpRequest();

            xmlhttp.onload = function() {
                const myObj = JSON.parse(this.responseText);
                
                document.getElementById("demo").innerHTML = myObj.name;
            }

            xmlhttp.open("GET", "./demo_file.php");
            xmlhttp.send();
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_PHP/Example_1.html)

## Get JSON array from php

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Get JSON Data from a PHP Server</h2>
        <p>Convert the data into a JavaScript array:</p>
        <p id="demo"></p>

        <script>
            const xmlhttp = new XMLHttpRequest();

            xmlhttp.onload = function() {
                const myObj = JSON.parse(this.responseText);
                
                document.getElementById("demo").innerHTML = myObj[2];
            }

            xmlhttp.open("GET", "./demo_file_array.php");
            xmlhttp.send();
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_PHP/Example_2.html)

## Get JSON from a database

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Get JSON Data from a PHP Server</h2>
        <p>The JSON received from the PHP file:</p>

        <p id="demo"></p>

        <script>
            const dbParam = JSON.stringify({"limit":10});
            const xmlhttp = new XMLHttpRequest();

            xmlhttp.onload = function() {
                document.getElementById("demo").innerHTML = this.responseText;
            }
            
            xmlhttp.open("GET", "./json_demo_db.php?x=" + dbParam);
            xmlhttp.send();
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_PHP/Example_3.html)

## Loop through the result from a database

Code: 

```html
<!DOCTYPE html>
<html>
    <body>

        <h2>Get JSON Data from a PHP Server</h2>
        <p id="demo"></p>

        <script>
            const obj = {"limit":10};
            const dbParam = JSON.stringify(obj);
            const xmlhttp = new XMLHttpRequest();

            xmlhttp.onload =    function() {   
                                    myObj = JSON.parse(this.responseText);
                                    let text = ""

                                    for (let x in myObj) {
                                        text += myObj[x].name + "<br>";
                                    }

                                    document.getElementById("demo").innerHTML = text;
                                };

            xmlhttp.open("GET", "./json_demo_db.php?x=" + dbParam);
            xmlhttp.send();
        </script>

        <p>Try changing the "limit" property from 10 to 5.</p>

    </body>
</html>
```

Output:

[Click here!](./JSON_PHP/Example_4.html)

## Send JSON using POST method

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Use HTTP POST to Get JSON Data from a PHP Server</h2>

        <p id="demo"></p>

        <script>
            const dbParam = JSON.stringify({"limit":10});
            const xmlhttp = new XMLHttpRequest();

            xmlhttp.onload =    function() {
                                    myObj = JSON.parse(this.responseText);
                                    let text = "";

                                    for (let x in myObj) {
                                        text += myObj[x].name + "<br>";
                                    }

                                    document.getElementById("demo").innerHTML = text;
                                }

            xmlhttp.open("POST", "./json_demo_db_post.php");
            xmlhttp.setRequestHeader("Content-type", "application/x-www-form-urlencoded");
            xmlhttp.send("x=" + dbParam);
        </script>

        <p>Try changing the "limit" property from 10 to 5.</p>
    </body>
</html>
```

Output:

[Click here!](./JSON_PHP/Example_5.html)