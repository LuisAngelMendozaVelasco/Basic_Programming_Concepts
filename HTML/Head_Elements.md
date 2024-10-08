# Head Elements

## - A valid HTML document with no `<html>` `<body>`, and `<head>` -

Code:

```html
<!DOCTYPE html>
<title>Page Title</title>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>
```

Output:

<!DOCTYPE html>
<title>Page Title</title>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

## - A valid HTML document with no `<head>` element -

Code:

```html
<!DOCTYPE html>
<html>
    <title>Page Title</title>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <title>Page Title</title>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html>

## - The `<title>` element defines the document title -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>A Meaningful Page Title</title>
    </head>
    <body>
        <p>The content of the body element is displayed in the browser window.</p>
        <p>The content of the title element is displayed in the browser tab, in favorites and in search-engine results.</p>
    </body>
</html>    
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <title>A Meaningful Page Title</title>
    </head>
    <body>
        <p>The content of the body element is displayed in the browser window.</p>
        <p>The content of the title element is displayed in the browser tab, in favorites and in search-engine results.</p>
    </body>
</html>    

## - The `<style>` element contains style information -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <style>
            body {background-color: powderblue;}
            h1 {color: red;}
            p {color: blue;}
        </style>
    </head>  
    <body>
        <h1>This is a Heading</h1>
        <p>This is a paragraph.</p>
            
        <p>The content of the body element is displayed in the browser window.</p>
        <p>The content of the title element is displayed in the browser tab, in favorites and in search-engine results.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <style>
            #block1 {
            body {background-color: powderblue;}
            h1 {color: red;}
            p {color: blue;}
            }
        </style>
    </head>  
    <body>
<div id="block1">
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
    
<p>The content of the body element is displayed in the browser window.</p>
<p>The content of the title element is displayed in the browser tab, in favorites and in search-engine results.</p>
</div>
    </body>
</html>

## - The `<link>` element defines a relationship to an external resource -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <link rel="stylesheet" href="./mystyle.css">
    </head>
    <body>
        <h1>This is a Heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <link rel="stylesheet" href="./mystyle.css">
    </head>
    <body>
        <h1>This is a Heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html>

## - The `<meta>` element defines special meta information -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="description" content="Free Web tutorials">
        <meta name="keywords" content="HTML, CSS, JavaScript">
        <meta name="author" content="John Doe">
    </head>
    <body>
        <p>All meta information goes inside the head section.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="description" content="Free Web tutorials">
        <meta name="keywords" content="HTML, CSS, JavaScript">
        <meta name="author" content="John Doe">
    </head>
    <body>
        <p>All meta information goes inside the head section.</p>
    </body>
</html>

## - The `<script>` element defines client-side JavaScripts -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <script>
            function myFunction() {
                document.getElementById("demo").innerHTML = "Hello JavaScript!";
            }
        </script>
    </head>
    <body>
        <h1>My Web Page</h1>
        <p id="demo">A Paragraph</p>
        <button type="button" onclick="myFunction()">Try it!</button>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <script>
            function myFunction() {
                document.getElementById("demo").innerHTML = "Hello JavaScript!";
            }
        </script>
    </head>
    <body>
        <h1>My Web Page</h1>
        <p id="demo">A Paragraph</p>
        <button type="button" onclick="myFunction()">Try it!</button>
    </body>
</html>

## - The `<base>` element defines the base URL for all URLs -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <base href="https://www.w3schools.com/" target="_blank">
    </head>
    <body>
        <h1>The base element</h1>

        <p><img src="images/stickman.gif" width="24" height="39" alt="Stickman"> - Notice that we have only specified a relative address for the image. Since we have specified a base URL in the head section, the browser will look for the image at "https://www.w3schools.com/images/stickman.gif".</p>

        <p><a href="tags/tag_base.asp">HTML base tag</a> - Notice that the link opens in a new window, even if it has no target="_blank" attribute. This is because the target attribute of the base element is set to "_blank".</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <base href="https://www.w3schools.com/" target="_blank">
    </head>
    <body>
<h1>The base element</h1>

<p><img src="images/stickman.gif" width="24" height="39" alt="Stickman"> - Notice that we have only specified a relative address for the image. Since we have specified a base URL in the head section, the browser will look for the image at "https://www.w3schools.com/images/stickman.gif".</p>

<p><a href="tags/tag_base.asp">HTML base tag</a> - Notice that the link opens in a new window, even if it has no target="_blank" attribute. This is because the target attribute of the base element is set to "_blank".</p>
    </body>
</html>