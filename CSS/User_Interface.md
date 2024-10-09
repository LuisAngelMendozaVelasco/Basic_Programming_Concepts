# User Interface

## Let a user resize the width of an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   border: 2px solid;
                    padding: 20px; 
                    width: 300px;
                    resize: horizontal;
                    overflow: auto;}
        </style>
    </head>
    <body>
        <h1>The resize Property</h1>

        <div>
            <p>Let the user resize only the width of this div element.</p>
            <p>To resize: Click and drag the bottom right corner of this div element.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./User_Interface/Example_1.html)

## Let a user resize the height of an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   border: 2px solid;
                    padding: 20px; 
                    width: 300px;
                    resize: vertical;
                    overflow: auto;}
        </style>
    </head>
    <body>
        <h1>The resize Property</h1>

        <div>
            <p>Let the user resize only the height of this div element.</p>
            <p>To resize: Click and drag the bottom right corner of this div element.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./User_Interface/Example_2.html)

## Let a user resize both the width and height of an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div {   border: 2px solid;
                    padding: 20px; 
                    width: 300px;
                    resize: both;
                    overflow: auto;}
        </style>
    </head>
    <body>
        <h1>The resize Property</h1>

        <div>
            <p>Let the user resize both the height and the width of this div element.</p>
            <p>To resize: Click and drag the bottom right corner of this div element.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./User_Interface/Example_3.html)

## Add space between an outline and the border of an element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div.ex1 {   margin: 20px;
                        border: 1px solid black;
                        outline: 4px solid red;
                        outline-offset: 15px;} 

            div.ex2 {   margin: 10px;
                        border: 1px solid black;
                        outline: 5px dashed blue;
                        outline-offset: 5px;} 
        </style>
    </head>
    <body>
        <h1>The outline-offset Property</h1>

        <div class="ex1">This div has a 4 pixels solid red outline 15 pixels outside the border edge.</div><br>

        <div class="ex2">This div has a 5 pixels dashed blue outline 5 pixels outside the border edge.</div>
    </body>
</html>
```

Output:

[Click here!](./User_Interface/Example_4.html)