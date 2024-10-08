# Div Element

## - `<div>` elements come with linebreaks -

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

<!DOCTYPE html>
<html>
    <style>
        #block1 {
            div {background-color: #FFF4A3;}
        }
    </style>
    <body>
<div id="block1">
<h1>HTML DIV Example</h1>

Lorem Ipsum <div>I am a div</div> dolor sit amet.

<p>The yellow background is added to demonstrate the footprint of the DIV element.</p>
</div>
    </body>
</html>

## - `<div>` as a container -

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

<!DOCTYPE html>
<html>
    <style>
        #block2{
            div {background-color: #FFF4A3;}
        }
    </style>
    <body>
<div id="block2">
<h1>HTML DIV Example</h1>

<div>
    <h2>London</h2>
    <p>London is the capital city of England.</p>
    <p>London has over 13 million inhabitants.</p>
</div>

<p>The yellow background is added to demonstrate the footprint of the DIV element.</p>
</div>
    </body>
</html>

## - Center align a `<div>` element -

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

<!DOCTYPE html>
<html>
    <style>
        #block3 {
            div {   width: 300px;
                    margin: auto;
                    background-color: #FFF4A3;}
        }
    </style>
    <body>
<div id="block3">
<h1>Center align a DIV element</h1>

<div>
    <h2>London</h2>
    <p>London is the capital city of England.</p>
    <p>London has over 13 million inhabitants.</p>
</div>
</div>
    </body>
</html>

## - Multiple `<div>` elements -

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

## - Floating `<div>` elements -

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

<!DOCTYPE html>
<html>
    <style>
        #block4 {
            div.mycontainer {   width:100%;
                                overflow:auto;}
            div.mycontainer div {   width:33%;  
                                    float:left;}
        }
    </style>
    <body>
<div id="block4">
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
</div>
    </body>
</html>

## - Position `<div>` elements with display:inline-block -

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

<!DOCTYPE html>
<html>
    <style>
        #block5 {
            div {   width:30%;  
                    display:inline-block;}
        }
    </style>
    <body>
<div id="block5">
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

## - Position `<div>` elements with display:flex -

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

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block6 {
                .mycontainer {display: flex;}
                .mycontainer > div {width:33%;}
            }
        </style>
    </head>
    <body>
<div id="block6">
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
</div>
    </body>
</html>

## - Position `<div>` elements with display:grid -

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

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block7 {
            .grid-container {   display: grid;
                                grid-template-columns: 33% 33% 33%;}
            }
        </style>
    </head>
    <body>
<div id="block7">
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
</div>
    </body>
</html>