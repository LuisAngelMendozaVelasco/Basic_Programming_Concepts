# Regular Expressions

## Search for an expression in a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Regular Expressions</h2>

        <p>Search a string for "w3Schools", and display the position of the match:</p>

        <p id="demo"></p>

        <script>
            let text = "Visit W3Schools!"; 
            let n = text.search(/w3Schools/i);
            
            document.getElementById("demo").innerHTML = n;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Regular_Expressions/Example_1.html)

## Search for an expression and replace it

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript String Methods</h2>

        <p>Replace "Microsoft" with "W3Schools" in the paragraph below:</p>

        <button onclick="myFunction()">Try it</button>

        <p id="demo">Please visit Microsoft!</p>

        <script>
            function myFunction() {
                let text = document.getElementById("demo").innerHTML;
                
                document.getElementById("demo").innerHTML = text.replace(/microsoft/i, "W3Schools");
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Regular_Expressions/Example_2.html)