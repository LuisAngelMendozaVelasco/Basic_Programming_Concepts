# Dates

## Use Date() to display today's date and time

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Dates</h1>
        <h2>Using new Date()</h2>
        <p>new Date() without arguments, creates a date object with the current date and time:</p>

        <p id="demo"></p>

        <script>
            const d = new Date();
            
            document.getElementById("demo").innerHTML = d;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Dates/Example_1.html)

## Use getFullYear() display the year

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Dates</h1>
        <h2>The getFullYear() Method</h2>
        <p>Return the full year of a date object:</p>

        <p id="demo"></p>

        <script>
            const d = new Date();
            
            document.getElementById("demo").innerHTML = d.getFullYear();
        </script>
    </body>
</html>
```

Output:

[Click here!](./Dates/Example_2.html)

## Use getTime() to calculate the number of milliseconds since 1970

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Dates</h1>
        <h2>The getTime() Method</h2>
        <p></p>
        <p>Return the number of milliseconds since midnight January 1, 1970:</p>

        <p id="demo"></p>

        <script>
            const d = new Date();
            
            document.getElementById("demo").innerHTML = d.getTime();
        </script>
    </body>
</html>
```

Output:

[Click here!](./Dates/Example_3.html)

## Use setFullYear() to set a specific date

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript setFullYear()</h2>
        <p>The setFullYear() method sets the year of a date object:</p>

        <p id="demo"></p>

        <script>
            const d = new Date();
            
            d.setFullYear(2020);
            document.getElementById("demo").innerHTML = d;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Dates/Example_4.html)

## Use toUTCString() to convert today's date (according to UTC) to a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Dates</h1>
        <h2>The toUTCString() Method</h2>
        <p>Convert a date to a string using the UTC standard:</p>

        <p id="demo"></p>

        <script>
            const d = new Date();
            
            document.getElementById("demo").innerHTML = d.toUTCString();
        </script>
    </body>
</html>
```

Output:

[Click here!](./Dates/Example_5.html)

## Use getDay() to display the weekday as a number

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Dates</h1>
        <h2>The getDay() Method</h2>
        <p>Return the weekday as a number:</p>

        <p id="demo"></p>

        <script>
            const d = new Date();
            
            document.getElementById("demo").innerHTML = d.getDay();
        </script>
    </body>
</html>
```

Output:

[Click here!](./Dates/Example_6.html)

## Use getDay() and an array to display the weekday as a name

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Dates</h1>
        <h2>The getDay() Method</h2>
        <p>Return the weekday as a number.</p>
        <p>You can use an array of names to return the weekday as a name:</p>

        <p id="demo"></p>

        <script>
            const days = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"];
            const d = new Date();
            let day = days[d.getDay()];
            
            document.getElementById("demo").innerHTML = day;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Dates/Example_7.html)

## Display a clock

Code: 

```html
<!DOCTYPE html>
<html>
    <body onload="startTime()">
        <h2>JavaScript Clock</h2>

        <div id="txt"></div>

        <script>
            function startTime() {
                const today = new Date();
                let h = today.getHours();
                let m = today.getMinutes();
                let s = today.getSeconds();

                m = checkTime(m);
                s = checkTime(s);
                document.getElementById('txt').innerHTML =  h + ":" + m + ":" + s;
                setTimeout(startTime, 1000);
            }

            function checkTime(i) {
                if (i < 10) {i = "0" + i};  // add zero in front of numbers < 10
                return i;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Dates/Example_8.html)