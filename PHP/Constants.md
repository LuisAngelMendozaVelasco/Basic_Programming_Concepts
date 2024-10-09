# Constants

## Case-sensitive constant name

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // case-sensitive constant name
            define("GREETING", "Welcome to W3Schools.com!");
            echo GREETING;
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_constant1)

## Case-insensitive constant name

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // case-insensitive constant name
            define("GREETING", "Welcome to W3Schools.com!", true);
            echo greeting;
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_constant2)

## Create a Array constant with define()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            define("cars", ["Alfa Romeo", "BMW", "Toyota"]);
            echo cars[0];
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_constant_array)

## Use a constant inside a function (when it is defined outside the function)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            define("GREETING", "Welcome to W3Schools.com!");

            function myTest() {
                echo GREETING;
            }
            
            myTest();
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_constant3)