# Functions

## Create a function

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function writeMsg() {
                echo "Hello world!";
            }

            writeMsg();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_function1)

## Function with one argument

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function familyName($fname) {
                echo "$fname Refsnes.<br>";
            }

            familyName("Jani");
            familyName("Hege");
            familyName("Stale");
            familyName("Kai Jim");
            familyName("Borge");
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_function2)

## Function with two arguments

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function familyName($fname, $year) {
                echo "$fname Refsnes. Born in $year <br>";
            }

            familyName("Hege", "1975");
            familyName("Stale", "1978");
            familyName("Kai Jim", "1983");
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_function3)

## Function with default argument value

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function setHeight(int $minheight = 50) {
                echo "The height is : $minheight <br>";
            }

            setHeight(350);
            setHeight();
            setHeight(135);
            setHeight(80);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_function4)

## Function that returns a value

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function sum(int $x, int $y) {
                $z = $x + $y;
                return $z;
            }

            echo "5 + 10 = " . sum(5, 10) . "<br>";
            echo "7 + 13 = " . sum(7, 13) . "<br>";
            echo "2 + 4 = " . sum(2, 4);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_function5)

## Return type declarations

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Return type declarations
            function addNumbers(float $a, float $b) : float {
                return $a + $b;
            }

            echo addNumbers(1.2, 5.2); 
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_func_return_strict)

## Passing arguments by reference

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function add_five(&$value) {
                $value += 5;
            }

            $num = 2;
            add_five($num);
            echo $num;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_func_pass_ref)