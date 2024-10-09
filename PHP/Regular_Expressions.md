# Regular Expressions

## Do a case-insensitive search for "w3schools" in a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $str = "Visit W3Schools";
            $pattern = "/w3schools/i";
            
            echo preg_match($pattern, $str); 
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_regex_match)

## Do a case-insensitive count of the number of occurrences of "ain" in a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $str = "The rain in SPAIN falls mainly on the plains.";
            $pattern = "/ain/i";
            
            echo preg_match_all($pattern, $str);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_regex_match_all)

## Replace "Microsoft" with "W3Schools" in a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $str = "Visit Microsoft!";
            $pattern = "/microsoft/i";
            
            echo preg_replace($pattern, "W3Schools", $str);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_regex_replace)