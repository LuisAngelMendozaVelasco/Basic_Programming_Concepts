# Forms

## Full-width input field

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input {width: 100%;}
        </style>
    </head>
    <body>
        <h2>A full-width input field</h2>

        <form>
            <label for="fname">First Name</label>
            <input type="text" id="fname" name="fname">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_1.html)

## Padded input field

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input[type=text] {  width: 100%;
                                padding: 12px 20px;
                                margin: 8px 0;
                                box-sizing: border-box;}
        </style>
    </head>
    <body>
        <h2>Padded input fields</h2>

        <form>
            <label for="fname">First Name</label>
            <input type="text" id="fname" name="fname">
            <label for="lname">Last Name</label>
            <input type="text" id="lname" name="lname">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_2.html)

## Bordered input field

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input[type=text] {  width: 100%;
                                padding: 12px 20px;
                                margin: 8px 0;
                                box-sizing: border-box;
                                border: 2px solid red;
                                border-radius: 4px;}
        </style>
    </head>
    <body>
        <h2>Input fields with borders</h2>

        <form>
            <label for="fname">First Name</label>
            <input type="text" id="fname" name="fname">
            <label for="lname">Last Name</label>
            <input type="text" id="lname" name="lname">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_3.html)

## Bottom bordered input field

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input[type=text] {  width: 100%;
                                padding: 12px 20px;
                                margin: 8px 0;
                                box-sizing: border-box;
                                border: none;
                                border-bottom: 2px solid red;}
        </style>
    </head>
    <body>
        <h2>Input fields with bottom border</h2>

        <form>
            <label for="fname">First Name</label>
            <input type="text" id="fname" name="fname">
            <label for="lname">Last Name</label>
            <input type="text" id="lname" name="lname">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_4.html)

## Colored input fields

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input[type=text] {  width: 100%;
                                padding: 12px 20px;
                                margin: 8px 0;
                                box-sizing: border-box;
                                border: none;
                                background-color: #3CBC8D;
                                color: white;}
        </style>
    </head>
    <body>
        <h2>Input fields with color</h2>

        <form>
            <label for="fname">First Name</label>
            <input type="text" id="fname" name="fname" value="John">
            <label for="lname">Last Name</label>
            <input type="text" id="lname" name="lname" value="Doe">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_5.html)

## Focused input fields

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input[type=text] {  width: 100%;
                                padding: 12px 20px;
                                margin: 8px 0;
                                box-sizing: border-box;
                                border: 1px solid #555;
                                outline: none;}

            input[type=text]:focus {background-color: lightblue;}
        </style>
    </head>
    <body>
        <h2>Input fields with color on :focus</h2>

        <p>Here, the input field gets a color when it gets focus (clicked on):</p>

        <form>
            <label for="fname">First Name</label>
            <input type="text" id="fname" name="fname" value="John">
            <label for="lname">Last Name</label>
            <input type="text" id="lname" name="lname" value="Doe">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_6.html)

## Focused input fields 2

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input[type=text] {  width: 100%;
                                padding: 12px 20px;
                                margin: 8px 0;
                                box-sizing: border-box;
                                border: 3px solid #ccc;
                                -webkit-transition: 0.5s;
                                transition: 0.5s;
                                outline: none;}

            input[type=text]:focus {border: 3px solid #555;}
        </style>
    </head>
    <body>
        <h2>Input fields with black border on :focus</h2>

        <p>Here, the input field gets a black border color when it gets focus (clicked on). We have also added the CSS transition property to animate the border color (takes 0.5 seconds to change the color on focus):</p>

        <form>
            <label for="fname">First Name</label>
            <input type="text" id="fname" name="fname" value="John">
            <label for="lname">Last Name</label>
            <input type="text" id="lname" name="lname" value="Doe">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_7.html)

## Input with icon/image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input[type=text] {  width: 100%;
                                box-sizing: border-box;
                                border: 2px solid #ccc;
                                border-radius: 4px;
                                font-size: 16px;
                                background-color: white;
                                background-image: url('../data/images/searchicon.png');
                                background-position: 10px 10px; 
                                background-repeat: no-repeat;
                                padding: 12px 20px 12px 40px;}
        </style>
    </head>
    <body>
        <h2>Input field with an icon inside</h2>

        <form>
            <input type="text" name="search" placeholder="Search..">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_8.html)

## Animated search input

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input[type=text] {  width: 130px;
                                box-sizing: border-box;
                                border: 2px solid #ccc;
                                border-radius: 4px;
                                font-size: 16px;
                                background-color: white;
                                background-image: url('../data/images/searchicon.png');
                                background-position: 10px 10px; 
                                background-repeat: no-repeat;
                                padding: 12px 20px 12px 40px;
                                transition: width 0.4s ease-in-out;}

            input[type=text]:focus {width: 100%;}
        </style>
    </head>
    <body>
        <h2>Animate width of search input</h2>

        <form>
            <input type="text" name="search" placeholder="Search..">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_9.html)

## Styling textareas

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            textarea {  width: 100%;
                        height: 150px;
                        padding: 12px 20px;
                        box-sizing: border-box;
                        border: 2px solid #ccc;
                        border-radius: 4px;
                        background-color: #f8f8f8;
                        font-size: 16px;
                        resize: none;}
        </style>
    </head>
    <body>
        <h2>Styling textarea</h2>

        <p><strong>Tip:</strong> Use the resize property to prevent textareas from being resized (disable the "grabber" in the bottom right corner):</p>

        <form>
            <textarea>Some text...</textarea>
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_10.html)

## Styling select menus

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            select {width: 100%;
                    padding: 16px 20px;
                    border: none;
                    border-radius: 4px;
                    background-color: #f1f1f1;}
        </style>
    </head>
    <body>
        <h2>Styling a select menu</h2>

        <form>
            <select id="country" name="country">
                <option value="au">Australia</option>
                <option value="ca">Canada</option>
                <option value="usa">USA</option>
            </select>
        </form>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_11.html)

## Styling input buttons

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            input[type=button], input[type=submit], input[type=reset] { background-color: #04AA6D;
                                                                        border: none;
                                                                        color: white;
                                                                        padding: 16px 32px;
                                                                        text-decoration: none;
                                                                        margin: 4px 2px;
                                                                        cursor: pointer;}
        </style>
    </head>
    <body>
        <h2>Styling form buttons</h2>

        <input type="button" value="Button">
        <input type="reset" value="Reset">
        <input type="submit" value="Submit">
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_12.html)

## Responsive form

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            * {box-sizing: border-box;}

            input[type=text], select, textarea {width: 100%;
                                                padding: 12px;
                                                border: 1px solid #ccc;
                                                border-radius: 4px;
                                                resize: vertical;}

            label { padding: 12px 12px 12px 0;
                    display: inline-block;}

            input[type=submit] {background-color: #04AA6D;
                                color: white;
                                padding: 12px 20px;
                                border: none;
                                border-radius: 4px;
                                cursor: pointer;
                                float: right;}

            input[type=submit]:hover {background-color: #45a049;}

            .container {border-radius: 5px;
                        background-color: #f2f2f2;
                        padding: 20px;}

            .col-25 {   float: left;
                        width: 25%;
                        margin-top: 6px;}

            .col-75 {   float: left;
                        width: 75%;
                        margin-top: 6px;}

            /* Clear floats after the columns */
            .row::after {   content: "";
                            display: table;
                            clear: both;}

            /* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */
            @media screen and (max-width: 600px) {.col-25, .col-75, input[type=submit] {width: 100%;
                                                                                        margin-top: 0;}}
        </style>
    </head>
    <body>
        <h2>Responsive Form</h2>
        <p>Resize the browser window to see the effect. When the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other.</p>

        <div class="container">
            <form action="/action_page.php">
                <div class="row">
                    <div class="col-25">
                        <label for="fname">First Name</label>
                    </div>
                    <div class="col-75">
                        <input type="text" id="fname" name="firstname" placeholder="Your name..">
                    </div>
                </div>
                <div class="row">
                    <div class="col-25">
                        <label for="lname">Last Name</label>
                    </div>
                    <div class="col-75">
                        <input type="text" id="lname" name="lastname" placeholder="Your last name..">
                    </div>
                </div>
                <div class="row">
                    <div class="col-25">
                        <label for="country">Country</label>
                    </div>
                    <div class="col-75">
                        <select id="country" name="country">
                            <option value="australia">Australia</option>
                            <option value="canada">Canada</option>
                            <option value="usa">USA</option>
                        </select>
                    </div>
                </div>
                <div class="row">
                    <div class="col-25">
                        <label for="subject">Subject</label>
                    </div>
                    <div class="col-75">
                        <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>
                    </div>
                </div>
                <br>
                <div class="row">
                    <input type="submit" value="Submit">
                </div>
            </form>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Forms/Example_13.html)