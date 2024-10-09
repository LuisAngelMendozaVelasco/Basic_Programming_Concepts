# SimpleXML Parser

## Use simplexml_load_string() to read XML data from a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $myXMLData =    "<?xml version='1.0' encoding='UTF-8'?>
                            <note>
                                <to>Tove</to>
                                <from>Jani</from>
                                <heading>Reminder</heading>
                                <body>Don't forget me this weekend!</body>
                            </note>";

            $xml = simplexml_load_string($myXMLData) or die("Error: Cannot create object");
            print_r($xml);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_simplexml_read_string)

## Use simplexml_load_file() to read XML data from a file

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $xml = simplexml_load_file("./note.xml") or die("Error: Cannot create object");

            print_r($xml);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_simplexml_read_file)

## Get node values

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $xml=simplexml_load_file("./note.xml") or die("Error: Cannot create object");

            echo $xml->to . "<br>";
            echo $xml->from . "<br>";
            echo $xml->heading . "<br>";
            echo $xml->body;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_simplexml_get_one)

## Get node values of specific elements

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $xml = simplexml_load_file("./books.xml") or die("Error: Cannot create object");
            
            echo $xml->book[0]->title . "<br>";
            echo $xml->book[1]->title;
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_simplexml_get_many1)

## Get node values - loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $xml = simplexml_load_file("./books.xml") or die("Error: Cannot create object");
            
            foreach($xml->children() as $books) {
                echo $books->title . ", ";
                echo $books->author . ", ";
                echo $books->year . ", ";
                echo $books->price . "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_simplexml_get_many2)

## Get attribute values

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $xml = simplexml_load_file("./books.xml") or die("Error: Cannot create object");

            echo $xml->book[0]['category'] . "<br>";
            echo $xml->book[1]->title['lang'];
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_simplexml_get_attr1)

## Get attribute values - loop

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $xml=simplexml_load_file("./books.xml") or die("Error: Cannot create object");

            foreach($xml->children() as $books) {
                echo $books->title['lang'];
                echo "<br>";
            }
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_simplexml_get_attr2)