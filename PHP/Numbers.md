# Numbers

## Check if the type of a variable is integer

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Check if the type of a variable is integer   
            $x = 5985;

            var_dump(is_int($x));
            echo "<br>";

            // Check again... 
            $x = 59.85;
            
            var_dump(is_int($x));
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_numbers_integer)

## Check if the type of a variable is float

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Check if the type of a variable is float 
            $x = 10.365;
            
            var_dump(is_float($x));
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_numbers_float)

## Check if a numeric value is finite or infinite

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Check if a numeric value is finite or infinite 
            $x = 1.9e411;
            
            var_dump($x);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_numbers_infinite)

## Invalid calculation will return a NaN value

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Invalid calculation will return a NaN value
            $x = acos(8);
            
            var_dump($x);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_numbers_nan)

## Check if a variable is numeric

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Check if the variable is numeric   
            $x = 5985;
            var_dump(is_numeric($x));

            echo "<br>";

            $x = "5985";
            var_dump(is_numeric($x));

            echo "<br>";

            $x = "59.85" + 100;
            var_dump(is_numeric($x));

            echo "<br>";

            $x = "Hello";
            var_dump(is_numeric($x));
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_numbers_numeric)

## Cast float and string to integer

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Cast float to int 
            $x = 23465.768;
            $int_cast = (int)$x;

            echo $int_cast;
            echo "<br>";

            // Cast string to int
            $x = "23465.768";
            $int_cast = (int)$x;
            
            echo $int_cast;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_numbers_cast)