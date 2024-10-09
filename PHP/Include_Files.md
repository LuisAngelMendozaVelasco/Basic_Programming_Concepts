# Include Files

## Use include to include "footer.php" in a page

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Welcome to my home page!</h1>
        <p>Some text.</p>
        <p>Some more text.</p>
        
        <?php include 'footer.php';?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_include1)

## Use include to include "menu.php" in a page

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <div class="menu">
            <?php include 'menu.php';?>
        </div>

        <h1>Welcome to my home page!</h1>
        <p>Some text.</p>
        <p>Some more text.</p>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_include2)

## Use include to include "vars.php" in a page

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Welcome to my home page!</h1>
        
        <?php 
            include 'vars.php';
            echo "I have a $color $car.";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_include3)

## Use include to include a non-existing file

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Welcome to my home page!</h1>
        
        <?php 
            include 'noFileExists.php';
            echo "I have a $color $car.";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_include4)

## Use require to include a non-existing file

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Welcome to my home page!</h1>
        
        <?php 
            require 'noFileExists.php';
            echo "I have a $color $car.";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_include5)