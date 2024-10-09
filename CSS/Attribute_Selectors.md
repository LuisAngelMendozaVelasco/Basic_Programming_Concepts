# Attribute Selectors

## Selects all `<a>` elements with a target attribute

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a[target] {background-color: yellow;}
        </style>
    </head>
    <body>
        <h2>CSS [attribute] Selector</h2>
        <p>The links with a target attribute gets a yellow background:</p>

        <a href="https://www.w3schools.com">w3schools.com</a>
        <a href="http://www.disney.com" target="_blank">disney.com</a>
        <a href="http://www.wikipedia.org" target="_top">wikipedia.org</a>
    </body>
</html>
```

Output:

[Click here!](./Attribute_Selectors/Example_1.html)

## Selects all `<a>` elements with a target="_blank" attribute

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            a[target="_blank"] {background-color: yellow;}
        </style>
    </head>
    <body>
        <h2>CSS [attribute="value"] Selector</h2>
        <p>The link with target="_blank" gets a yellow background:</p>

        <a href="https://www.w3schools.com">w3schools.com</a>
        <a href="http://www.disney.com" target="_blank">disney.com</a>
        <a href="http://www.wikipedia.org" target="_top">wikipedia.org</a>
    </body>
</html>
```

Output:

[Click here!](./Attribute_Selectors/Example_2.html)

## Selects all elements with a title attribute that contains a space-separated list of words, one of which is "flower"

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            [title~="flower"] {border: 5px solid yellow;}
        </style>
    </head>
    <body>
        <h2>CSS [attribute~="value"] Selector</h2>
        <p>All images with the title attribute containing the word "flower" get a yellow border.</p>

        <img src="../data/images/klematis.jpg" title="klematis flower" width="150" height="113">
        <img src="../data/images/img_flwr.gif" title="flower" width="224" height="162">
        <img src="../data/images/img_tree.gif" title="tree" width="200" height="358">
    </body>
</html>
```

Output:

[Click here!](./Attribute_Selectors/Example_3.html)

## Selects all elements with a class attribute value that begins with "top" (must be whole word)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            [class|="top"] {background: yellow;}
        </style>
    </head>
    <body>
        <h2>CSS [attribute|="value"] Selector</h2>

        <h1 class="top-header">Welcome</h1>
        <p class="top-text">Hello world!</p>
        <p class="topcontent">Are you learning CSS?</p>
    </body>
</html>
```

Output:

[Click here!](./Attribute_Selectors/Example_4.html)

## Selects all elements with a class attribute value that begins with "top" (must not be whole word)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            [class^="top"] {background: yellow;}
        </style>
    </head>
    <body>
        <h2>CSS [attribute^="value"] Selector</h2>

        <h1 class="top-header">Welcome</h1>
        <p class="top-text">Hello world!</p>
        <p class="topcontent">Are you learning CSS?</p>
    </body>
</html>
```

Output:

[Click here!](./Attribute_Selectors/Example_5.html)

## Selects all elements with a class attribute value that ends with "test"

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            [class$="test"] {background: yellow;}
        </style>
    </head>
    <body>
        <h2>CSS [attribute$="value"] Selector</h2>

        <div class="first_test">The first div element.</div>
        <div class="second">The second div element.</div>
        <div class="my-test">The third div element.</div>
        <p class="mytest">This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Attribute_Selectors/Example_6.html)

## Selects all elements with a class attribute value that contains "te"

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            [class*="te"] {background: yellow;}
        </style>
    </head>
    <body>
        <h2>CSS [attribute*="value"] Selector</h2>

        <div class="first_test">The first div element.</div>
        <div class="second">The second div element.</div>
        <div class="my-test">The third div element.</div>
        <p class="mytest">This is some text in a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Attribute_Selectors/Example_7.html)

