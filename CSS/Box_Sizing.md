# Box Sizing

## Width of elements without box-sizing

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .div1 { width: 300px;
                    height: 100px;
                    border: 1px solid blue;}

            .div2 { width: 300px;
                    height: 100px;  
                    padding: 50px;
                    border: 1px solid red;}
        </style>
    </head>
    <body>
        <h1>Without box-sizing</h1>

        <div class="div1">This div is smaller (width is 300px and height is 100px).</div>
        <br>
        <div class="div2">This div is bigger (width is also 300px and height is 100px).</div>
    </body>
</html>
```

Output:

[Click here!](./Box_Sizing/Example_1.html)

## Width of elements with box-sizing

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .div1 { width: 300px;
                    height: 100px;
                    border: 1px solid blue;
                    box-sizing: border-box;}

            .div2 { width: 300px;
                    height: 100px;  
                    padding: 50px;
                    border: 1px solid red;
                    box-sizing: border-box;}
        </style>
    </head>
    <body>
        <h1>With box-sizing</h1>

        <div class="div1">Both divs are the same size now!</div>
        <br>
        <div class="div2">Hooray!</div>
    </body>
</html>
```

Output:

[Click here!](./Box_Sizing/Example_2.html)

## Form elements + box-sizing

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {margin: 0;}
            * {box-sizing: border-box;} 
            input, textarea {width: 100%;}
        </style>
    </head>
    <body>
        <form action="/action_page.php">
            First name:<br>
            <input type="text" name="firstname" value="Mickey"><br>
            Last name:<br>
            <input type="text" name="lastname" value="Mouse"><br>
            Comments:<br>
            <textarea name="message" rows="5" cols="30"></textarea>
            <br><br>
            <input type="submit" value="Submit">
        </form> 

        <p>
            <strong>Tip:</strong> Try to remove the box-sizing property from the style element and look what happens.
            Notice that the width of input, textarea, and submit button will go outside of the screen.
        </p>
    </body>
</html>
```

Output:

[Click here!](./Box_Sizing/Example_3.html)