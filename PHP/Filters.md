# Filters

## Use filter_list() to list what the PHP filter extension offers

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}

            th, td {padding: 5px;}
        </style>
    </head>
    <body>
        <table>
            <tr>
                <td>Filter Name</td>
                <td>Filter ID</td>
            </tr>
            <?php
                foreach (filter_list() as $id => $filter) {
                    echo '<tr><td>' . $filter . '</td><td>' . filter_id($filter) . '</td></tr>';
                }
            ?>
        </table>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_filter1)

## Sanitize a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $str = "<h1>Hello World!</h1>";
            // $newstr = filter_var($str, FILTER_SANITIZE_STRING); // 'FILTER_SANITIZE_STRING' is deprecated.
            $newstr = filter_var($str, 513);

            echo $newstr;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_filter2)

## Validate an integer

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $int = 100;
            
            if (!filter_var($int, FILTER_VALIDATE_INT) === false) {
                echo("Integer is valid");
            } 
            else {
                echo("Integer is not valid");
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_filter3)

## Validate an integer that is 0

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $int = 0;

            if (filter_var($int, FILTER_VALIDATE_INT) === 0 || !filter_var($int, FILTER_VALIDATE_INT) === false) {
                echo("Integer is valid");
            } 
            else {
                echo("Integer is not valid");
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_filter4)

## Validate an IP address

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $ip = "127.0.0.1";

            if (!filter_var($ip, FILTER_VALIDATE_IP) === false) {
                echo("$ip is a valid IP address");
            } 
            else {
                echo("$ip is not a valid IP address");
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_filter5)

## Sanitize and validate an email address

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $email = "luis.mendoza@example.com";

            // Remove all illegal characters from email
            $email = filter_var($email, FILTER_SANITIZE_EMAIL);

            // Validate e-mail
            if (!filter_var($email, FILTER_VALIDATE_EMAIL) === false) {
                echo("$email is a valid email address");
            } 
            else {
                echo("$email is not a valid email address");
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_filter6)

## Sanitize and validate a URL

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $url = "https://www.w3schools.com";

            // Remove all illegal characters from a url
            $url = filter_var($url, FILTER_SANITIZE_URL);

            // Validate url
            if (!filter_var($url, FILTER_VALIDATE_URL) === false) {
                echo("$url is a valid URL");
            } 
            else {
                echo("$url is not a valid URL");
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_filter7)