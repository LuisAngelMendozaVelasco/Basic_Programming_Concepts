# Image Reflection

## Create reflection below the image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {-webkit-box-reflect: below;}
        </style>
    </head>
    <body>
        <h1>CSS Image Reflection</h1>

        <p>Show the reflection below the image:</p>
        <img src="../data/images/img_tree.png">
    </body>
</html>
```

Output:

[Click here!](./Image_Reflection/Example_1.html)

## Create reflection to the right of the image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {-webkit-box-reflect: right;}
        </style>
    </head>
    <body>
        <h1>CSS Image Reflection</h1>

        <p>Show the reflection to the right of the image:</p>
        <img src="../data/images/img_tree.png">
    </body>
</html>
```

Output:

[Click here!](./Image_Reflection/Example_2.html)

## Create a gap between the image and the reflection

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {-webkit-box-reflect: below 20px;}
        </style>
    </head>
    <body>
        <h1>CSS Image Reflection</h1>

        <p>Show the reflection below the image, with a 20 pixels offset:</p>
        <img src="../data/images/img_tree.png">
    </body>
</html>
```

Output:

[Click here!](./Image_Reflection/Example_3.html)

## Create a fade-out effect on the reflection

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {-webkit-box-reflect: below 0px linear-gradient(to bottom, rgba(0,0,0,1), rgba(0,0,0,0));}
        </style>
    </head>
    <body>
        <h1>CSS Image Reflection</h1>

        <p>Show the reflection with gradient (to make a fade-out effect):</p>
        <img src="../data/images/img_tree.png">
    </body>
</html>
```

Output:

[Click here!](./Image_Reflection/Example_4.html)