# Data Types

## PHP string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php 
            $x = "Hello world!";
            $y = 'Hello world!';

            echo $x;
            echo "<br>"; 
            echo $y;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_datatypes_string)

## PHP integer

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php  
            $x = 5985;
            
            var_dump($x);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_datatypes_integer)

## PHP float

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php  
            $x = 10.365;
            
            var_dump($x);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_datatypes_float)

## PHP array

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php  
            $cars = array("Volvo", "BMW", "Toyota");
            
            var_dump($cars);
        ?>  
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_datatypes_array)

## PHP object

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class Car {
                public $color;
                public $model;
                
                public function __construct($color, $model) {
                    $this->color = $color;
                    $this->model = $model;
                }

                public function message() {
                    return "My car is a " . $this->color . " " . $this->model . "!";
                }
            }

            $myCar = new Car("black", "Volvo");
            echo $myCar -> message();
            echo "<br>";
            $myCar = new Car("red", "Toyota");
            echo $myCar -> message();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_datatypes_object)

## PHP NULL value

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $x = "Hello world!";
            $x = null;
            
            var_dump($x);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_datatypes_null)