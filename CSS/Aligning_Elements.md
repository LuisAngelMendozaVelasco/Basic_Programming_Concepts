# Aligning Elements

## Center aligning with margin

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .center {   margin: auto;
                        width: 60%;
                        border: 3px solid #73AD21;
                        padding: 10px;}
        </style>
    </head>
    <body>
        <h2>Center Align Elements</h2>
        <p>To horizontally center a block element (like div), use margin: auto;</p>

        <div class="center">
            <p>Hello World!</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_1.html)

## Center aligning text

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .center {   text-align: center;
                        border: 3px solid green;}
        </style>
    </head>
    <body>
        <h2>Center Text</h2>

        <div class="center">
            <p>This text is centered.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_2.html)

## Center an image

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   display: block;
                    margin-left: auto;
                    margin-right: auto;}
        </style>
    </head>
    <body>
        <h2>Center an Image</h2>
        <p>To center an image, set left and right margin to auto, and make it into a block element.</p>

        <img src="../data/images/paris.jpg" alt="Paris" style="width:40%">
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_3.html)

## Left/Right aligning with position

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .right {position: absolute;
                    right: 0px;
                    width: 300px;
                    border: 3px solid #73AD21;
                    padding: 10px;}
        </style>
    </head>
    <body>
        <h2>Right align with the position property</h2>

        <p>An example of how to right align elements with the position property:</p>

        <div class="right">
            <p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my mind ever since.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_4.html)

## Left/Right aligning with position - Crossbrowser solution

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {  margin: 0;
                    padding: 0;}

            .container {position: relative;
                        width: 100%;}

            .right {position: absolute;
                    right: 0px;
                    width: 300px;
                    background-color: #b0e0e6;}
        </style>
    </head>
    <body>
        <h2>Right Align</h2>

        <div class="container">
            <div class="right">
                <p><b>Note:</b> When aligning using the position property, always include the !DOCTYPE declaration! If missing, it can produce strange results in IE browsers.</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_5.html)

## Left/Right aligning with float

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .right {float: right;
                    width: 300px;
                    border: 3px solid #73AD21;
                    padding: 10px;}
        </style>
    </head>
    <body>
        <h2>Right align with the float property</h2>

        <p>An example of how to right align elements with the float property:</p>

        <div class="right">
            <p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my mind ever since.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_6.html)

## Left/Right aligning with float - Crossbrowser solution

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {  margin: 0;
                    padding: 0;}

            .right {float: right;
                    width: 300px;
                    background-color: #b0e0e6;}
        </style>
    </head>
    <body>
        <h2>Right Align</h2>

        <div class="right">
            <p><b>Note:</b> When aligning using the float property, always include the !DOCTYPE declaration! If missing, it can produce strange results in IE browsers.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_7.html)

## Center vertically with padding

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .center {   padding: 70px 0;
                        border: 3px solid green;}
        </style>
    </head>
    <body>
        <h2>Center vertically with padding</h2>

        <p>In this example, we use the padding property to center the div element vertically:</p>

        <div class="center">
            <p>I am vertically centered.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_8.html)

## Center vertically and horizontally

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .center {   padding: 70px 0;
                        border: 3px solid green;
                        text-align: center;}
        </style>
    </head>
    <body>
        <h2>Center with padding and text-align</h2>

        <p>In this example, we use padding and text-align to center the div element both vertically and horizontally:</p>

        <div class="center">
            <p>I am vertically and horizontally centered.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_9.html)

## Center vertically with line-height

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .center {   line-height: 200px;
                        height: 200px;
                        border: 3px solid green;
                        text-align: center;}

            .center p { line-height: 1.5;
                        display: inline-block;
                        vertical-align: middle;}
        </style>
    </head>
    <body>
        <h2>Center with line-height</h2>

        <p>In this example, we use the line-height property with a value that is equal to the height property to center the div element:</p>

        <div class="center">
            <p>I am vertically and horizontally centered.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_10.html)

## Center vertically and horizontally with position

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .center {   height: 200px;
                        position: relative;
                        border: 3px solid green;}

            .center p { margin: 0;
                        position: absolute;
                        top: 50%;
                        left: 50%;
                        -ms-transform: translate(-50%, -50%);
                        transform: translate(-50%, -50%);}
        </style>
    </head>
    <body>
        <h2>Center with position and transform</h2>

        <p>In this example, we use positioning and the transform property to vertically and horizontally center the div element:</p>

        <div class="center">
            <p>I am vertically and horizontally centered.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Aligning_Elements/Example_11.html)