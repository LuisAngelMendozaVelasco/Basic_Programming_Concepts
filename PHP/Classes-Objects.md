# Classes-Objects

## Define a class and an object

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class Fruit {
                // Properties
                public $name;
                public $color;

                function __construct() {}

                // Methods
                function set_name($name) {
                    $this->name = $name;
                }

                function get_name() {
                    return $this->name;
                }
            }

            $apple = new Fruit();
            $banana = new Fruit();
            $apple->set_name('Apple');
            $banana->set_name('Banana');

            echo $apple->get_name();
            echo "<br>";
            echo $banana->get_name();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_class2)

## Using the $this keyword

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class Fruit {
                public $name;

                function __construct() {}

                function set_name($name) {
                    $this->name = $name;
                }
            }

            $apple = new Fruit();
            $apple->set_name("Apple");

            echo $apple->name;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_this)

## Using the instanceof keyword

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class Fruit {
                // Properties
                public $name;
                public $color;

                function __construct() {}

                // Methods
                function set_name($name) {
                    $this->name = $name;
                }

                function get_name() {
                    return $this->name;
                }
            }

            $apple = new Fruit();
            var_dump($apple instanceof Fruit);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_class4)

## Creating a constructor

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class Fruit {
                public $name;
                public $color;

                function __construct($name) {
                    $this->name = $name; 
                }
                
                function get_name() {
                    return $this->name;
                }
            }

            $apple = new Fruit("Apple");
            echo $apple->get_name();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_constructor)

## Creating a destructor

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class Fruit {
                public $name;
                public $color;

                function __construct($name) {
                    $this->name = $name; 
                }
                
                function __destruct() {
                    echo "The fruit is {$this->name}."; 
                }
            }

            $apple = new Fruit("Apple");
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_destructor)

## Inheritance

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class Fruit {
                public $name;
                public $color;

                public function __construct($name, $color) {
                    $this->name = $name;
                    $this->color = $color; 
                }
                
                public function intro() {
                    echo "The fruit is {$this->name} and the color is {$this->color}."; 
                }
            }

            // Strawberry is inherited from Fruit
            class Strawberry extends Fruit {
                public function message() {
                    echo "Am I a fruit or a berry? "; 
                }
            }

            $strawberry = new Strawberry("Strawberry", "red");
            $strawberry->message();
            $strawberry->intro();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_inheritance)

## Class constants

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class Goodbye {
                const LEAVING_MESSAGE = "Thank you for visiting W3Schools.com!";
            }

            echo Goodbye::LEAVING_MESSAGE;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_class_constant)

## Abstract classes

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            // Parent class
            abstract class Car {
                public $name;

                public function __construct($name) {
                    $this->name = $name;
                }
                
                abstract public function intro() : string; 
            }

            // Child classes
            class Audi extends Car {
                public function intro() : string {
                    return "Choose German quality! I'm an $this->name!"; 
                }
            }

            class Volvo extends Car {
                public function intro() : string {
                    return "Proud to be Swedish! I'm a $this->name!"; 
                }
            }

            class Citroen extends Car {
                public function intro() : string {
                    return "French extravagance! I'm a $this->name!"; 
                }
            }

            // Create objects from the child classes
            $audi = new audi("Audi");
            echo $audi->intro();
            echo "<br>";

            $volvo = new volvo("Volvo");
            echo $volvo->intro();
            echo "<br>";

            $citroen = new citroen("Citroen");
            echo $citroen->intro();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_abstract)

## Traits

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            trait message1 {
                public function msg1() {
                    echo "OOP is fun! "; 
                }
            }

            class Welcome {
                use message1;
            }

            $obj = new Welcome();
            $obj->msg1();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_trait)

## Static method

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class greeting {
                public static function welcome() {
                    echo "Hello World!";
                }
            }

            // Call static method
            greeting::welcome();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_static_method)

## Static property

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            class pi {
                public static $value = 3.14159;
            }

            // Get static property
            echo pi::$value;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_static_prop)