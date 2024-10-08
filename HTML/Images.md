# Images

## - An image -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Italian Trulli</h2>
        <img src="./images/pic_trulli.jpg" alt="Italian Trullti" style="width:100%">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Italian Trulli</h2>
        <img src="./images/pic_trulli.jpg" alt="Italian Trullti" style="width:100%">
    </body>
</html>

## - An image height and width using attributes -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Image Size</h2>
        <p>Here we specify the width and height of an image with the width and height attributes:</p>
        <img src="./images/img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Image Size</h2>
        <p>Here we specify the width and height of an image with the width and height attributes:</p>
        <img src="./images/img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
    </body>
</html>

## - An image height and width using CSS -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Image Size</h2>
        <p>Here we use the style attribute to specify the width and height of an image:</p>
        <img src="./images/img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Image Size</h2>
        <p>Here we use the style attribute to specify the width and height of an image:</p>
        <img src="./images/img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">
    </body>
</html>

## - An image height and width using both -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            /* This style sets the width of all images to 100%: */
            img {width: 100%;}
        </style>
    </head>
    <body>
        <h2>Width/Height Attributes or Style?</h2>
        <p>The first image uses the width attribute (set to 128 pixels), but the style in the head section overrides it, and sets the width to 100%.</p>
        <img src="./images/html5.gif" alt="HTML5 Icon" width="128" height="128">
        <p>The second image uses the style attribute to set the width to 128 pixels, this will not be overridden by the style in the head section:</p>
        <img src="./images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            /* This style sets the width of all images to 100%: */
            #block1 {
                img {width: 100%;}
            }
        </style>
    </head>
    <body>
        <div id="block1">
            <h2>Width/Height Attributes or Style?</h2>
            <p>The first image uses the width attribute (set to 128 pixels), but the style in the head section overrides it, and sets the width to 100%.</p>
            <img src="./images/html5.gif" alt="HTML5 Icon" width="128" height="128">
            <p>The second image uses the style attribute to set the width to 128 pixels, this will not be overridden by the style in the head section:</p>
            <img src="./images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
        </div>
    </body>
</html>

## - An image in another folder -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Images in Another Folder</h2>
        <p>It is common to store images in a sub-folder. You must then include the folder name in the src attribute:</p>
        <img src="./images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Images in Another Folder</h2>
        <p>It is common to store images in a sub-folder. You must then include the folder name in the src attribute:</p>
        <img src="./images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
    </body>
</html>

## - An image with a broken link -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p>If a browser cannot find an image, it will display the alternate text:</p>
        <img src="wrongname.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <p>If a browser cannot find an image, it will display the alternate text:</p>
        <img src="wrongname.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
    </body>
</html>

## - An image on another server -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Images on Another Server</h2>
        <img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com" style="width:104px;height:142px;">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Images on Another Server</h2>
        <img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com" style="width:104px;height:142px;">
    </body>
</html>

## - Using an image as a link -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Image as a Link</h2>
        <p>The image is a link. You can click on it.</p>
        <a href="https://www.w3schools.com/html/default.asp">
            <img src="./images/smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
        </a>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Image as a Link</h2>
        <p>The image is a link. You can click on it.</p>
        <a href="https://www.w3schools.com/html/default.asp">
            <img src="./images/smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
        </a>
    </body>
</html>

## - A moving image -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Animated Images</h2>
        <p>HTML allows moving images:</p>
        <img src="./images/programming.gif" alt="Computer man" style="width:48px;height:48px;">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Animated Images</h2>
        <p>HTML allows moving images:</p>
        <img src="./images/programming.gif" alt="Computer man" style="width:48px;height:48px;">
    </body>
</html>

## - An image map with clickable regions -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Image Maps</h2>
        <p>Click on the sun or on one of the planets to watch it closer:</p>
        <img src="./images/planets.gif" alt="Planets" usemap="#planetmap" style="width:145px;height:126px;">
        <map name="planetmap">
            <area shape="rect" coords="0,0,82,126" alt="Sun" href="./images/sun.gif">
            <area shape="circle" coords="90,58,3" alt="Mercury" href="./images/merglobe.gif">
            <area shape="circle" coords="124,58,8" alt="Venus" href="./images/venglobe.gif">
        </map>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Image Maps</h2>
        <p>Click on the sun or on one of the planets to watch it closer:</p>
        <img src="./images/planets.gif" alt="Planets" usemap="#planetmap" style="width:145px;height:126px;">
        <map name="planetmap">
            <area shape="rect" coords="0,0,82,126" alt="Sun" href="./images/sun.gif">
            <area shape="circle" coords="90,58,3" alt="Mercury" href="./images/merglobe.gif">
            <area shape="circle" coords="124,58,8" alt="Venus" href="./images/venglobe.gif">
        </map>
    </body>
</html>

## - A floating image -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Floating Images</h2>
        <p><strong>Float the image to the right:</strong></p>
        <p>
            <img src="./images/smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
            A paragraph with a floating image. A paragraph with a floating image. A paragraph with a floating image.
        </p>
        <p><strong>Float the image to the left:</strong></p>
        <p>
            <img src="./images/smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
            A paragraph with a floating image. A paragraph with a floating image. A paragraph with a floating image.  
        </p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Floating Images</h2>
        <p><strong>Float the image to the right:</strong></p>
        <p>
            <img src="./images/smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
            A paragraph with a floating image. A paragraph with a floating image. A paragraph with a floating image.
        </p>
        <p><strong>Float the image to the left:</strong></p>
        <p>
            <img src="./images/smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
            A paragraph with a floating image. A paragraph with a floating image. A paragraph with a floating image.  
        </p>
    </body>
</html>