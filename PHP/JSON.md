# JSON

## Encode an associative array into a JSON object

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $age = array("Peter"=>35, "Ben"=>37, "Joe"=>43);

            echo json_encode($age);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/showphp.asp?filename=demo_json_encode1)

## Decode JSON data into a PHP object

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $jsonobj = '{"Peter":35,"Ben":37,"Joe":43}';
            
            var_dump(json_decode($jsonobj));
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/showphp.asp?filename=demo_json_decode1)

## Access the values from a PHP object

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $jsonobj = '{"Peter":35, "Ben":37, "Joe":43}';
            $obj = json_decode($jsonobj);

            echo $obj->Peter . ", ";
            echo $obj->Ben . ", ";
            echo $obj->Joe;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/showphp.asp?filename=demo_json_decode3)

## Loop through the values of a PHP object

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $jsonobj = '{"Peter":35, "Ben":37, "Joe":43}';
            $obj = json_decode($jsonobj);

            foreach($obj as $key => $value) {
                echo $key . " => " . $value . "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://www.w3schools.com/php/showphp.asp?filename=demo_json_decode5)