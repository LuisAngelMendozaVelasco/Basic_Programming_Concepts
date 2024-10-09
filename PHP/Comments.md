# Comments

## Syntax for single-line comments

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // This is a single-line comment
            # This is also a single-line comment
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_comments)

## Syntax for multi-line comments

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            /*
            This is a multiple-lines comment block
            that spans over multiple
            lines
            */
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_comments2)

## Using comments to leave out parts of the code

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // You can also use comments to leave out parts of a code line
            $x = 5 /* + 15 */ + 5;
            
            echo $x;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_comments3)