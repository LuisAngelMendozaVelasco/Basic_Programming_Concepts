# Numbers

## Numbers can be written with or without decimals

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Numbers can be written with or without decimals:</p>

        <p id="demo"></p>

        <script>
            let x = 3.14;
            let y = 3;
            
            document.getElementById("demo").innerHTML = x + "<br>" + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_1.html)

## Extra large or extra small numbers can be written with exponent notation

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Extra large or extra small numbers can be written with scientific (exponent) notation:</p>

        <p id="demo"></p>

        <script>
            let x = 123e5;
            let y = 123e-5;
            
            document.getElementById("demo").innerHTML = x + "<br>" + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_2.html)

## Number are considered accurate only up to 15 digits

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Numbers</h1>
        <h2>Integer Precision</h2>

        <p>Integers (numbers without a period or exponent notation) are accurate up to 15 digits:</p>

        <p id="demo"></p>

        <script>
            let x = 999999999999999;
            let y = 9999999999999999;
            
            document.getElementById("demo").innerHTML = x + "<br>" + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_3.html)

## Floating point arithmetic is not always 100% accurate

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>JavaScript Numbers</h1>
        <h2>Floating Point Precision</h2>

        <p>Floating point arithmetic is not always 100% accurate.</p>

        <p id="demo"></p>

        <script>
            let x = 0.2 + 0.1;
            
            document.getElementById("demo").innerHTML = "0.2 + 0.1 = " + x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_4.html)

## But it helps to multiply and divide by 10

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Floating point arithmetic is not always 100% accurate:</p>
        <p id="demo1"></p>

        <p>But it helps to multiply and divide:</p>

        <p id="demo2"></p>

        <script>
            let x = 0.2 + 0.1;
            let y = (0.2*10 + 0.1*10) / 10;

            document.getElementById("demo1").innerHTML = "0.2 + 0.1 = " + x;
            document.getElementById("demo2").innerHTML = "0.2 + 0.1 = " + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_5.html)

## Adding two numbers results in a new number

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>If you add two numbers, the result will be a number:</p>

        <p id="demo"></p>

        <script>
            let x = 10;
            let y = 20;
            let z = x + y;
            
            document.getElementById("demo").innerHTML = z;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_6.html)

## Adding two numeric strings results in a concatenated string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>If you add two numeric strings, the result will be a concatenated string:</p>

        <p id="demo"></p>

        <script>
            let x = "10";
            let y = "20";
            let z = x + y;
            
            document.getElementById("demo").innerHTML = z;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_7.html)

## Adding a number and a numeric string also results in a concatenated string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>If you add a number and a numeric string, the result will be a concatenated string:</p>

        <p id="demo"></p>

        <script>
            let x = 10;
            let y = "20";
            let z = x + y;
            
            document.getElementById("demo").innerHTML = z;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_8.html)

## Adding a numeric string and a number also results in a concatenated string

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>If you add a numeric string and a number, the result will be a concatenated string:</p>

        <p id="demo"></p>

        <script>
            let x = "10";
            let y = 20;
            
            document.getElementById("demo").innerHTML = "The result is: " + x + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_9.html)

## Common mistake when adding strings and numbers 1

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>A common mistake is to expect this result to be 30:</p>

        <p id="demo"></p>

        <script>
            var x = 10;
            var y = 20;
            
            document.getElementById("demo").innerHTML = "The result is: " + x + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_10.html)

## Common mistake when adding strings and numbers 2

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>A common mistake is to expect this result to be 102030:</p>

        <p id="demo"></p>

        <script>
            let x = 10;
            let y = 20;
            let z = "30";
            let result = x + y + z;
            
            document.getElementById("demo").innerHTML = result;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_11.html)

## JavaScript will try to convert strings to numbers when dividing

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>JavaScript will try to convert strings to numbers when dividing:</p>

        <p id="demo"></p>

        <script>
            let x = "100";
            let y = "10";
            let z = x / y;   
            
            document.getElementById("demo").innerHTML = z;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_12.html)

## JavaScript will try to convert strings to numbers when multiplying

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>JavaScript will try to convert strings to numbers when multiplying:</p>

        <p id="demo"></p>

        <script>
            let x = "100";
            let y = "10";
            let z = x * y;   
            
            document.getElementById("demo").innerHTML = z;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_13.html)

## JavaScript will try to convert strings to numbers when subtracting

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>JavaScript will try to convert strings to numbers when subtracting:</p>

        <p id="demo"></p>

        <script>
            let x = "100";
            let y = "10";
            let z = x - y;   
            
            document.getElementById("demo").innerHTML = z;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_14.html)

## JavaScript will NOT convert strings to numbers when adding

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>JavaScript will NOT convert strings to numbers when adding:</p>

        <p id="demo"></p>

        <script>
            let x = "100";
            let y = "10";
            let z = x + y;   
            
            document.getElementById("demo").innerHTML = z;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_15.html)

## A number divided by a string is NaN (Not a Number)

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

[Click here!](./Numbers/Example_16.html)

## A number divided by a numeric string is a number

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>A number divided by a numeric string becomes a number:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = 100 / "10";
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_17.html)

## The global JavaScript function isNaN() returns if a value is a number

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>You can use the global JavaScript function isNaN() to find out if a value is not a number:</p>

        <p id="demo"></p>

        <script>
            let x = 100 / "Apple";

            document.getElementById("demo").innerHTML = isNaN(x);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_18.html)

## Using NaN in a mathematical operation will always return NaN

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>If you use NaN in a mathematical operation, the result will also be NaN:</p>

        <p id="demo"></p>

        <script>
            let x = NaN;
            let y = 5;
            
            document.getElementById("demo").innerHTML = x + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_19.html)

## Using NaN in a mathematical string operation will concatenate NaN

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>If you use NaN in a mathematical operation, the result can be a concatenation:</p>

        <p id="demo"></p>

        <script>
            let x = NaN;
            let y = "5";
            
            document.getElementById("demo").innerHTML = x + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_20.html)

## NaN (Not a Number) is a number (Yes! typeof NaN returns number)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>The typeof NaN is number:</p>

        <p id="demo"></p>

        <script>
            let x = NaN;
            
            document.getElementById("demo").innerHTML = typeof(x);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_21.html)

## Infinity is returned if you calculate a number outside the largest possible number

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Infinity is returned if you calculate a number outside the largest possible number:</p>

        <p id="demo"></p>

        <script>
            let myNumber = 2; 
            let txt = "";
            
            while (myNumber != Infinity) {
                myNumber = myNumber * myNumber;
                txt = txt + myNumber + "<br>";
            }
            document.getElementById("demo").innerHTML = txt;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_22.html)

## Division by zero also generates Infinity

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Division by zero generates Infinity;</p>

        <p id="demo"></p>

        <script>
            let x = 2/0;
            let y = -2/0;
            
            document.getElementById("demo").innerHTML = x + "<br>" + y;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_23.html)

## Infinity is a number (typeof Infinity returns number)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Infinity is a number:</p>

        <p id="demo"></p>

        <script>
            document.getElementById("demo").innerHTML = typeof(Infinity);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_24.html)

## Constants, preceded by 0x, are interpreted as hexadecimal

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Numeric constants, preceded by 0x, are interpreted as hexadecimal:</p>

        <p id="demo"></p>

        <script>
            let x = 0xFF;
            
            document.getElementById("demo").innerHTML = "0xFF = " + x;
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_25.html)

## The toString() method can output numbers as hex, octal, and binary

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

[Click here!](./Numbers/Example_26.html)

## Numbers can be objects

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p id="demo"></p>

        <script>
            // x is a number
            let x = 123;

            // y is a Number object
            let y = new Number(123);

            document.getElementById("demo").innerHTML = typeof(x) + "<br>" + typeof(y);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_27.html)

## Numbers and objects cannot be safely compared

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>Numbers and Number objects cannot be safely compared:</p>

        <p id="demo"></p>

        <script>
            // x is a number
            let x = 500;

            // y is an object
            let y = new Number(500);

            document.getElementById("demo").innerHTML = (x===y);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_28.html)

## Objects and objects cannot be safely compared

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>JavaScript Numbers</h2>

        <p>JavaScript objects cannot be compared:</p>

        <p id="demo"></p>

        <script>
            // x is an object
            let x = new Number(500);

            // y is an object
            let y = new Number(500);

            document.getElementById("demo").innerHTML = (x==y);
        </script>
    </body>
</html>
```

Output:

[Click here!](./Numbers/Example_29.html)