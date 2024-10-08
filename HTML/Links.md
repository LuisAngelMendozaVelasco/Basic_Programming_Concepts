# Links

## - Linking, using an absolute UR -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>HTML Links</h1>
        <p><a href="https://www.w3schools.com/">Visit W3Schools.com!</a></p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h1>HTML Links</h1>
        <p><a href="https://www.w3schools.com/">Visit W3Schools.com!</a></p>
    </body>
</html>

## - Linking, using a relative URL -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Absolute URLs</h2>
        <p><a href="https://www.w3.org/">W3C</a></p>
        <p><a href="https://www.google.com/">Google</a></p>
        <h2>Relative URLs</h2>
        <!-- <p><a href="html_images.asp">HTML Images</a></p> -->
        <p><a href="https://www.w3schools.com/html/html_images.asp">HTML Images</a></p>
        <!-- <p><a href="/css/default.asp">CSS Tutorial</a></p> -->
        <p><a href="https://www.w3schools.com/css/default.asp">CSS Tutorial</a></p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Absolute URLs</h2>
        <p><a href="https://www.w3.org/">W3C</a></p>
        <p><a href="https://www.google.com/">Google</a></p>
        <h2>Relative URLs</h2>
        <!-- <p><a href="html_images.asp">HTML Images</a></p> -->
        <p><a href="https://www.w3schools.com/html/html_images.asp">HTML Images</a></p>
        <!-- <p><a href="/css/default.asp">CSS Tutorial</a></p> -->
        <p><a href="https://www.w3schools.com/css/default.asp">CSS Tutorial</a></p>
    </body>
</html>

## - Changing the color of links -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a:link {color: green;
                    background-color: transparent;
                    text-decoration: none;}
            a:visited { color: pink;
                        background-color: transparent;
                        text-decoration: none;}
            a:hover {   color: red;
                        background-color: transparent;
                        text-decoration: underline;}
            a:active {  color: yellow;
                        background-color: transparent;
                        text-decoration: underline;}
        </style>
    </head>
    <body>
        <h2>Link Colors</h2>
        <p>You can change the default colors of links</p>
        <a href="https://www.w3schools.com/html/html_images.asp" target="_blank">HTML Images</a> 
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block1 {
                a:link {color: green;
                        background-color: transparent;
                        text-decoration: none;}
                a:visited { color: pink;
                            background-color: transparent;
                            text-decoration: none;}
                a:hover {   color: red;
                            background-color: transparent;
                            text-decoration: underline;}
                a:active {  color: yellow;
                            background-color: transparent;
                            text-decoration: underline;}
            }
        </style>
    </head>
    <body>
        <div id="block1">
            <h2>Link Colors</h2>
            <p>You can change the default colors of links</p>
            <a href="https://www.w3schools.com/html/html_images.asp" target="_blank">HTML Images</a> 
        </div>
    </body>
</html>

## - Removing the underline from links -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <a href="https://www.w3schools.com/html/html_images.asp" style="text-decoration:none">HTML Images</a>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <a href="https://www.w3schools.com/html/html_images.asp" style="text-decoration:none">HTML Images</a>
    </body>
</html>

## - Changing the target of a link -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The target Attribute</h2>
        <a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a> 
        <p>If target="_blank", the link will open in a new browser window or tab.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>The target Attribute</h2>
        <a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a> 
        <p>If target="_blank", the link will open in a new browser window or tab.</p>
    </body>
</html>

## - An image as a link -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Image as a Link</h2>
        <p>The image below is a link. Try to click on it.</p>
        <a href="https://www.w3schools.com/html/default.asp"><img src="./images/smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;"></a>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Image as a Link</h2>
        <p>The image below is a link. Try to click on it.</p>
        <a href="https://www.w3schools.com/html/default.asp"><img src="./images/smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;"></a>
    </body>
</html>

## - Creating a bookmark link -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p><a href="#C4">Jump to Chapter 4</a></p>
        <p><a href="#C10">Jump to Chapter 10</a></p>

        <h2>Chapter 1</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 2</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 3</h2>
        <p>This chapter explains ba bla bla</p>

        <h2 id="C4">Chapter 4</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 5</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 6</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 7</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 8</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 9</h2>
        <p>This chapter explains ba bla bla</p>

        <h2 id="C10">Chapter 10</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 11</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 12</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 13</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 14</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 15</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 16</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 17</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 18</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 19</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 20</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 21</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 22</h2>
        <p>This chapter explains ba bla bla</p>

        <h2>Chapter 23</h2>
        <p>This chapter explains ba bla bla</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<p><a href="#C4">Jump to Chapter 4</a></p>
<p><a href="#C10">Jump to Chapter 10</a></p>

<h2>Chapter 1</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 2</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 3</h2>
<p>This chapter explains ba bla bla</p>

<h2 id="C4">Chapter 4</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 5</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 6</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 7</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 8</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 9</h2>
<p>This chapter explains ba bla bla</p>

<h2 id="C10">Chapter 10</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 11</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 12</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 13</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 14</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 15</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 16</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 17</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 18</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 19</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 20</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 21</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 22</h2>
<p>This chapter explains ba bla bla</p>

<h2>Chapter 23</h2>
<p>This chapter explains ba bla bla</p>
    </body>
</html>

## - A link that breaks out of a frame -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Locked in a frame? <a href="https://www.w3schools.com/html/" target="_top">Click here!</a></p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <p>Locked in a frame? <a href="https://www.w3schools.com/html/" target="_top">Click here!</a></p>
    </body>
</html>

## - A mailto link -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p>
            This is an email link:
            <a href="mailto:someone@example.com?Subject=Hello%20again" target="_top">Send Mail</a>
        </p>
        <p>The link will only work if you have email installed.</p>
        <p>(Spaces between words should be replaced by %20 to ensure that the browser will display the text properly)</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <p>
            This is an email link:
            <a href="mailto:someone@example.com?Subject=Hello%20again" target="_top">Send Mail</a>
        </p>
        <p>The link will only work if you have email installed.</p>
        <p>(Spaces between words should be replaced by %20 to ensure that the browser will display the text properly)</p>
    </body>
</html>

## - A mailto link with subject -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p>
            This is another mailto link:
            <a href="mailto:someone@example.com?cc=someoneelse@example.com&bcc=andsomeoneelse@example.com&subject=Summer%20Party&body=You%20are%20invited%20to%20a%20big%20summer%20party!" target="_top">Send mail!</a>
        </p>
        <p>The link will only work if you have email installed.</p>
        <p>(Spaces between words should be replaced by %20 to ensure that the browser will display the text properly)</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <p>
            This is another mailto link:
            <a href="mailto:someone@example.com?cc=someoneelse@example.com&bcc=andsomeoneelse@example.com&subject=Summer%20Party&body=You%20are%20invited%20to%20a%20big%20summer%20party!" target="_top">Send mail!</a>
        </p>
        <p>The link will only work if you have email installed.</p>
        <p>(Spaces between words should be replaced by %20 to ensure that the browser will display the text properly)</p>
    </body>
</html>