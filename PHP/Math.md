# Math

## Find the value of PI

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo(pi());
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_math_pi)

## Find the lowest and highest value in a list of arguments

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo(min(0, 150, 30, 20, -8, -200) . "<br>");
            echo(max(0, 150, 30, 20, -8, -200));
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_math_min_max)

## Find the absolute (positive) value of a number

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo(abs(-6.7));
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_math_abs)

## Find the square root of a number

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo(sqrt(64) . "<br>");
            echo(sqrt(0) . "<br>");
            echo(sqrt(1) . "<br>");
            echo(sqrt(9));
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_math_sqrt)

## Round a floating-point number to its nearest integer

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo(round(0.60) . "<br>");
            echo(round(0.50) . "<br>");
            echo(round(0.49) . "<br>");
            echo(round(-4.40) . "<br>");
            echo(round(-4.60));
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_math_round)

## Generate a random number

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo(rand());
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_math_rand)

## Generate a random number between 10 and 100

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo(rand(10, 100));
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_math_rand2)