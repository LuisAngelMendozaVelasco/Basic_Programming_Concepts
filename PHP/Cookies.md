# Cookies

## Create and retrieve a cookie

Code: 

```html
<!DOCTYPE html>
<?php
    $cookie_name = "user";
    $cookie_value = "Luis Mendoza";
    setcookie($cookie_name, $cookie_value, time() + (60*60*24*30), "/"); // 60*60*24*30 = 30 days
?>
<html>
    <body>
        <?php
            if(!isset($_COOKIE[$cookie_name])) {
                echo "Cookie named '" . $cookie_name . "' is not set!";
            } 
            else {
                echo "Cookie '" . $cookie_name . "' is set!<br>";
                echo "Value is: " . $_COOKIE[$cookie_name];
            }
        ?>
        <p><strong>Note:</strong> You might have to reload the page to see the value of the cookie.</p>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_cookie1)

## Modify a cookie value

Code: 

```html
<!DOCTYPE html>
<?php
    $cookie_name = "user";
    $cookie_value = "Angel Velasco";
    setcookie($cookie_name, $cookie_value, time() + (60*60*24*30), "/");
?>
<html>
    <body>
        <?php
            if(!isset($_COOKIE[$cookie_name])) {
                echo "Cookie named '" . $cookie_name . "' is not set!";
            } 
            else {
                echo "Cookie '" . $cookie_name . "' is set!<br>";
                echo "Value is: " . $_COOKIE[$cookie_name];
            }
        ?>
        <p><strong>Note:</strong> You might have to reload the page to see the new value of the cookie.</p>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_cookie3)

## Delete a cookie

Code: 

```html
<!DOCTYPE html>
<?php
    // Set the expiration date to one hour ago
    setcookie("user", "", time() - 3600);
?>
<html>
    <body>
        <?php
            echo "Cookie 'user' is deleted.";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_cookie4)

## Check if cookies are enabled

Code: 

```html
<!DOCTYPE html>
<?php
    setcookie("test_cookie", "test", time() + 3600, '/');
?>
<html>
    <body>
        <?php
            if(count($_COOKIE) > 0) {
                echo "Cookies are enabled.";
            } 
            else {
                echo "Cookies are disabled.";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_cookie5)