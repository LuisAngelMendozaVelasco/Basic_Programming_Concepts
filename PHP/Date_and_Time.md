# Date and Time

## Format today's date in several ways

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo "Today is " . date("Y/m/d") . "<br>";
            echo "Today is " . date("Y.m.d") . "<br>";
            echo "Today is " . date("Y-m-d") . "<br>";
            echo "Today is " . date("l");
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_date1)

## Automatically update the copyright year on your website

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        © 2010-<?php echo date("Y");?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_date_copyright)

## Output the current time (server time)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            date_default_timezone_set('America/Mexico_City');

            echo "The time is " . date("h:i:sa");
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_date2)

## Set timezone, then output current time

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            date_default_timezone_set("America/New_York");
            
            echo "The time is " . date("h:i:sa");
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_date3)

## Create a date and time from a number of parameters in mktime()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $d = mktime(11, 14, 54, 8, 12, 2014);
            
            echo "Created date is " . date("Y-m-d h:i:sa", $d);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_date4)

## Create a date and time from the strtotime() function

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $d = strtotime("10:30pm April 15 2014");
            
            echo "Created date is " . date("Y-m-d h:i:sa", $d);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_date5)

## Create more dates/times from strtotime()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
        $d = strtotime("tomorrow");
        echo date("Y-m-d h:i:sa", $d) . "<br>";

        $d = strtotime("next Saturday");
        echo date("Y-m-d h:i:sa", $d) . "<br>";

        $d = strtotime("+3 Months");
        echo date("Y-m-d h:i:sa", $d) . "<br>";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_date6)

## Output the dates for the next six Saturdays

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $startdate = strtotime("Saturday");
            $enddate = strtotime("+6 weeks", $startdate);

            while ($startdate < $enddate) {
                echo date("M d", $startdate) . "<br>";
                $startdate = strtotime("+1 week", $startdate);
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_date7)

## Output the number of days until 4th of July

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $d1 = strtotime("July 04");
            $d2 = ceil(($d1-time())/60/60/24);

            echo "There are " . $d2 . " days until 4th of July.";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/phptryit.asp?filename=tryphp_date8)