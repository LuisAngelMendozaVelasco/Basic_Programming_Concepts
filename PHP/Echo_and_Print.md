# Echo and Print

## Display strings with the echo command

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo "<h2>PHP is Fun!</h2>";
            echo "Hello world!<br>";
            echo "I'm about to learn PHP!<br>";
            echo "This ", "string ", "was ", "made ", "with multiple parameters.";
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_echo1)

## Display strings and variables with the echo command

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $txt1 = "Learn PHP";
            $txt2 = "W3Schools.com";
            $x = 5;
            $y = 4;

            echo "<h2>" . $txt1 . "</h2>";
            echo "Study PHP at " . $txt2 . "<br>";
            echo $x + $y;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_echo2)

## Display strings with the print command

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            print "<h2>PHP is Fun!</h2>";
            print "Hello world!<br>";
            print "I'm about to learn PHP!";
        ?> 
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_print1)

## Display strings and variables with the print command

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $txt1 = "Learn PHP";
            $txt2 = "W3Schools.com";
            $x = 5;
            $y = 4;

            print "<h2>" . $txt1 . "</h2>";
            print "Study PHP at " . $txt2 . "<br>";
            print $x + $y;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_print2)