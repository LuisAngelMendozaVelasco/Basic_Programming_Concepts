# Array Sort

## Sort an array in ascending order

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>The sort() method sorts an array alphabetically:</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            const fruits = ["Banana", "Orange", "Apple", "Mango"];
            
            document.getElementById("demo1").innerHTML = fruits;
            fruits.sort();
            document.getElementById("demo2").innerHTML = fruits;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_1.html)

## Sort an array in descending order

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort Reverse</h2>

        <p>The reverse() method reverses the elements in an array.</p>
        <p>By combining sort() and reverse() you can sort an array in descending order:</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            // Create and display an array:
            const fruits = ["Banana", "Orange", "Apple", "Mango"];

            document.getElementById("demo1").innerHTML = fruits;

            // First sort the array
            fruits.sort();

            // Then reverse it:
            fruits.reverse();
            document.getElementById("demo2").innerHTML = fruits;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_2.html)

## Sort an array of numbers ascending

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>Sort the array in ascending order:</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];

            document.getElementById("demo1").innerHTML = points;  
            points.sort(function(a, b) {return a - b});
            document.getElementById("demo2").innerHTML = points;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_3.html)

## Sort an array of numbers descending

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>Sort the array in descending order:</p>

        <p id="demo1"></p>
        <p id="demo2"></p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];
        
            document.getElementById("demo1").innerHTML = points;
            points.sort(function(a, b) {return b - a});
            document.getElementById("demo2").innerHTML = points;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_4.html)

## Sort numbers (alphabetically or numerically)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>

        <p>Click the buttons to sort the array alphabetically or numerically.</p>

        <button onclick="myFunction1()">Sort Alphabetically</button>
        <button onclick="myFunction2()">Sort Numerically</button>

        <p id="demo"></p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];

            document.getElementById("demo").innerHTML = points;  

            function myFunction1() {
                points.sort();
                document.getElementById("demo").innerHTML = points;
            }

            function myFunction2() {
                points.sort(function(a, b) {return a - b});
                document.getElementById("demo").innerHTML = points;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_5.html)

## Sort array numbers in random order

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>Click the button (again and again) to sort the array in random order.</p>

        <button onclick="myFunction()">Try it</button>
        <p id="demo"></p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];

            document.getElementById("demo").innerHTML = points;  

            function myFunction() {
                points.sort(function() {return 0.5 - Math.random()});
                document.getElementById("demo").innerHTML = points;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_6.html)

## Find the lowest number in an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>The lowest number is <span id="demo"></span>.</p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];

            points.sort(function(a, b) {return a - b});
            document.getElementById("demo").innerHTML = points[0];
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_7.html)

## Find the highest number in an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>The highest number is <span id="demo"></span>.</p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];
            
            points.sort(function(a, b) {return b - a});
            document.getElementById("demo").innerHTML = points[0];
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_8.html)

## Find the lowest number in an array using Math.min()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>

        <p>The lowest number is <span id="demo"></span>.</p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];
            
            document.getElementById("demo").innerHTML = myArrayMin(points);

            function myArrayMin(arr) {
                return Math.min.apply(null, arr);
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_9.html)

## Find the highest number in an array using Math.max()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>The highest number is <span id="demo"></span>.</p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];
            
            document.getElementById("demo").innerHTML = myArrayMax(points);

            function myArrayMax(arr) {
                return Math.max.apply(null, arr);
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_10.html)

## Using a "homemade" myArrayMin method

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>The lowest number is <span id="demo"></span>.</p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];

            document.getElementById("demo").innerHTML = myArrayMin(points);

            function myArrayMin(arr) {
                let len = arr.length;
                let min = Infinity;
                
                while (len--) {
                    if (arr[len] < min) {
                        min = arr[len];
                    }
                }
                return min;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_11.html)

## Using a "homemade" myArrayMax method

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>The highest number is <span id="demo"></span>.</p>

        <script>
            const points = [40, 100, 1, 5, 25, 10];

            document.getElementById("demo").innerHTML = myArrayMax(points);

            function myArrayMax(arr) {
                let len = arr.length;
                let max = -Infinity;
                
                while (len--) {
                    if (arr[len] > max) {
                        max = arr[len];
                    }
                }
                return max;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_12.html)

## Sort objects by numeric properties

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Array Sort</h2>
        <p>Sort car objects on age:</p>

        <p id="demo1"></p>
        
        <p id="demo2"></p>

        <script>
            const cars = [  {type:"Volvo", year:2016},
                            {type:"Saab", year:2001},
                            {type:"BMW", year:2010}];

            displayCars("demo1");
            cars.sort(function(a, b) {return a.year - b.year});
            displayCars("demo2");

            function displayCars(id_) {
                document.getElementById(id_).innerHTML =    cars[0].type + " " + cars[0].year + "<br>" +
                                                            cars[1].type + " " + cars[1].year + "<br>" +
                                                            cars[2].type + " " + cars[2].year;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_13.html)

## Sort objects by string properties

Code: 

```html
<!DOCTYPE html>
<html>
    <body>

        <h2>JavaScript Array Sort</h2>
        <p>Click the buttons to sort car objects on type.</p>

        <button onclick="myFunction()">Sort</button>
        <p id="demo"></p>

        <script>
            const cars = [  {type:"Volvo", year:2016},
                            {type:"Saab", year:2001},
                            {type:"BMW", year:2010}];

            displayCars();

            function myFunction() {
                cars.sort(  function(a, b) {  
                                let x = a.type.toLowerCase();
                                let y = b.type.toLowerCase();
                                if (x < y) {return -1;}
                                if (x > y) {return 1;}

                                return 0;
                            });
                displayCars();
            }

            function displayCars() {
                document.getElementById("demo").innerHTML = cars[0].type + " " + cars[0].year + "<br>" +
                                                            cars[1].type + " " + cars[1].year + "<br>" +
                                                            cars[2].type + " " + cars[2].year;
            }
        </script>

    </body>
</html>
```

Output:

[Click here!](./Array_Sort/Example_14.html)