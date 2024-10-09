# Superglobals

## $GLOBAL - Used to access global variables from anywhere in the PHP script

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php 
            $x = 75;
            $y = 25; 

            function addition() {
                $GLOBALS['z'] = $GLOBALS['x'] + $GLOBALS['y'];
            }

            addition();
            echo $z;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_global_global)

## $_SERVER - Holds information about headers, paths, and script locations

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php 
            echo $_SERVER['PHP_SELF'];
            echo "<br>";
            echo $_SERVER['SERVER_NAME'];
            echo "<br>";
            echo $_SERVER['HTTP_HOST'];
            echo "<br>";
            echo $_SERVER['HTTP_REFERER'];
            echo "<br>";
            echo $_SERVER['HTTP_USER_AGENT'];
            echo "<br>";
            echo $_SERVER['SCRIPT_NAME'];
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_global_server)

## $_REQUEST - Used to collect data after submitting an HTML form

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <form method="post" action="<?php echo $_SERVER['PHP_SELF'];?>">
            Name: <input type="text" name="fname"> <input type="submit">
        </form>

        <?php
            if ($_SERVER["REQUEST_METHOD"] == "POST") {
                // Collect value of input field
                $name = htmlspecialchars($_REQUEST['fname']); 

                if (empty($name)) {
                    echo "Name is empty";
                } 
                else {
                    echo $name;
                }
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_global_request)

## $_POST - Used to collect form data after submitting an HTML form. Also used to pass variables

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <form method="post" action="<?php echo $_SERVER['PHP_SELF'];?>">
            Name: <input type="text" name="fname"> <input type="submit">
        </form>

        <?php
            if ($_SERVER["REQUEST_METHOD"] == "POST") {
                // Collect value of input field
                $name = $_POST['fname']; 
                
                if (empty($name)) {
                    echo "Name is empty";
                } 
                else {
                    echo $name;
                }
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_global_post)

## $_GET - Collect data sent in the URL

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <a href="test_get.php?subject=PHP&web=W3schools.com">Test $GET</a>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_global_get)