# Sessions

## Start a session

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Set session variables
            $_SESSION["favcolor"] = "green";
            $_SESSION["favanimal"] = "cat";
            
            echo "Session variables are set.";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_session1)

## Get session variable values

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Echo session variables that were set on previous page
            echo "Favorite color is " . $_SESSION["favcolor"] . ".<br>";
            echo "Favorite animal is " . $_SESSION["favanimal"] . ".";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_session2)

## Get all session variable values

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            print_r($_SESSION);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_session3)

## Modify a session variable

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // To change a session variable, just overwrite it
            $_SESSION["favcolor"] = "yellow";
            
            print_r($_SESSION);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_session4)

## Destroy a session

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Remove all session variables
            session_unset();

            // Destroy the session
            session_destroy();

            echo "All session variables are now removed, and the session is destroyed."
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_session5)