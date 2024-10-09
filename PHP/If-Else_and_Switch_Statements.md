# If-Else and Switch Statements

## The if statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $t = date("H");

            if ($t < "20") {
                echo "Have a good day!";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_if)

## The if...else statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $t = date("H");

            if ($t < "20") {
                echo "Have a good day!";
            } 
            else {
                echo "Have a good night!";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_if_else)

## The if...elseif...else statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            date_default_timezone_set('America/Mexico_City');

            $t = date("H");
            echo "<p>The hour (of the server) is " . $t; 
            echo ", and will give the following message:</p>";

            if ($t < "10") {
                echo "Have a good morning!";
            } 
            elseif ($t < "20") {
                echo "Have a good day!";
            } 
            else {
                echo "Have a good night!";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_if_elseif)

## The switch statement

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $favcolor = "red";

            switch ($favcolor) {
                case "red":
                    echo "Your favorite color is red!";
                    break;
                case "blue":
                    echo "Your favorite color is blue!";
                    break;
                case "green":
                    echo "Your favorite color is green!";
                    break;
                default:
                    echo "Your favorite color is neither red, blue, nor green!";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_switch)