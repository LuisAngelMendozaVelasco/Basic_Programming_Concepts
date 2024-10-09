# Objects

## Create a JavaScript variable

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Variables</h2>

        <p id="demo"></p>

        <script>
            // Create and display a variable:
            let car = "Fiat";
            
            document.getElementById("demo").innerHTML = car;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_1.html)

## Create a JavaScript object

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>

        <p id="demo"></p>

        <script>
            // Create an object:
            const car = {type:"Fiat", model:"500", color:"white"};

            // Display some data from the object:
            document.getElementById("demo").innerHTML = "The car type is " + car.type;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_2.html)

## Create a person object (single line)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>

        <p id="demo"></p>

        <script>
            // Create an object:
            const person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};

            // Display some data from the object:
            document.getElementById("demo").innerHTML = person.firstName + " is " + person.age + " years old.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_3.html)

## Create a person object (multiple lines)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>

        <p id="demo"></p>

        <script>
            // Create an object:
            const person = {firstName: "John",
                            lastName: "Doe",
                            age: 50,
                            eyeColor: "blue"};

            // Display some data from the object:
            document.getElementById("demo").innerHTML = person.firstName + " is " + person.age + " years old.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_4.html)

## Access object properties using .property

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>

        <p>There are two different ways to access an object property.</p>

        <p>You can use person.property or person["property"].</p>

        <p id="demo"></p>

        <script>
            // Create an object:
            const person = {firstName   : "John",
                            lastName    : "Doe",
                            id          :  5566};

            // Display some data from the object:
            document.getElementById("demo").innerHTML = person.firstName + " " + person.lastName;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_5.html)

## Access object properties using [property]

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>

        <p>There are two different ways to access an object property.</p>

        <p>You can use person.property or person["property"].</p>

        <p id="demo"></p>

        <script>
            // Create an object:
            const person = {firstName   : "John",
                            lastName    : "Doe",
                            id          :  5566};

            // Display some data from the object:
            document.getElementById("demo").innerHTML = person["firstName"] + " " + person["lastName"];
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_6.html)

## Access a function property as a method

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>
        <p>An object method is a function definition, stored as a property value.</p>

        <p id="demo"></p>

        <script>
            // Create an object:
            const person = {firstName: "John",
                            lastName: "Doe",
                            id: 5566,
                            fullName: function() {
                                return this.firstName + " " + this.lastName;
                            }};

            // Display data from the object:
            document.getElementById("demo").innerHTML = person.fullName();
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_7.html)

## Access a function property as a property

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>

        <p>If you access an object method without (), it will return the function definition:</p>

        <p id="demo"></p>

        <script>
            // Create an object:
            const person = {firstName: "John",
                            lastName : "Doe",
                            id: 5566,
                            fullName : function() {
                                return this.firstName + " " + this.lastName;
                            }};

            // Display data from the object:
            document.getElementById("demo").innerHTML = person.fullName;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_8.html)

## Creating a JavaScript object using new

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>
        <p>Creating a JavaScript Object:</p>

        <p id="demo"></p>

        <script>
            const person = new Object();
            person.firstName = "John";
            person.lastName = "Doe";
            person.age = 50;
            person.eyeColor = "blue"; 

            document.getElementById("demo").innerHTML = person.firstName + " is " + person.age + " years old.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_9.html)

## Creating JavaScript objects using a constructor

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Object Constructors</h2>

        <p id="demo"></p>

        <script>
            // Constructor function for Person objects
            function Person(first, last, age, eye) {
                this.firstName = first;
                this.lastName = last;
                this.age = age;
                this.eyeColor = eye;
            }

            // Create a Person object
            const myFather = new Person("John", "Doe", 50, "blue");

            // Display age
            document.getElementById("demo").innerHTML = "My father is " + myFather.age + "."; 
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_10.html)

## Creating built-in JavaScript objects

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p id="demo"></p>

        <script>
            var x1 = new Object();      // A new Object object
            var x2 = new String();      // A new String object
            var x3 = new Number();      // A new Number object
            var x4 = new Boolean();     // A new Boolean object
            var x5 = new Array();       // A new Array object
            var x6 = new RegExp();      // A new RegExp object
            var x7 = new Function();    // A new Function object
            var x8 = new Date();        // A new Date object

            document.getElementById("demo").innerHTML = "x1: " + typeof(x1) + "<br>" +
                                                        "x2: " + typeof(x2) + "<br>" +
                                                        "x3: " + typeof(x3) + "<br>" +
                                                        "x4: " + typeof(x4) + "<br>" +
                                                        "x5: " + typeof(x5) + "<br>" +
                                                        "x6: " + typeof(x6) + "<br>" +
                                                        "x7: " + typeof(x7) + "<br>" +
                                                        "x8: " + typeof(x8) + "<br>";
        </script>

        <p>There is no need to use String(), Number(), Boolean(), Array(), and RegExp()</p>
        <p>Read the JavaScript tutorials.</p>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_11.html)

## The best way to create JavaScript variables

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p id="demo"></p>

        <script>
            var x1 = {};
            var x2 = "";
            var x3 = 0;
            var x4 = false;
            var x5 = [];
            var x6 = /()/;
            var x7 = function(){};

            document.getElementById("demo").innerHTML = "x1: " + typeof(x1) + "<br>" +
                                                        "x2: " + typeof(x2) + "<br>" +
                                                        "x3: " + typeof(x3) + "<br>" +
                                                        "x4: " + typeof(x4) + "<br>" +
                                                        "x5: " + typeof(x5) + "<br>" +
                                                        "x6: " + typeof(x6) + "<br>" +
                                                        "x7: " + typeof(x7) + "<br>";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_12.html)

## JavaScript objects are mutable

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Objects</h2>
        <p>JavaScript objects are mutable.</p>
        <p>Any changes to a copy of an object will also change the original object:</p>

        <p id="demo"></p>

        <script>
            const person = {firstName: "John",
                            lastName: "Doe",
                            age: 50,
                            eyeColor: "blue"};

            const x = person;
            x.age = 10;

            document.getElementById("demo").innerHTML = person.firstName + " is " + person.age + " years old.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_13.html)

## Accessing properties using for in

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Object Properties</h2>
        <p>Looping object property values:</p>

        <p id="demo"></p>

        <script>
            const person = {fname:"John",
                            lname:"Doe",
                            age:25}; 

            let txt = "";
            
            for (let x in person) {
                txt += person[x] + " ";
            }

            document.getElementById("demo").innerHTML = txt;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_14.html)

## Adding new properties to existing objects

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Object Properties</h2>
        <p>Add a new property to an existing object:</p>

        <p id="demo"></p>

        <script>
            const person = {firstname: "John",
                            lastname: "Doe",
                            age: 50,
                            eyecolor: "blue"};

            person.nationality = "English";
            document.getElementById("demo").innerHTML = person.firstname + " is " + person.nationality + ".";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_15.html)

## Deleting properties from objects

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Object Properties</h2>
        <p>Deleting object properties.</p>

        <p id="demo"></p>

        <script>
            const person = {firstname: "John",
                            lastname: "Doe",
                            age: 50,
                            eyecolor: "blue"};

            delete person.age;

            document.getElementById("demo").innerHTML = person.firstname + " is " + person.age + " years old.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Objects/Example_16.html)