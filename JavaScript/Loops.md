# Loops

## For loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript For Loop</h2>

        <p id="demo"></p>

        <script>
            let text = "";

            for (let i = 0; i < 5; i++) {
                text += "The number is " + i + "<br>";
            }

            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Loops/Example_1.html)

## Looping an Array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript For Loop</h2>

        <p id="demo"></p>

        <script>
            const cars = ["BMW", "Volvo", "Saab", "Ford", "Fiat", "Audi"];
            let text = "";
            
            for (let i = 0; i < cars.length; i++) {
                text += cars[i] + "<br>";
            }

            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Loops/Example_2.html)

## Looping through HTML headers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript For Loop</h2>

        <p>Loop from 1 to 6, to make HTML headings.</p>

        <div id="demo"></div>

        <script>
            var x ="", i;

            for (i=1; i<=6; i++) {
                x = x + "<h" + i + ">Heading " + i + "</h" + i + ">";
            }

            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Loops/Example_3.html)

## While loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript While Loop</h2>

        <p id="demo"></p>

        <script>
            let text = "";
            let i = 0;

            while (i < 10) {
                text += "The number is " + i + "<br>";
                i++;
            }

            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Loops/Example_4.html)

## Do While loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Do While Loop</h2>

        <p id="demo"></p>

        <script>
            let text = ""
            let i = 0;

            do {
                text += "The number is " + i + "<br>";
                i++;
            }
            while (i < 10);  

            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Loops/Example_5.html)

## Break a loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Loops</h2>

        <p>A loop with a <b>break</b> statement.</p>

        <p id="demo"></p>

        <script>
            let text = "";

            for (let i = 0; i < 10; i++) {
                if (i === 3) {break;}
                text += "The number is " + i + "<br>";
            }

            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Loops/Example_6.html)

## Break and continue a loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Loops</h2>

        <p>A loop with a <b>continue</b> statement.</p>

        <p>A loop which will skip the step where i = 3.</p>

        <p id="demo"></p>

        <script>
            let text = "";

            for (let i = 0; i < 10; i++) {
                if (i === 3) {continue;}
                text += "The number is " + i + "<br>";
            }

            document.getElementById("demo").innerHTML = text;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Loops/Example_7.html)

## Use a for...in statement to loop through the elements of an object

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript For In Loop</h2>
        <p>The for in statement loops through the properties of an object:</p>

        <p id="demo"></p>

        <script>
            const person = {fname:"John", lname:"Doe", age:25}; 
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

[Click here!](./Loops/Example_8.html)