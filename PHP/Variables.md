# Variables

## Create different variables

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $txt = "Hello world!";
            $x = 5;
            $y = 10.5;

            echo $txt;
            echo "<br>";
            echo $x;
            echo "<br>";
            echo $y;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_var)

## Test global scope (variable outside function)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 5; // Global scope
            
            function myTest() {
                // Using x inside this function will generate an error
                echo "<p>Variable x inside function is: $x</p>";
            }

            myTest();
            echo "<p>Variable x outside function is: $x</p>";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_var_global)

## Test local scope (variable inside function)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function myTest() {
                $x = 5; // Local scope
                echo "<p>Variable x inside function is: $x</p>";
            } 

            myTest();
            // Using x outside the function will generate an error
            echo "<p>Variable x outside function is: $x</p>";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_var_local)

## Use the global keyword to access a global variable from within a function

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 5;
            $y = 10;

            function myTest() {
                global $x, $y;
                $y = $x + $y;
            } 

            myTest();  // run function
            echo $y; // output the new value for variable $y
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_var_global_keyword)

## Use the $GLOBALS[] array to access a global variable from within a function

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 5;
            $y = 10;

            function myTest() {
                $GLOBALS['y'] = $GLOBALS['x'] + $GLOBALS['y'];
            } 

            myTest();
            echo $y;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_var_globals)

## Use the static keyword to let a local variable not be deleted after execution of function

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function myTest() {
                static $x = 0;
                echo $x;
                $x++;
            }

            myTest();
            echo "<br>";
            myTest();
            echo "<br>";
            myTest();
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_var_static)