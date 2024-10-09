# Number Methods

## The toString() method converts a number to a string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>The toString() method can output numbers from base 2 to 36:</p>

        <p id="demo"></p>

        <script>
            let myNumber = 32;
            document.getElementById("demo").innerHTML = "Decimal 32 = " + "<br><br>" + 
                                                        "Hexatrigesimal (base 36): " + myNumber.toString(36) + "<br>" +
                                                        "Duotrigesimal (base 32): " + myNumber.toString(32) + "<br>" +
                                                        "Hexadecimal (base 16): " + myNumber.toString(16) + "<br>" +
                                                        "Duodecimal (base 12): " + myNumber.toString(12) + "<br>" +
                                                        "Decimal (base 10): " + myNumber.toString(10) + "<br>" +
                                                        "Octal (base 8): " + myNumber.toString(8) + "<br>" +
                                                        "Binary (base 2): " + myNumber.toString(2);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_1.html)

## The valueOf() method returns a number as a number

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Number Methods</h2>

        <p>The valueOf() method returns a number as a number():</p>

        <p id="demo"></p>

        <script>
            let x = 123;

            document.getElementById("demo").innerHTML = x.valueOf() + "<br>" +
                                                        (123).valueOf() + "<br>" +
                                                        (100 + 23).valueOf();
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_2.html)

## The toExponential() returns a number with exponential notation

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Number Methods</h2>

        <p>The toExponential() method returns a string, with the number rounded and written using exponential notation.</p>

        <p>An optional parameter defines the number of digits behind the decimal point.</p>

        <p id="demo"></p>

        <script>
            let x = 9.656;
            
            document.getElementById("demo").innerHTML = x.toExponential() + "<br>" + 
                                                        x.toExponential(2) + "<br>" + 
                                                        x.toExponential(4) + "<br>" + 
                                                        x.toExponential(6);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_3.html)

## The toFixed() method rounds a number to a number of digits

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Number Methods</h2>

        <p>The toFixed() method rounds a number to a given number of digits.</p>
        <p>For working with money, toFixed(2) is perfect.</p>

        <p id="demo"></p>

        <script>
            let x = 9.656;
            
            document.getElementById("demo").innerHTML = x.toFixed(0) + "<br>" +
                                                        x.toFixed(2) + "<br>" +
                                                        x.toFixed(4) + "<br>" +
                                                        x.toFixed(6);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_4.html)

## The toPrecision() method a number written with a specified length

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Number Methods</h2>

        <p>The toPrecision() method returns a string, with a number written with a specified length:</p>

        <p id="demo"></p>

        <script>
            let x = 9.656;
            
            document.getElementById("demo").innerHTML = x.toPrecision() + "<br>" +
                                                        x.toPrecision(2) + "<br>" +
                                                        x.toPrecision(4) + "<br>" +
                                                        x.toPrecision(6);  
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_5.html)

## The global method Number() converts variables to numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Global Methods</h2>

        <p>The Number() method converts variables to numbers:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Number(true) + "<br>" +
                                                        Number(false) + "<br>" +
                                                        Number("10") + "<br>" + 
                                                        Number("  10") + "<br>" +
                                                        Number("10  ") + "<br>" +
                                                        Number(" 10  ") + "<br>" +
                                                        Number("10.33") + "<br>" + 
                                                        Number("10,33") + "<br>" +
                                                        Number("10 33") + "<br>" +
                                                        Number("John");
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_6.html)

## The global method Number() can even convert dates to numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Global Methods</h2>

        <p>The Number() method can convert a date to a number:</p>

        <p id="demo"></p>

        <script>
            let x = new Date("2017-09-30");
            
            document.getElementById("demo").innerHTML = Number(x); 
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_7.html)

## The global method parseInt() converts strings to numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Global Functions</h2>
        <h2>parseInt()</h2>
        <p>The global JavaScript function parseInt() converts strings to numbers:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = parseInt("-10") + "<br>" +
                                                        parseInt("-10.33") + "<br>" +
                                                        parseInt("10") + "<br>" +
                                                        parseInt("10.33") + "<br>" +
                                                        parseInt("10 6") + "<br>" +  
                                                        parseInt("10 years") + "<br>" +  
                                                        parseInt("years 10");  
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_8.html)

## The global method parseFloat() converts strings to numbers

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Global Methods</h2>

        <p>The parseFloat() method converts strings to numbers:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = parseFloat("10") + "<br>" +
                                                        parseFloat("10.33") + "<br>" +
                                                        parseFloat("10 6") + "<br>" +  
                                                        parseFloat("10 years") + "<br>" +
                                                        parseFloat("years 10");    
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_9.html)

## MAX_VALUE returns the largest possible number in JavaScript

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Numbers</h1>
        <h2>The MAX_VALUE Property</h2>

        <p>The largest possible number in JavaScript is:</p>
        <p id="demo"></p>

        <script>
            let x = Number.MAX_VALUE;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_10.html)

## MIN_VALUE returns the smallest possible number in JavaScript

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Numbers</h1>
        <h2>The MAX_VALUE Property</h2>

        <p>The smallest number possible in JavaScript is:</p>
        <p id="demo"></p>

        <script>
            let x = Number.MIN_VALUE;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_11.html)

## POSITIVE_INFINITY represents infinity

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Numbers</h1>
        <h2>The POSITIVE_INFINITY Property</h2>

        <p id="demo"></p>

        <script>
            let x = Number.POSITIVE_INFINITY;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_12.html)

## POSITIVE_INFINITY is returned on overflow

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Numbers</h1>
        <h2>The POSITIVE_INFINITY Property</h2>

        <p>POSITIVE_INFINITY is returned on overflow:</p>
        <p id="demo"></p>

        <script>
            let x = 1 / 0;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_13.html)

## NEGATIVE_INFINITY represents negative infinity

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Numbers</h1>
        <h2>The NEGATIVE_INFINITY Property</h2>

        <p></p>

        <p id="demo"></p>

        <script>
            let x = Number.NEGATIVE_INFINITY;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_14.html)

## NEGATIVE_INFINITY is returned on overflow

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Numbers</h1>
        <h2>The NEGATIVE_INFINITY Property</h2>

        <p>NEGATIVE_INFINITY is returned on overflow:</p>
        <p id="demo"></p>

        <script>
            let x = -1 / 0;
            
            document.getElementById("demo").innerHTML = x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_15.html)

## NaN Represents "Not-a-Number"

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Number Properties</h2>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = Number.NaN;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_16.html)

## Arithmetic performed on a string will result in NaN

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>A number divided by a non-numeric string becomes NaN (Not a Number):</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = 100 / "Apple";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_17.html)

## Using a Number property on a variable will return undefined

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Number Properties</h1>

        <p>Using a Number property on a variable, or value, will return undefined:</p>

        <p id="demo"></p>

        <script>
            let x = 6;
            
            document.getElementById("demo").innerHTML = x.MAX_VALUE;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Number_Methods/Example_18.html)