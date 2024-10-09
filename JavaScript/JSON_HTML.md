# JSON HTML

## Make an HTML table based on JSON data

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Make a table based on JSON data.</h2>

        <p id="demo"></p>

        <script>
            const dbParam = JSON.stringify({table:"customers", limit:20});
            const xmlhttp = new XMLHttpRequest();

            xmlhttp.onload =    function() {
                                    const myObj = JSON.parse(this.responseText);
                                    let text = "<table border='1'>"

                                    for (let x in myObj) {
                                        text += "<tr><td>" + myObj[x].name + "</td></tr>";
                                    }

                                    text += "</table>"    
                                    document.getElementById("demo").innerHTML = text;
                                }

            xmlhttp.open("POST", "./json_demo_html_table.php");
            xmlhttp.setRequestHeader("Content-type", "application/x-www-form-urlencoded");
            xmlhttp.send("x=" + dbParam);
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_HTML/Example_1.html)

## Make a dynamic HTML Table

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Make a table based on the value of a drop down menu.</h2>

        <select id="myselect" onchange="change_myselect(this.value)">
            <option value="">Choose an option:</option>
            <option value="customers">Customers</option>
            <option value="products">Products</option>
            <option value="suppliers">Suppliers</option>
        </select>

        <p id="demo"></p>

        <script>
            function change_myselect(sel) {
                const dbParam = JSON.stringify({table:sel, limit:20});
                const xmlhttp = new XMLHttpRequest();

                xmlhttp.onload = function() {
                    myObj = JSON.parse(this.responseText);
                    text = "<table border='1'>"

                    for (x in myObj) {
                        text += "<tr><td>" + myObj[x].name + "</td></tr>";
                    }
                    
                    text += "</table>"    
                    document.getElementById("demo").innerHTML = text;
                }

                xmlhttp.open("POST", "./json_demo_html_table.php", true);
                xmlhttp.setRequestHeader("Content-type", "application/x-www-form-urlencoded");
                xmlhttp.send("x=" + dbParam);
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_HTML/Example_2.html)

## Make an HTML drop down list based on JSON data

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Make a drop down list based on JSON data.</h2>
        <p id="demo"></p>

        <script>
            const dbParam = JSON.stringify({table:"customers", limit:20});
            const xmlhttp = new XMLHttpRequest();

            xmlhttp.onload = function() {
                const myObj = JSON.parse(this.responseText);
                let text = "<select>"

                for (let x in myObj) {
                    text += "<option>" + myObj[x].name + "</option>";
                }

                text += "</select>"
                document.getElementById("demo").innerHTML = text;
            }

            xmlhttp.open("POST", "./json_demo_html_table.php");
            xmlhttp.setRequestHeader("Content-type", "application/x-www-form-urlencoded");
            xmlhttp.send("x=" + dbParam);
        </script>
    </body>
</html>
```

Output:

[Click here!](./JSON_HTML/Example_3.html)