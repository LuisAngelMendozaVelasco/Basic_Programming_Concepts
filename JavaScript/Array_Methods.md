# Array Methods

## Add an element to an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2> 
        <h2>push()</h2>
        <p>The push() method appends a new element to an array:</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            
            document.getElementById("demo1").innerHTML = fruits;
            fruits.push("Kiwi");
            document.getElementById("demo2").innerHTML = fruits;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_1.html)

## Remove the last element of an array - pop()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2>
        <h2>pop()</h2>
        <p>The pop() method removes the last element from an array.</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            
            document.getElementById("demo1").innerHTML = fruits;
            fruits.pop();
            document.getElementById("demo2").innerHTML = fruits;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_2.html)

## Join all elements of an array into a string - join()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2> 
        <h2>join()</h2> 
        <p>The join() method joins array elements into a string.</p>
        <p>It this example we have used " * " as a separator between the elements:</p>

        <p id="demo"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            
            document.getElementById("demo").innerHTML = fruits.join(" * ");
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_3.html)

## Join two arrays - concat()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2>
        <h2>concat()</h2>
        <p>The concat() method merges (concatenates) arrays:</p>

        <p id="demo"></p>

        <script>
            const myGirls = ["Cecilie", "Lone"];
            const myBoys = ["Emil", "Tobias", "Linus"];
            const myChildren = myGirls.concat(myBoys);

            document.getElementById("demo").innerHTML = myChildren;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_4.html)

## Join three arrays - concat()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2>
        <h2>concat()</h2>
        <p>The concat() method merges (concatenates) arrays:</p>

        <p id="demo"></p>

        <script>
            const array1 = ["Cecilie", "Lone"];
            const array2 = ["Emil", "Tobias", "Linus"];
            const array3 = ["Robin", "Morgan"];
            const myChildren = array1.concat(array2, array3); 

            document.getElementById("demo").innerHTML = myChildren;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_5.html)

## Add an element to position 2 in an array - splice()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2>
        <h2>splice()</h2>
        <p>The splice() method adds new elements to an array:</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];

            document.getElementById("demo1").innerHTML = fruits;
            fruits.splice(2, 0, "Lemon", "Kiwi");
            document.getElementById("demo2").innerHTML = fruits;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_6.html)

## Convert an array to a string - toString()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2> 
        <h2>toString()</h2>
        <p>The toString() method returns an array as a comma separated string:</p>

        <p id="demo"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            
            document.getElementById("demo").innerHTML = fruits.toString();
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_7.html)

## Add new elements to the beginning of an array - unshift()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2> 
        <h2>unshift()</h2>
        <p>The unshift() method adds new elements to the beginning of an array:</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            
            document.getElementById("demo1").innerHTML = fruits;
            fruits.unshift("Lemon");
            document.getElementById("demo2").innerHTML = fruits;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_8.html)

## Remove the first element of an array - shift()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2> 
        <h2>shift()</h2>
        <p>The shift() method removes the first element of an array (and "shifts" the other elements to the left):</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            
            document.getElementById("demo1").innerHTML = fruits;
            fruits.shift();
            document.getElementById("demo2").innerHTML = fruits;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_9.html)

## Select elements from an array - slice()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Methods</h2> 
        <h2>slice()</h2>
        <p>When the slice() method is given two arguments, it selects array elements from the start argument, and up to (but not included) the end argument:</p>

        <p id="demo"></p>

        <script>
            const fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
            const citrus = fruits.slice(1, 3);
            
            document.getElementById("demo").innerHTML = fruits + "<br><br>" + citrus;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Methods/Example_10.html)