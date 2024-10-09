# While and For Loops

## The while loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php  
            $x = 1;
            
            while($x <= 5) {
                echo "The number is: $x <br>";
                
                $x++;
            } 
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_loop_while)

## The do...while loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php 
            $x = 1;

            do {
                echo "The number is: $x <br>";
                
                $x++;
            } while ($x <= 5);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_loop_do_while)

## Another do...while loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php 
            $x = 6;

            do {
                echo "The number is: $x <br>";
                
                $x++;
            } while ($x <= 5);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_loop_do_while2)

## The for loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php  
            for ($x = 0; $x <= 10; $x++) {
                echo "The number is: $x <br>";
            }
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_loop_for)

## The foreach loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php  
            $colors = array("red", "green", "blue", "yellow"); 

            foreach ($colors as $value) {
                echo "$value <br>";
            }
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_loop_foreach)

## The break statement in a loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php  
            for ($x = 0; $x < 10; $x++) {
                if ($x == 4) {
                    break;
                }
                
                echo "The number is: $x <br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_break)

## The continue statement in a loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php  
            for ($x = 0; $x < 10; $x++) {
                if ($x == 4) {
                    continue;
                }
                
                echo "The number is: $x <br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_continue)