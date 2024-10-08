# Classes

## Style all elements with a specified class name

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .cities {   background-color: black;
                        color: white;
                        padding: 20px;}
        </style>
    </head>
    <body>
        <h2>The class Attribute</h2>
        <p>Use CSS to style an element with the class name "cities":</p>
        <div class="cities">
            <h2>London</h2>
            <p>London is the capital of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
            <p>Standing on the River Thames, London has been a major settlement for two millennia, its history going back to its founding by the Romans, who named it Londinium.</p>
        </div> 
    </body>
</html>
```

Output:

[Click here!](./Classes/Example_1.html)

## Access elements with a specified class name, with JavaScript

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .city { background-color: tomato;
                    color: white;
                    border: 2px solid black;
                    margin: 20px;
                    padding: 20px;}
        </style>
    </head>
    <body>
        <div class="city">
            <h2>London</h2>
            <p>London is the capital of England.</p>
        </div> 
        <div class="city">
            <h2>Paris</h2>
            <p>Paris is the capital of France.</p>
        </div>
        <div class="city">
            <h2>Tokyo</h2>
            <p>Tokyo is the capital of Japan.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Classes/Example_2.html)

## Multiple classes

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .note { font-size: 120%;
                    color: red;}
        </style>
    </head>
    <body>
        <h1>My <span class="note">Important</span> Heading</h1>
        <p>This is some <span class="note">important</span> text.</p>
    </body>
</html>
```

Output:

[Click here!](./Classes/Example_3.html)

## Same class, different tag

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .city { background-color: tomato;
                    color: white;
                    padding: 10px;} 
        </style>
    </head>
    <body>
        <h2>Different Elements Can Share Same Class</h2>
        <p>Even if the two elements do not have the same tag name, they can both point to the same class, and get the same CSS styling:</p>
        <h2 class="city">Paris</h2>
        <p class="city">Paris is the capital of France.</p>
    </body>
</html>
```

Output:

[Click here!](./Classes/Example_4.html)