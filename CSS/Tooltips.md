# Tooltips

## Right tooltip

Code: 

```html
<!DOCTYPE html>
<html>
    <style>
        .tooltip {  position: relative;
                    display: inline-block;
                    border-bottom: 1px dotted black;}

        .tooltip .tooltiptext { visibility: hidden;
                                width: 120px;
                                background-color: black;
                                color: #fff;
                                text-align: center;
                                border-radius: 6px;
                                padding: 5px 0;
                                
                                /* Position the tooltip */
                                position: absolute;
                                z-index: 1;
                                top: -5px;
                                left: 105%;}

        .tooltip:hover .tooltiptext {visibility: visible;}
    </style>
    <body style="text-align:center;">
        <h2>Right Tooltip</h2>
        <p>Move the mouse over the text below:</p>

        <div class="tooltip">Hover over me
            <span class="tooltiptext">Tooltip text</span>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Tooltips/Example_1.html)

## Left tooltip

Code: 

```html
<!DOCTYPE html>
<html>
    <style>
        .tooltip {  position: relative;
                    display: inline-block;
                    border-bottom: 1px dotted black;}

        .tooltip .tooltiptext { visibility: hidden;
                                width: 120px;
                                background-color: black;
                                color: #fff;
                                text-align: center;
                                border-radius: 6px;
                                padding: 5px 0;
                                
                                /* Position the tooltip */
                                position: absolute;
                                z-index: 1;
                                top: -5px;
                                right: 105%;}

        .tooltip:hover .tooltiptext {visibility: visible;}
    </style>
    <body style="text-align:center;">
        <h2>Left Tooltip</h2>
        <p>Move the mouse over the text below:</p>

        <div class="tooltip">Hover over me
            <span class="tooltiptext">Tooltip text</span>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Tooltips/Example_2.html)

## Top tooltip

Code: 

```html
<!DOCTYPE html>
<html>
    <style>
        .tooltip {  position: relative;
                    display: inline-block;
                    border-bottom: 1px dotted black;}

        .tooltip .tooltiptext { visibility: hidden;
                                width: 120px;
                                background-color: black;
                                color: #fff;
                                text-align: center;
                                border-radius: 6px;
                                padding: 5px 0;
                                
                                /* Position the tooltip */
                                position: absolute;
                                z-index: 1;
                                bottom: 100%;
                                left: 50%;
                                margin-left: -60px;}

        .tooltip:hover .tooltiptext {visibility: visible;}
    </style>
    <body style="text-align:center;">
        <h2>Top Tooltip</h2>
        <p>Move the mouse over the text below:</p>

        <div class="tooltip">Hover over me
            <span class="tooltiptext">Tooltip text</span>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Tooltips/Example_3.html)

## Bottom tooltip

Code: 

```html
<!DOCTYPE html>
<html>
    <style>
        .tooltip {  position: relative;
                    display: inline-block;
                    border-bottom: 1px dotted black;}

        .tooltip .tooltiptext { visibility: hidden;
                                width: 120px;
                                background-color: black;
                                color: #fff;
                                text-align: center;
                                border-radius: 6px;
                                padding: 5px 0;
                                
                                /* Position the tooltip */
                                position: absolute;
                                z-index: 1;
                                top: 100%;
                                left: 50%;
                                margin-left: -60px;}

        .tooltip:hover .tooltiptext {visibility: visible;}
    </style>
    <body style="text-align:center;">
        <h2>Bottom Tooltip</h2>
        <p>Move the mouse over the text below:</p>

        <div class="tooltip">Hover over me
            <span class="tooltiptext">Tooltip text</span>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Tooltips/Example_4.html)

## Tooltip with arrow

Code: 

```html
<!DOCTYPE html>
<html>
    <style>
        .tooltip {  position: relative;
                    display: inline-block;
                    border-bottom: 1px dotted black;}

        .tooltip .tooltiptext { visibility: hidden;
                                width: 120px;
                                background-color: black;
                                color: #fff;
                                text-align: center;
                                border-radius: 6px;
                                padding: 5px 0;
                                position: absolute;
                                z-index: 1;
                                bottom: 150%;
                                left: 50%;
                                margin-left: -60px;}

        .tooltip .tooltiptext::after {  content: "";
                                        position: absolute;
                                        top: 100%;
                                        left: 50%;
                                        margin-left: -5px;
                                        border-width: 5px;
                                        border-style: solid;
                                        border-color: black transparent transparent transparent;}

        .tooltip:hover .tooltiptext {visibility: visible;}
    </style>
    <body style="text-align:center;">
        <h2>Top Tooltip w/ Bottom Arrow</h2>

        <div class="tooltip">Hover over me
            <span class="tooltiptext">Tooltip text</span>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Tooltips/Example_5.html)

## Animated tooltip

Code: 

```html
<!DOCTYPE html>
<html>
    <style>
        .tooltip {  position: relative;
                    display: inline-block;
                    border-bottom: 1px dotted black;}

        .tooltip .tooltiptext { visibility: hidden;
                                width: 120px;
                                background-color: black;
                                color: #fff;
                                text-align: center;
                                border-radius: 6px;
                                padding: 5px 0;
                                position: absolute;
                                z-index: 1;
                                bottom: 100%;
                                left: 50%;
                                margin-left: -60px;
                                
                                /* Fade in tooltip - takes 1 second to go from 0% to 100% opac: */
                                opacity: 0;
                                transition: opacity 1s;}

        .tooltip:hover .tooltiptext {   visibility: visible;
                                        opacity: 1;}
    </style>
    <body style="text-align:center;">
        <h2>Fade In Tooltip on Hover</h2>
        <p>When you move the mouse over the text below, the tooltip text will fade in and take 1 second to go from completely invisible to visible.</p>

        <div class="tooltip">Hover over me
            <span class="tooltiptext">Tooltip text</span>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Tooltips/Example_6.html)