# Conditionals

## The if statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript if</h2>

        <p>Display "Good day!" if the hour is less than 18:00:</p>

        <p id="demo">Good Evening!</p>

        <script>
            if (new Date().getHours() < 18) {
                document.getElementById("demo").innerHTML = "Good day!";
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Conditionals/Example_1.html)

## The else statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript if .. else</h2>

        <p>A time-based greeting:</p>

        <p id="demo"></p>

        <script>
            const hour = new Date().getHours(); 
            let greeting;

            if (hour < 18) {
                greeting = "Good day!";
            } 
            else {
                greeting = "Good evening!";
            }

            document.getElementById("demo").innerHTML = greeting;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Conditionals/Example_2.html)

## The else if statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript if .. else</h2>

        <p>A time-based greeting:</p>

        <p id="demo"></p>

        <script>
            const time = new Date().getHours();
            let greeting;

            if (time < 10) {
                greeting = "Good morning!";
            } 
            else if (time < 20) {
                greeting = "Good day!";
            } 
            else {
                greeting = "Good evening!";
            }
            
            document.getElementById("demo").innerHTML = greeting;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Conditionals/Example_3.html)

## Random link

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Math.random()</h2>

        <p id="demo"></p>

        <script>
            let text;

            if (Math.random() < 0.5) {
                text = "<a href='https://w3schools.com'>Visit W3Schools</a>";
            } 
            else {
                text = "<a href='https://wwf.org'>Visit WWF</a>";
            }
            
            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Conditionals/Example_4.html)

## Switch statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript switch</h2>

        <p id="demo"></p>

        <script>
            let day;

            switch (new Date().getDay()) {
                case 0:
                    day = "Sunday";
                    break;
                case 1:
                    day = "Monday";
                    break;
                case 2:
                    day = "Tuesday";
                    break;
                case 3:
                    day = "Wednesday";
                    break;
                case 4:
                    day = "Thursday";
                    break;
                case 5:
                    day = "Friday";
                    break;
                case  6:
                    day = "Saturday";
            }
            
            document.getElementById("demo").innerHTML = "Today is " + day;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Conditionals/Example_5.html)