# Sorting Arrays

## sort() - Sort array in ascending alphabetical order

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $cars = array("Volvo", "BMW", "Toyota");

            sort($cars);
            $clength = count($cars);
            
            for($x = 0; $x < $clength; $x++) {
                echo $cars[$x];
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_sort_alpha)

## sort() - Sort array in ascending numerical order

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $numbers = array(4, 6, 2, 22, 11);

            sort($numbers);
            $arrlength = count($numbers);
            
            for($x = 0; $x < $arrlength; $x++) {
                echo $numbers[$x];
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_sort_num)

## rsort() - Sort array in descending alphabetical order

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $cars = array("Volvo", "BMW", "Toyota");

            rsort($cars);
            $clength = count($cars);
            
            for($x = 0; $x < $clength; $x++) {
                echo $cars[$x];
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_rsort_alpha)

## rsort() - Sort array in descending numerical order

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $numbers = array(4, 6, 2, 22, 11);

            rsort($numbers);
            $arrlength = count($numbers);
            
            for($x = 0; $x < $arrlength; $x++) {
                echo $numbers[$x];
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_rsort_num)

## asort() - Sort array in ascending order, according to value

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");
            
            asort($age);

            foreach($age as $x => $x_value) {
                echo "Key=" . $x . ", Value=" . $x_value;
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_asort)

## ksort() - Sort array in ascending order, according to key

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");
            
            ksort($age);

            foreach($age as $x => $x_value) {
                echo "Key=" . $x . ", Value=" . $x_value;
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_ksort)

## arsort() - Sort array in descending order, according to value

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");
            
            arsort($age);

            foreach($age as $x => $x_value) {
                echo "Key=" . $x . ", Value=" . $x_value;
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_arsort)

## krsort() - Sort array in descending order, according to key

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");
            
            krsort($age);

            foreach($age as $x => $x_value) {
                echo "Key=" . $x . ", Value=" . $x_value;
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_array_krsort)