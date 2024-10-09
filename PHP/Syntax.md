# Syntax

## Write text to the output using PHP

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>My first PHP page</h1>
        
        <?php
            echo "Hello World!";
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_syntax)

## Keywords, classes, functions, and user-defined functions ARE NOT case-sensitive

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            ECHO "Hello World!<br>";
            echo "Hello World!<br>";
            EcHo "Hello World!<br>";
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_syntax_case1)

## Variable names ARE case-sensitive

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $color = "red";
            
            echo "My car is " . $color . "<br>";
            echo "My house is " . $COLOR . "<br>";
            echo "My boat is " . $coLOR . "<br>";
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_syntax_case2)