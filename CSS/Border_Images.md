# Border Images

## Create an image border around an element, using the round keyword

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            #borderimg {border: 10px solid transparent;
                        padding: 15px;
                        border-image: url(../data/images/border.png) 30 round;}
        </style>
    </head>
    <body>
        <h1>The border-image Property</h1>

        <p>Here, the middle sections of the image are repeated to create the border:</p>
        <p id="borderimg">border-image: url(border.png) 30 round;</p>

        <p>Here is the original image:</p><img src="../data/images/border.png">
        <p><strong>Note:</strong> Internet Explorer 10, and earlier versions, do not support the border-image property.</p>
    </body>
</html>
```

Output:

[Click here!](./Border_Images/Example_1.html)

## Create an image border around an element, using the stretch keyword

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            #borderimg {border: 10px solid transparent;
                        padding: 15px;
                        border-image: url(../data/images/border.png) 30 stretch;}
        </style>
    </head>
    <body>
        <h1>The border-image Property</h1>

        <p>Here, the middle sections of the image are stretched to create the border:</p>
        <p id="borderimg">border-image: url(border.png) 30 stretch;</p>

        <p>Here is the original image:</p><img src="../data/images/border.png">
        <p><strong>Note:</strong> Internet Explorer 10, and earlier versions, do not support the border-image property.</p>
    </body>
</html>
```

Output:

[Click here!](./Border_Images/Example_2.html)

## Image border - Different slice values

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #borderimg1 {   border: 10px solid transparent;
                            padding: 15px;
                            border-image: url(../data/images/border.png) 50 round;}

            #borderimg2 {   border: 10px solid transparent;
                            padding: 15px;
                            border-image: url(../data/images/border.png) 20% round;}

            #borderimg3 {   border: 10px solid transparent;
                            padding: 15px;
                            border-image: url(../data/images/border.png) 30% round;}
        </style>
    </head>
    <body>
        <h1>The border-image Property</h1>

        <p id="borderimg1">border-image: url(border.png) 50 round;</p>
        <p id="borderimg2">border-image: url(border.png) 20% round;</p>
        <p id="borderimg3">border-image: url(border.png) 30% round;</p>

        <p><strong>Note:</strong> Internet Explorer 10, and earlier versions, do not support the border-image property.</p>
    </body>
</html>
```

Output:

[Click here!](./Border_Images/Example_3.html)