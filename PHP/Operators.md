# Operators

## Arithmetic operator: Addition (+)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;  
            $y = 6;

            echo $x + $y;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_addition)

## Arithmetic operator: Subtraction (-)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;
            $y = 6;

            echo $x - $y;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_subtraction)

## Arithmetic operator: Multiplication (*)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;  
            $y = 6;

            echo $x * $y;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_multiplication)

## Arithmetic operator: Division (/)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;  
            $y = 6;

            echo $x / $y;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_division)

## Arithmetic operator: Modulus (%)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;  
            $y = 6;

            echo $x % $y;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_modulus)

## Assignment operator: x = y

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;  
            
            echo $x;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_set)

## Assignment operator: x += y

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 20;  
            $x += 100;

            echo $x;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_addition2)

## Assignment operator: x -= y

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 50;
            $x -= 30;

            echo $x;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_subtraction2)

## Assignment operator: x *= y

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 5;
            $x *= 6;

            echo $x;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_multiplication2)

## Assignment operator: x /= y

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;
            $x /= 5;

            echo $x;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_division2)

## Assignment operator: x %= y

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 15;
            $x %= 4;

            echo $x;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_modulus2)

## Comparison operator: Equal (==)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = "100";

            var_dump($x == $y); // Returns true because values are equal
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_equal)

## Comparison operator: Identical (===)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = "100";

            var_dump($x === $y); // Returns false because types are not equal
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_identical)

## Comparison operator: Not equal (!=)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = "100";

            var_dump($x != $y); // Returns false because values are equal
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_not_equal)

## Comparison operator: Not equal (<>)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = "100";

            var_dump($x <> $y); // Returns false because values are equal
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_not_equal2)

## Comparison operator: Not identical (!==)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = "100";

            var_dump($x !== $y); // Returns true because types are not equal
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_not_identical)

## Comparison operator: Greater than (>)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;
            $y = 50;

            var_dump($x > $y); // Returns true because $x is greater than $y
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_greater_than)

## Comparison operator: Less than (<)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;
            $y = 50;

            var_dump($x < $y); // Returns true because $x is less than $y
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_less_than)

## Comparison operator: Greater than or equal (>=)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 50;
            $y = 50;

            var_dump($x >= $y); // Returns true because $x is greater than or equal to $y
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_greater_than2)

## Comparison operator: Less than or equal (<=)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 50;
            $y = 50;

            var_dump($x <= $y); // Returns true because $x is less than or equal to $y
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_less_than2)

## Comparison operator: Spaceship (<=>)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 5;  
            $y = 10;

            echo ($x <=> $y); // Returns -1 because $x is less than $y
            echo "<br>";

            $x = 10;  
            $y = 10;

            echo ($x <=> $y); // Returns 0 because values are equal
            echo "<br>";

            $x = 15;  
            $y = 10;

            echo ($x <=> $y); // Returns +1 because $x is greater than $y
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_spaceship)

## Increment operator: ++$x

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;
            
            echo ++$x;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_pre_incr)

## Increment operator: $x++

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;  
            
            echo $x++;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_post_incr)

## Decrement operator: --$x

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;  
            
            echo --$x;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_pre_decr)

## Decrement operator: $x--

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 10;  
            
            echo $x--;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_post_decr)

## Logical operator: and

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = 50;

            if ($x == 100 and $y == 50) {
                echo "Hello world!";
            }
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_and)

## Logical operator: or

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = 50;

            if ($x == 100 or $y == 80) {
                echo "Hello world!";
            }
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_or)

## Logical operator: xor

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = 50;

            if ($x == 100 xor $y == 80) {
                echo "Hello world!";
            }
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_xor)

## Logical operator: && (and)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = 50;

            if ($x == 100 && $y == 50) {
                echo "Hello world!";
            }
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_and2)

## Logical operator: || (or)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  
            $y = 50;

            if ($x == 100 || $y == 80) {
                echo "Hello world!";
            }
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_or2)

## Logical operator: not

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = 100;  

            if ($x !== 90) {
                echo "Hello world!";
            }
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_not)

## String operator: Concatenation of $txt1 and $txt2

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $txt1 = "Hello";
            $txt2 = " world!";
            
            echo $txt1 . $txt2;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_string1)

## String operator: Appends $txt2 to $txt1

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $txt1 = "Hello";
            $txt2 = " world!";
            $txt1 .= $txt2;
            
            echo $txt1;
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_string2)

## Array operator: Union (+)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = array("a" => "red", "b" => "green");  
            $y = array("c" => "blue", "d" => "yellow");  

            print_r($x + $y); // Union of $x and $y
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_arr_union)

## Array operator: Equality (==)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = array("a" => "red", "b" => "green");  
            $y = array("c" => "blue", "d" => "yellow");  

            var_dump($x == $y);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_arr_equality)

## Array operator: Identity (===)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = array("a" => "red", "b" => "green");  
            $y = array("c" => "blue", "d" => "yellow");  

            var_dump($x === $y);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_arr_identity)

## Array operator: Inequality (!=)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = array("a" => "red", "b" => "green");  
            $y = array("c" => "blue", "d" => "yellow");  

            var_dump($x != $y);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_arr_inequality)

## Array operator: Inequality (<>)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = array("a" => "red", "b" => "green");  
            $y = array("c" => "blue", "d" => "yellow");  

            var_dump($x <> $y);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_arr_inequality2)

## Array operator: Non-identity (!==)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = array("a" => "red", "b" => "green");  
            $y = array("c" => "blue", "d" => "yellow");  

            var_dump($x !== $y);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_arr_non_identity)

## Conditional assignment operator: Ternary (?:)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // If empty($user) = TRUE, set $status = "anonymous"
            echo $status = (empty($user)) ? "anonymous" : "logged in";
            echo("<br>");

            $user = "John Doe";
            // If empty($user) = FALSE, set $status = "logged in"
            echo $status = (empty($user)) ? "anonymous" : "logged in";
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_ternary)

## Conditional assignment: Null coalescing (??)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Variable $user is the value of $_GET['user']
            // and 'anonymous' if it does not exist
            echo $user = $_GET["user"] ?? "anonymous";
            echo("<br>");
            
            // Variable $color is "red" if $color does not exist or is null
            echo $color = $color ?? "red";
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_oper_null_coalescing)