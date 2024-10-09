# Exceptions

## Throw an Exception

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function divide($dividend, $divisor) {
                if($divisor == 0) {
                    throw new Exception("Division by zero");
                }
                return $dividend / $divisor;
            }

            echo divide(5, 0);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_exceptions_throw)

## Use try..catch to show a message when an exception is thrown

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function divide($dividend, $divisor) {
                if($divisor == 0) {
                    throw new Exception("Division by zero");
                }
                return $dividend / $divisor;
            }

            try {
                echo divide(5, 0);
            } 
            catch(Exception $e) {
                echo "Unable to divide.";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_exceptions_try_catch)

## Use finally

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function divide($dividend, $divisor) {
                if($divisor == 0) {
                    throw new Exception("Division by zero");
                }
                return $dividend / $divisor;
            }

            try {
                echo divide(5, 0);
            } 
            catch(Exception $e) {
                echo "Unable to divide. <br>";
            } 
            finally {
                echo "Process complete.";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_exceptions_finally)

## Output information about an exception that was thrown

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            function divide($dividend, $divisor) {
                if($divisor == 0) {
                    throw new Exception("Division by zero", 1);
                }
                return $dividend / $divisor;
            }

            try {
                echo divide(5, 0);
            } 
            catch(Exception $ex) {
                $code = $ex->getCode();
                $message = $ex->getMessage();
                $file = $ex->getFile();
                $line = $ex->getLine();
                echo "Exception thrown in $file on line $line: [Code $code] $message";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_exceptions_obj_info)