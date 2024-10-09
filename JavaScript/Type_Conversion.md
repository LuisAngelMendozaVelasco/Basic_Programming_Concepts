# Type Conversion

## Display the typeof all variable types

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Operators</h1>
        <h2>The typeof Operator</h2>

        <p>The typeof operator returns the type of a variable, object, function or expression:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "'John' is " + typeof("John") + "<br>" +
                                                        "3.14 is " + typeof(3.14) + "<br>" +
                                                        "NaN is " + typeof(NaN) + "<br>" +
                                                        "false is " + typeof(false) + "<br>" +
                                                        "[1, 2, 3, 4] is " + typeof([1, 2, 3, 4]) + "<br>" +
                                                        "{name:'John', age:34} is " + typeof({name:'John', age:34}) + "<br>" +
                                                        "new Date() is " + typeof(new Date()) + "<br>" +
                                                        "function () {} is " + typeof(function () {}) + "<br>" +
                                                        "myCar is " + typeof(myCar) + "<br>" +
                                                        "null is " + typeof(null);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Type_Conversion/Example_1.html)

## Display the constructor of all variable types

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Properties</h1>
        <h2>The constructor Property</h2>

        <p>The constructor property returns the constructor function for a variable or an object.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "john".constructor + "<br>" +
                                                        (3.14).constructor + "<br>" +
                                                        false.constructor + "<br>" +
                                                        [1,2,3,4].constructor + "<br>" +
                                                        {name:'john', age:34}.constructor + "<br>" +
                                                        new Date().constructor + "<br>" +
                                                        function () {}.constructor;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Type_Conversion/Example_2.html)

## Convert a number to a string using String()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The JavaScript String() Method</h2>

        <p>The String() method can convert a number to a string.</p>

        <p id="demo"></p>

        <script>
            let x = 123;
            document.getElementById("demo").innerHTML = String(x) + "<br>" +
                                                        String(123) + "<br>" +
                                                        String(100 + 23);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Type_Conversion/Example_3.html)

## Convert a number to a string using toString()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Number Methods</h2>

        <p>The toString() method converts a number to a string.</p>

        <p id="demo"></p>

        <script>
            let x = 123;
            document.getElementById("demo").innerHTML = x.toString() + "<br>" +
                                                        (123).toString() + "<br>" +
                                                        (100 + 23).toString();
        </script>
    </body>
</html>
```

Output:

[Click here!](./Type_Conversion/Example_4.html)

## Find out if a variable is an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Arrays</h1>
        <p>This "home made" isArray() function returns true when used on an array:</p>

        <p id="demo"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple"];

            document.getElementById("demo").innerHTML = isArray(fruits);

            function isArray(myArray) {
                return myArray.constructor.toString().indexOf("Array") > -1;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Type_Conversion/Example_5.html)

## Find out if a variable is a date

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Date Object</h2>
        <p>This "home made" isDate() function returns true when used on an date:</p>

        <p id="demo"></p>

        <script>
            const myDate = new Date();
            
            document.getElementById("demo").innerHTML = isDate(myDate);

            function isDate(myDate) {
                return myDate.constructor.toString().indexOf("Date") > -1;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Type_Conversion/Example_6.html)