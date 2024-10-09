# Pseudo-classes

## Add different colors to a hyperlink

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            /* unvisited link */
            a:link {color: red;}

            /* visited link */
            a:visited {color: green;}

            /* mouse over link */
            a:hover {color: hotpink;}

            /* selected link */
            a:active {color: blue;}
        </style>
    </head>
    <body>
        <h2>Styling a link depending on state</h2>

        <p><b><a href="https://www.w3schools.com/css/default.asp" target="_blank">This is a link</a></b></p>
        <p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be effective.</p>
        <p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-classes/Example_1.html)

## Add other styles to hyperlinks

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a.one:link {color:#ff0000;}
            a.one:visited {color:#0000ff;}
            a.one:hover {color:#ffcc00;}

            a.two:link {color:#ff0000;}
            a.two:visited {color:#0000ff;}
            a.two:hover {font-size:150%;}

            a.three:link {color:#ff0000;}
            a.three:visited {color:#0000ff;}
            a.three:hover {background:#66ff66;}

            a.four:link {color:#ff0000;}
            a.four:visited {color:#0000ff;}
            a.four:hover {font-family:monospace;}

            a.five:link {color:#ff0000; text-decoration:none;}
            a.five:visited {color:#0000ff; text-decoration:none;}
            a.five:hover {text-decoration:underline;}
        </style>
    </head>
    <body>
        <h2>Styling Links</h2>

        <p>Mouse over the links and watch them change layout:</p>

        <p><b><a class="one" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes color</a></b></p>
        <p><b><a class="two" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes font-size</a></b></p>
        <p><b><a class="three" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes background-color</a></b></p>
        <p><b><a class="four" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes font-family</a></b></p>
        <p><b><a class="five" href="https://www.w3schools.com/css/default.asp" target="_blank">This link changes text-decoration</a></b></p>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-classes/Example_2.html)

## Use of :focus

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            input:focus {background-color: yellow;}
        </style>
    </head>
    <body>
        <form action="/action_page.php" method="get">
            First name: <input type="text" name="fname"><br><br>
            Last name: <input type="text" name="lname"><br><br>
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-classes/Example_3.html)

## :first-child - match the first p element

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p:first-child {color: blue;} 
        </style>
    </head>
    <body>
        <p>This is some text.</p>
        <p>This is some text.</p>

        <div>
            <p>This is some text.</p>
            <p>This is some text.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-classes/Example_4.html)

## :first-child - match the first i element in all p elements

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p i:first-child {color: blue;} 
        </style>
    </head>
    <body>
        <p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
        <p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-classes/Example_5.html)

## :first-child - Match all i elements in all first child p elements

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p:first-child i {color: blue;} 
        </style>
    </head>
    <body>
        <p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
        <p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>

        <div>
            <p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
            <p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-classes/Example_6.html)

## Use of :lang

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            q:lang(no) {quotes: "~" "~";}
        </style>
    </head>
    <body>
        <p>Some text <q lang="no">A quote in a paragraph</q> Some text.</p>
        <p>In this example, :lang defines the quotation marks for q elements with lang="no":</p>
    </body>
</html>
```

Output:

[Click here!](./Pseudo-classes/Example_7.html)