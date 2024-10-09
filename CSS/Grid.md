# Grid

## Grid layout

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .item1 { grid-area: header; }
            .item2 { grid-area: menu; }
            .item3 { grid-area: main; }
            .item4 { grid-area: right; }
            .item5 { grid-area: footer; }

            .grid-container {   display: grid;
                                grid-template-areas:'header header header header header header'
                                                    'menu main main main right right'
                                                    'menu footer footer footer footer footer';
                                gap: 10px;
                                background-color: #2196F3;
                                padding: 10px;}

            .grid-container > div { background-color: rgba(255, 255, 255, 0.8);
                                    text-align: center;
                                    padding: 20px 0;
                                    font-size: 30px;}
        </style>
    </head>
    <body>
        <h1>Grid Layout</h1>

        <p>This grid layout contains six columns and three rows:</p>

        <div class="grid-container">
            <div class="item1">Header</div>
            <div class="item2">Menu</div>
            <div class="item3">Main</div>  
            <div class="item4">Right</div>
            <div class="item5">Footer</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Grid/Example_1.html)

## Grid elements

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .grid-container {   display: grid;
                                grid-template-columns: auto auto auto;
                                background-color: #2196F3;
                                padding: 10px;}

            .grid-item {background-color: rgba(255, 255, 255, 0.8);
                        border: 1px solid rgba(0, 0, 0, 0.8);
                        padding: 20px;
                        font-size: 30px;
                        text-align: center;}
        </style>
    </head>
    <body>
        <h1>Grid Elements</h1>

        <p>A Grid Layout must have a parent element with the <em>display</em> property set to <em>grid</em> or <em>inline-grid</em>.</p>

        <p>Direct child element(s) of the grid container automatically becomes grid items.</p>

        <div class="grid-container">
            <div class="grid-item">1</div>
            <div class="grid-item">2</div>
            <div class="grid-item">3</div>  
            <div class="grid-item">4</div>
            <div class="grid-item">5</div>
            <div class="grid-item">6</div>  
            <div class="grid-item">7</div>
            <div class="grid-item">8</div>
            <div class="grid-item">9</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Grid/Example_2.html)

## Grid column gaps

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .grid-container {   display: grid;
                                column-gap: 50px;
                                grid-template-columns: auto auto auto;
                                background-color: #2196F3;
                                padding: 10px;}

            .grid-item {background-color: rgba(255, 255, 255, 0.8);
                        border: 1px solid rgba(0, 0, 0, 0.8);
                        padding: 20px;
                        font-size: 30px;
                        text-align: center;}
        </style>
    </head>
    <body>
        <h1>The column-gap Property</h1>

        <p>Use the <em>column-gap</em> property to adjust the space between the columns:</p>

        <div class="grid-container">
            <div class="grid-item">1</div>
            <div class="grid-item">2</div>
            <div class="grid-item">3</div>  
            <div class="grid-item">4</div>
            <div class="grid-item">5</div>
            <div class="grid-item">6</div>  
            <div class="grid-item">7</div>
            <div class="grid-item">8</div>
            <div class="grid-item">9</div>  
        </div>
    </body>
</html>
```

Output:

[Click here!](./Grid/Example_3.html)

## Grid lines

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .grid-container {   display: grid;
                                grid-template-columns: auto auto auto;
                                gap: 10px;
                                background-color: #2196F3;
                                padding: 10px;}

            .grid-container > div { background-color: rgba(255, 255, 255, 0.8);
                                    text-align: center;
                                    padding: 20px 0;
                                    font-size: 30px;}

            .item1 {grid-column-start: 1;
                    grid-column-end: 3;}
        </style>
    </head>
    <body>
        <h1>Grid Lines</h1>

        <div class="grid-container">
            <div class="item1">1</div>
            <div class="item2">2</div>
            <div class="item3">3</div>  
            <div class="item4">4</div>
            <div class="item5">5</div>
            <div class="item6">6</div>
            <div class="item7">7</div>
            <div class="item8">8</div>  
        </div>

        <p>You can refer to line numbers when placing grid items.</p>
    </body>
</html>
```

Output:

[Click here!](./Grid/Example_4.html)

## Grid container

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .grid-container {   display: grid;
                                grid-template-columns: auto auto auto auto;
                                gap: 10px;
                                background-color: #2196F3;
                                padding: 10px;}

            .grid-container > div { background-color: rgba(255, 255, 255, 0.8);
                                    border: 1px solid black;
                                    text-align: center;
                                    font-size: 30px;}
        </style>
    </head>
    <body>
        <h1>Grid Container</h1>

        <p>A Grid Container consists of grid items arranged in columns and rows</p>

        <div class="grid-container">
            <div>1</div>
            <div>2</div>
            <div>3</div>  
            <div>4</div>
            <div>5</div>
            <div>6</div>
            <div>7</div>
            <div>8</div>
        </div>

        <p>Direct child elements(s) of the grid container automatically becomes grid items.</p>
    </body>
</html>
```

Output:

[Click here!](./Grid/Example_5.html)

## Grid items

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .grid-container {   display: grid;
                                gap: 10px;
                                background-color: #2196F3;
                                padding: 10px;}

            .grid-item {background-color: rgba(255, 255, 255, 0.8);
                        text-align: center;
                        padding: 20px;
                        font-size: 30px;}

            .item1 {grid-column: 1 / span 2;
                    grid-row: 1;}

            .item2 {grid-column: 3;
                    grid-row: 1 / span 2;}

            .item5 {grid-column: 1 / span 3;
                    grid-row: 3;}
        </style>
    </head>
    <body>
        <h1>A Five Items Grid Layout</h1>

        <div class="grid-container">
            <div class="grid-item item1">1</div>
            <div class="grid-item item2">2</div>
            <div class="grid-item item3">3</div>  
            <div class="grid-item item4">4</div>
            <div class="grid-item item5">5</div>
        </div>

        <p>Direct child elements(s) of the grid container automatically becomes grid items.</p>

        <p>Item 1, 2, and 5 are set to span multiple columns or rows.</p>
    </body>
</html>
```

Output:

[Click here!](./Grid/Example_6.html)