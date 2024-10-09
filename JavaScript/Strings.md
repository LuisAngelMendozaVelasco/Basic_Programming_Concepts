# Strings

## Strings can be written with single or double quotes

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Strings</h1>

        <p>Strings are written inside quotes.</p>
        <p>You can use single or double quotes:</p>

        <p id="demo"></p>

        <script>
            var carName1 = "Volvo XC60";
            var carName2 = 'Volvo XC60';

            document.getElementById("demo").innerHTML = carName1 + " " + carName2; 
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_1.html)

## Show some string examples

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Strings</h2>

        <p>You can use quotes inside a string, as long as they don't match the quotes surrounding the string:</p>

        <p id="demo"></p>

        <script>
            let answer1 = "It's alright";
            let answer2 = "He is called 'Johnny'";
            let answer3 = 'He is called "Johnny"';

            document.getElementById("demo").innerHTML = answer1 + "<br>" + 
                                                        answer2 + "<br>" + 
                                                        answer3;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_2.html)

## Backslash before quotes accepts quotes as quotes

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p id="demo"></p>

        <script>
            var x = 'It\'s alright';
            var y = "We are the so-called \"Vikings\" from the north.";

            document.getElementById("demo").innerHTML = x + "<br>" + y; 
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_3.html)

## Find the length of a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Strings</h1>
        <h2>The length Property</h2>

        <p>The length of the string is:</p>
        <p id="demo"></p>

        <script>
            let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
            
            document.getElementById("demo").innerHTML = text.length;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_4.html)

## You can break text string with a backslash

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Strings</h2>

        <p>You can break a code line within a text string with a backslash.</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = "Hello \
                                                        Dolly!";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_5.html)

## You cannot break code with a backslash

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Statements</h2>

        <p id="demo">You cannot break a code line with a \ backslash.</p>

        <script>
            document.getElementById("demo").innerHTML = \
                                                        "Hello Dolly.";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_6.html)

## Find the position of the first occurrence of a text in a string - indexOf()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Strings</h1>
        <h2>The indexOf() Method</h2>

        <p>The position of the first occurrence of "locate" is:</p>
        <p id="demo"></p>

        <script>
            let text = "Please locate where 'locate' occurs!";
            
            document.getElementById("demo").innerHTML = text.indexOf("locate");
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_7.html)

## Search for a text in a string and return the text if found - match()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Click the button to perfom a global (/g) search for the letters "ain" (/ain) in a string, and display the matches.</p>

        <button onclick="myFunction()">Try it</button>

        <p id="demo"></p>

        <script>
            function myFunction() {
                var str = "The rain in SPAIN stays mainly in the plain"; 
                var res = str.match(/ain/g);
                
                document.getElementById("demo").innerHTML = res;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_8.html)

## Replace characters in a string - replace()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript String Methods</h1>
        <p>Replace "Microsoft" with "W3Schools" in the paragraph below:</p>

        <button onclick="myFunction()">Try it</button>

        <p id="demo">Please visit Microsoft!</p>

        <script>
            function myFunction() {
                let text = document.getElementById("demo").innerHTML;
                
                document.getElementById("demo").innerHTML = text.replace("Microsoft", "W3Schools");
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_9.html)

## Convert string to upper case - toUpperCase()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript String Methods</h1>
        <p>Convert string to upper case:</p>

        <button onclick="myFunction()">Try it</button>

        <p id="demo">Hello World!</p>

        <script>
            function myFunction() {
                let text = document.getElementById("demo").innerHTML;
                
                document.getElementById("demo").innerHTML = text.toUpperCase();
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_10.html)

## Convert string to lower case - toLowerCase()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript String Methods</h1>
        <p>Convert string to lower case:</p>

        <button onclick="myFunction()">Try it</button>

        <p id="demo">Hello World!</p>

        <script>
            function myFunction() {
                let text = document.getElementById("demo").innerHTML;
                
                document.getElementById("demo").innerHTML = text.toLowerCase();
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_11.html)

## Split a string into an array - split()

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript String Methods</h1>
        <p>Display the first array element, after a string split:</p>

        <p id="demo"></p>

        <script>
            let text = "a,b,c,d,e,f";
            const myArray = text.split(",");
            
            document.getElementById("demo").innerHTML = myArray[0];
        </script>
    </body>
</html>
```

Output:

[Click here!](./Strings/Example_12.html)