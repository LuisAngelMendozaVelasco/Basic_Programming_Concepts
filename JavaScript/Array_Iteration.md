# Array Iteration

## Array.forEach()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.forEach()</h2>
        <p>Calls a function once for each array element.</p>

        <p id="demo"></p>

        <script>
            const numbers = [45, 4, 9, 16, 25];
            let txt = "";
            
            numbers.forEach(myFunction);
            document.getElementById("demo").innerHTML = txt;

            function myFunction(value, index, array) {
                txt += value + "<br>";
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_1.html)

## Array.map()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.map()</h2>
        <p>Creates a new array by performing a function on each array element.</p>

        <p id="demo"></p>

        <script>
            const numbers1 = [45, 4, 9, 16, 25];
            const numbers2 = numbers1.map(myFunction);

            document.getElementById("demo").innerHTML = numbers2;

            function myFunction(value, index, array) {
                return value * 2;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_2.html)

## Array.filter()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.filter()</h2>
        <p>Creates a new array with all array elements that passes a test.</p>

        <p id="demo"></p>

        <script>
            const numbers = [45, 4, 9, 16, 25];
            const over18 = numbers.filter(myFunction);

            document.getElementById("demo").innerHTML = over18;

            function myFunction(value, index, array) {
                return value > 18;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_3.html)

## Array.reduce()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.reduce()</h2>
        <p>This example finds the sum of all numbers in an array:</p>

        <p id="demo"></p>

        <script>
            const numbers = [45, 4, 9, 16, 25];
            let sum = numbers.reduce(myFunction);

            document.getElementById("demo").innerHTML = "The sum is " + sum;

            function myFunction(total, value, index, array) {
                return total + value;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_4.html)

## Array.reduceRight()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.reduceRight()</h2>
        <p>This example finds the sum of all numbers in an array:</p>

        <p id="demo"></p>

        <script>
            const numbers = [45, 4, 9, 16, 25];
            let sum = numbers.reduceRight(myFunction);

            document.getElementById("demo").innerHTML = "The sum is " + sum;

            function myFunction(total, value, index, array) {
                return total + value;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_5.html)

## Array.every()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.every()</h2>
        <p>The every() method checks if all array values pass a test.</p>

        <p id="demo"></p>

        <script>
            const numbers = [45, 4, 9, 16, 25];
            let allOver18 = numbers.every(myFunction);

            document.getElementById("demo").innerHTML = "All over 18 is " + allOver18;

            function myFunction(value, index, array) {
                return value > 18;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_6.html)

## Array.some()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.some()</h2>
        <p>The some() method checks if some array values pass a test.</p>

        <p id="demo"></p>

        <script>
            const numbers = [45, 4, 9, 16, 25];
            let someOver18 = numbers.some(myFunction);

            document.getElementById("demo").innerHTML = "Some over 18 is " + someOver18;

            function myFunction(value, index, array) {
                return value > 18;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_7.html)

## Array.indexOf()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.indexOf()</h2>

        <p id="demo"></p>

        <script>
            const fruits = ["Apple", "Orange", "Apple", "Mango"];
            let position = fruits.indexOf("Apple") + 1;

            document.getElementById("demo").innerHTML = "Apple is found in position " + position;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_8.html)

## Array.lastIndexOf()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.lastIndexOf()</h2>
        <p id="demo"></p>

        <script>
            const fruits = ["Apple", "Orange", "Apple", "Mango"];
            let position = fruits.lastIndexOf("Apple") + 1;

            document.getElementById("demo").innerHTML = "Apple is found in position " + position;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_9.html)

## Array.find()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.find()</h2>
        <p id="demo"></p>

        <script>
            const numbers = [4, 9, 16, 25, 29];
            let first = numbers.find(myFunction);

            document.getElementById("demo").innerHTML = "First number over 18 is " + first;

            function myFunction(value, index, array) {
                return value > 18;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_10.html)

## Array.findIndex()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array.findIndex()</h2>
        <p id="demo"></p>

        <script>
            const numbers = [4, 9, 16, 25, 29];

            document.getElementById("demo").innerHTML = "First number over 18 has index " + numbers.findIndex(myFunction);

            function myFunction(value, index, array) {
                return value > 18;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Iteration/Example_11.html)