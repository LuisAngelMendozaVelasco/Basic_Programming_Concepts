# File Open-Read-Close

## Use fopen(), fread(), and fclose() to open, read, and close a file

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $myfile = fopen("webdictionary.txt", "r") or die("Unable to open file!");
            
            echo fread($myfile, filesize("webdictionary.txt"));
            fclose($myfile);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_file_fopen)

## Use fgets() to read a single line from a file

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $myfile = fopen("webdictionary.txt", "r") or die("Unable to open file!");
            
            echo fgets($myfile);
            fclose($myfile);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_file_fgets)

## Use feof() to read through a file, line by line, until end-of-file is reached

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $myfile = fopen("webdictionary.txt", "r") or die("Unable to open file!");

            // Output one line until end-of-file
            while(!feof($myfile)) {
                echo fgets($myfile) . "<br>";
            }
            
            fclose($myfile);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_file_feof)

## Use fgetc() to read a single character from a file

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $myfile = fopen("webdictionary.txt", "r") or die("Unable to open file!");

            // Output one character until end-of-file
            while(!feof($myfile)) {
                echo fgetc($myfile);
            }
            
            fclose($myfile);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphp.php?filename=demo_file_fgetc)