# Div Element

## `<div>` elements come with linebreaks

Code:

```html
<!DOCTYPE html>
<html>
    <style>
        div {background-color: #FFF4A3;}
    </style>
    <body>
        <h1>HTML DIV Example</h1>

        Lorem Ipsum <div>I am a div</div> dolor sit amet.

        <p>The yellow background is added to demonstrate the footprint of the DIV element.</p>
    </body>
</html>
```

Output:

[Click here!](./Div_Element/Example_1.html)

## `<div>` as a container

Code:

```html
<!DOCTYPE html>
<html>
    <style>
        div {background-color: #FFF4A3;}
    </style>
    <body>
        <h1>HTML DIV Example</h1>

        <div>
            <h2>London</h2>
            <p>London is the capital city of England.</p>
            <p>London has over 13 million inhabitants.</p>
        </div>

        <p>The yellow background is added to demonstrate the footprint of the DIV element.</p>
    </body>
</html>
```

Output:

[Click here!](./Div_Element/Example_2.html)

## Center align a `<div>` element

Code:

```html
<!DOCTYPE html>
<html>
    <style>
        div {   width: 300px;
                margin: auto;
                background-color: #FFF4A3;}
    </style>
    <body>
        <h1>Center align a DIV element</h1>

        <div>
            <h2>London</h2>
            <p>London is the capital city of England.</p>
            <p>London has over 13 million inhabitants.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Div_Element/Example_3.html)

## Multiple `<div>` elements

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Multiple DIV Elements</h1>

        <div style="background-color:#FFF4A3;">
            <h2>London</h2>
            <p>London is the capital city of England.</p>
            <p>London has over 13 million inhabitants.</p>
        </div>

        <div style="background-color:#FFC0C7;">
            <h2>Oslo</h2>
            <p>Oslo is the capital city of Norway.</p>
            <p>Oslo has over 600.000 inhabitants.</p>
        </div>

        <div style="background-color:#D9EEE1;">
            <h2>Rome</h2>
            <p>Rome is the capital city of Italy.</p>
            <p>Rome has almost 3 million inhabitants.</p>
        </div>

        <p>CSS styles are added to make it easier to separate the divs, and to meake them more pretty:)</p>
    </body>
</html>
```

Output:

[Click here!](./Div_Element/Example_4.html)

## Floating `<div>` elements

Code:

```html
<!DOCTYPE html>
<html>
    <style>
        div.mycontainer {   width:100%;
                            overflow:auto;}
        div.mycontainer div {   width:33%;  
                                float:left;}
    </style>
    <body>
        <div class="mycontainer">
            <div style="background-color:#FFF4A3;">
                <h2>London</h2>
                <p>London is the capital city of England.</p>
                <p>London has over 13 million inhabitants.</p>
            </div>
            
            <div style="background-color:#FFC0C7;">
                <h2>Oslo</h2>
                <p>Oslo is the capital city of Norway.</p>
                <p>Oslo has over 600.000 inhabitants.</p>
            </div>
            
            <div style="background-color:#D9EEE1;">
                <h2>Rome</h2>
                <p>Rome is the capital city of Italy.</p>
                <p>Rome has almost 3 million inhabitants.</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Div_Element/Example_5.html)

## Position `<div>` elements with display:inline-block

Code:

```html
<!DOCTYPE html>
<html>
    <style>
        div {   width:30%;  
                display:inline-block;}
    </style>
    <body>
        <div style="background-color:#FFF4A3;">
            <h2>London</h2>
            <p>London is the capital city of England.</p>
            <p>London has over 13 million inhabitants.</p>
        </div>

        <div style="background-color:#FFC0C7;">
            <h2>Oslo</h2>
            <p>Oslo is the capital city of Norway.</p>
            <p>Oslo has over 600.000 inhabitants.</p>
        </div>

        <div style="background-color:#D9EEE1;">
            <h2>Rome</h2>
            <p>Rome is the capital city of Italy.</p>
            <p>Rome has almost 3 million inhabitants.</p>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Div_Element/Example_6.html)

## Position `<div>` elements with display:flex

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .mycontainer {display: flex;}
            .mycontainer > div {width:33%;}
        </style>
    </head>
    <body>
        <h1>Flexbox Example</h1>

        <p>Align three DIV elements side by side.</p>

        <div class="mycontainer">

            <div style="background-color:#FFF4A3;">
                <h2>London</h2>
                <p>London is the capital city of England.</p>
                <p>London has over 13 million inhabitants.</p>
            </div>
            
            <div style="background-color:#FFC0C7;">
                <h2>Oslo</h2>
                <p>Oslo is the capital city of Norway.</p>
                <p>Oslo has over 600.000 inhabitants.</p>
            </div>
            
            <div style="background-color:#D9EEE1;">
                <h2>Rome</h2>
                <p>Rome is the capital city of Italy.</p>
                <p>Rome has almost 3 million.</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Div_Element/Example_7.html)

## Position `<div>` elements with display:grid

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .grid-container {   display: grid;
                                grid-template-columns: 33% 33% 33%;}
        </style>
    </head>
    <body>
        <h1>Grid Example</h1>

        <p>Align three DIV elements side by side.</p>

        <div class="grid-container">
            <div style="background-color:#FFF4A3;">
                <h2>London</h2>
                <p>London is the capital city of England.</p>
                <p>London has over 13 million inhabitants.</p>
            </div>

            <div style="background-color:#FFC0C7;">
                <h2>Oslo</h2>
                <p>Oslo is the capital city of Norway.</p>
                <p>Oslo has over 600.000 inhabitants.</p>
            </div>

            <div style="background-color:#D9EEE1;">
                <h2>Rome</h2>
                <p>Rome is the capital city of Italy.</p>
                <p>Rome has almost 3 million inhabitants.</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Div_Element/Example_8.html)