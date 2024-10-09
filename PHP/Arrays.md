# Arrays

## Indexed arrays

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $cars = array("Volvo", "BMW", "Toyota"); 
            
            echo "I like " . $cars[0] . ", " . $cars[1] . " and " . $cars[2] . ".";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_num)

## count() - Return the length of an array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $cars = array("Volvo", "BMW", "Toyota");
            
            echo count($cars);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_length)

## Loop through an indexed array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $cars = array("Volvo", "BMW", "Toyota");
            $arrlength = count($cars);

            for($x = 0; $x < $arrlength; $x++) {
                echo $cars[$x];
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_num_loop)

## Associative arrays

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");
            
            echo "Peter is " . $age['Peter'] . " years old.";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_assoc)

## Loop through an associative array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");

            foreach($age as $x => $x_value) {
                echo "Key=" . $x . ", Value=" . $x_value;
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_assoc_loop)