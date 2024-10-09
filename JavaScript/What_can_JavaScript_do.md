# What can JavaScript do

## JavaScript can change HTML content

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>What Can JavaScript Do?</h2>

        <p id="demo">JavaScript can change HTML content.</p>

        <button type="button" onclick='document.getElementById("demo").innerHTML = "Hello JavaScript!"'>Click Me!</button>
    </body>
</html>
```

Output:

[Click here!](./What_can_JavaScript_do/Example_1.html)

## JavaScript can change HTML attributes

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>What Can JavaScript Do?</h2>

        <p>JavaScript can change HTML attribute values.</p>

        <p>In this case JavaScript changes the value of the src (source) attribute of an image.</p>

        <button onclick="document.getElementById('myImage').src='../data/images/pic_bulbon.gif'">Turn on the light</button>

        <img id="myImage" src="../data/images/pic_bulboff.gif" style="width:100px">

        <button onclick="document.getElementById('myImage').src='../data/images/pic_bulboff.gif'">Turn off the light</button>
    </body>
</html>
```

Output:

[Click here!](./What_can_JavaScript_do/Example_2.html)

## JavaScript can change CSS style

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>What Can JavaScript Do?</h2>

        <p id="demo">JavaScript can change the style of an HTML element.</p>

        <button type="button" onclick="document.getElementById('demo').style.fontSize = '35px'">Click Me!</button>
    </body>
</html> 
```

Output:

[Click here!](./What_can_JavaScript_do/Example_3.html)

## JavaScript can hide HTML elements

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>What Can JavaScript Do?</h2>

        <p id="demo">JavaScript can hide HTML elements.</p>

        <button type="button" onclick="document.getElementById('demo').style.display = 'none'">Click Me!</button>
    </body>
</html> 
```

Output:

[Click here!](./What_can_JavaScript_do/Example_4.html)

## JavaScript can show hidden HTML elements

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>What Can JavaScript Do?</h2>

        <p>JavaScript can show hidden HTML elements.</p>

        <p id="demo" style="display:none">Hello JavaScript!</p>

        <button type="button" onclick="document.getElementById('demo').style.display = 'block'">Click Me!</button>
    </body>
</html> 
```

Output:

[Click here!](./What_can_JavaScript_do/Example_5.html)