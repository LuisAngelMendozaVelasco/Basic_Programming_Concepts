# Tables

## - Basic HTML tables -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>HTML Tables</h2>
        <p>HTML tables start with a table tag.</p>
        <p>Table rows start with a tr tag.</p>
        <p>Table data start with a td tag.</p>
        <hr>
        <h2>1 Column:</h2>
        <table>
            <tr>
                <td>100</td>
            </tr>
        </table>
        <hr>

        <h2>1 Row and 3 Columns:</h2>
        <table>
            <tr>
                <td>100</td>
                <td>200</td>
                <td>300</td>
            </tr>
        </table>
        <hr>
        
        <h2>3 Rows and 3 Columns:</h2>
        <table>
            <tr>
                <td>100</td>
                <td>200</td>
                <td>300</td>
            </tr>
            <tr>
                <td>400</td>
                <td>500</td>
                <td>600</td>
            </tr>
            <tr>
                <td>700</td>
                <td>800</td>
                <td>900</td>
            </tr>
        </table>
        <hr>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h2>HTML Tables</h2>
<p>HTML tables start with a table tag.</p>
<p>Table rows start with a tr tag.</p>
<p>Table data start with a td tag.</p>
<hr>
<h2>1 Column:</h2>
<table>
    <tr>
        <td>100</td>
    </tr>
</table>
<hr>

<h2>1 Row and 3 Columns:</h2>
<table>
    <tr>
        <td>100</td>
        <td>200</td>
        <td>300</td>
    </tr>
</table>
<hr>

<h2>3 Rows and 3 Columns:</h2>
<table>
    <tr>
        <td>100</td>
        <td>200</td>
        <td>300</td>
    </tr>
    <tr>
        <td>400</td>
        <td>500</td>
        <td>600</td>
    </tr>
    <tr>
        <td>700</td>
        <td>800</td>
        <td>900</td>
    </tr>
</table>
<hr>
    </body>
</html>

## - A table with borders -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td {border: 1px solid black;}
        </style>
    </head>
    <body>
        <h2>Table With Border</h2>
        <p>Use the CSS border property to add a border to the table.</p>

        <table style="width:100%">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block1 {
                table, th, td {border: 1px solid black;}
            }
        </style>
    </head>
    <body>
<div id="block1">
<h2>Table With Border</h2>
<p>Use the CSS border property to add a border to the table.</p>
<table style="width:100%">
<tr>
    <th>Firstname</th>
    <th>Lastname</th> 
    <th>Age</th>
</tr>
<tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
</tr>
<tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
</tr>
<tr>
    <td>John</td>
    <td>Doe</td>
    <td>80</td>
</tr>
</table>
</div>
    </body>
</html>

## - A table with collapsed borders -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
        </style>
    </head>
    <body>
        <h2>Collapsed Borders</h2>
        <p>If you want the borders to collapse into one border, add the CSS border-collapse property.</p>

        <table style="width:100%">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block2 {
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
            }
        </style>
    </head>
    <body>
<div id="block2">
<h2>Collapsed Borders</h2>
<p>If you want the borders to collapse into one border, add the CSS border-collapse property.</p>

<table style="width:100%">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
</div>
    </body>
</html>

## - A table with cell padding -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 15px;}
        </style>
    </head>
    <body>
        <h2>Cellpadding</h2>
        <p>Cell padding specifies the space between the cell content and its borders.</p>

        <table style="width:100%">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
        
        <p><strong>Tip:</strong> Try to change the padding to 5px.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block3 {
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 15px;}
            }
        </style>
    </head>
    <body>
<div id="block3">
<h2>Cellpadding</h2>
<p>Cell padding specifies the space between the cell content and its borders.</p>

<table style="width:100%">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
        
<p><strong>Tip:</strong> Try to change the padding to 5px.</p>
</div>
    </body>
</html>

## - A table with headings -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 5px;}
        </style>
    </head>
    <body>
        <table style="width:100%">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block4 {
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 5px;}
            }
        </style>
    </head>
    <body>
<div id="block4">
<table style="width:100%">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
</div>
    </body>
</html>

## - A table with left-aligned headings -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 5px;}
            th {text-align: left;}
        </style>
    </head>
    <body>
        <h2>Left-align Headings</h2>
        <p>To left-align the table headings, use the CSS text-align property.</p>

        <table style="width:100%">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block5 {
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 5px;}
                th {text-align: left;}
            }
        </style>
    </head>
    <body>
<div id="block5">
<h2>Left-align Headings</h2>
<p>To left-align the table headings, use the CSS text-align property.</p>

<table style="width:100%">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
</div>
    </body>
</html>

## - Horizontal/Vertical table headings -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td {
                border: 1px solid black;
                border-collapse: collapse;
            }
            th, td {
                padding: 5px;
                text-align: left;
            }
        </style>
    </head>
    <body>
        <h2>Horizontal Headings:</h2>

        <table style="width:100%">
            <tr>
                <th>Name</th>
                <th>Telephone</th>
                <th>Telephone</th>
            </tr>
            <tr>
                <td>Bill Gates</td>
                <td>555 77 854</td>
                <td>555 77 855</td>
            </tr>
        </table>

        <h2>Vertical Headings:</h2>

        <table style="width:100%">
            <tr>
                <th>Name:</th>
                <td>Bill Gates</td>
            </tr>
            <tr>
                <th>Telephone:</th>
                <td>555 77 854</td>
            </tr>
            <tr>
                <th>Telephone:</th>
                <td>555 77 855</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block 6 {
                table, th, td {
                    border: 1px solid black;
                    border-collapse: collapse;
                }
                th, td {
                    padding: 5px;
                    text-align: left;
                }
            }
        </style>
    </head>
    <body>
<div id="block6">
<h2>Horizontal Headings:</h2>

<table style="width:100%">
    <tr>
        <th>Name</th>
        <th>Telephone</th>
        <th>Telephone</th>
    </tr>
    <tr>
        <td>Bill Gates</td>
        <td>555 77 854</td>
        <td>555 77 855</td>
    </tr>
</table>

<h2>Vertical Headings:</h2>

<table style="width:100%">
    <tr>
        <th>Name:</th>
        <td>Bill Gates</td>
    </tr>
    <tr>
        <th>Telephone:</th>
        <td>555 77 854</td>
    </tr>
    <tr>
        <th>Telephone:</th>
        <td>555 77 855</td>
    </tr>
</table>
</div>
    </body>
</html>

## - A table with a caption -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 5px;
                    text-align: left;}
        </style>
    </head>
    <body>
        <h2>Table Caption</h2>
        <p>To add a caption to a table, use the caption tag.</p>

        <table style="width:100%">
            <caption>Monthly savings</caption>
            <tr>
                <th>Month</th>
                <th>Savings</th>
            </tr>
            <tr>
                <td>January</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>February</td>
                <td>$50</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block7 {
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 5px;
                        text-align: left;}
            }
        </style>
    </head>
    <body>
<div id="block7">
<h2>Table Caption</h2>
<p>To add a caption to a table, use the caption tag.</p>

<table style="width:100%">
    <caption>Monthly savings</caption>
    <tr>
        <th>Month</th>
        <th>Savings</th>
    </tr>
    <tr>
        <td>January</td>
        <td>$100</td>
    </tr>
    <tr>
        <td>February</td>
        <td>$50</td>
    </tr>
</table>
</div>
    </body>
</html>

## - Table cells that span more than one column -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 5px;
                    text-align: left;}
        </style>
    </head>
    <body>
        <h2>Cell that spans two columns</h2>
        <p>To make a cell span more than one column, use the colspan attribute.</p>

        <table style="width:100%">
            <tr>
                <th>Name</th>
                <th colspan="2">Telephone</th>
            </tr>
            <tr>
                <td>Bill Gates</td>
                <td>55577854</td>
                <td>55577855</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block8 {
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 5px;
                        text-align: left;}
            }
        </style>
    </head>
    <body>
<div id="block8">
<h2>Cell that spans two columns</h2>
<p>To make a cell span more than one column, use the colspan attribute.</p>

<table style="width:100%">
    <tr>
        <th>Name</th>
        <th colspan="2">Telephone</th>
    </tr>
    <tr>
        <td>Bill Gates</td>
        <td>55577854</td>
        <td>55577855</td>
    </tr>
</table>
</div>
    </body>
</html>

## - Table cells that span more than one row -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 5px;
                    text-align: left;}
        </style>
    </head>
    <body>
        <h2>Cell that spans two rows</h2>
        <p>To make a cell span more than one row, use the rowspan attribute.</p>

        <table style="width:100%">
            <tr>
                <th>Name:</th>
                <td>Bill Gates</td>
            </tr>
            <tr>
                <th rowspan="2">Telephone:</th>
                <td>55577854</td>
            </tr>
            <tr>
                <td>55577855</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block9 {
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 5px;
                        text-align: left;}
            }
        </style>
    </head>
    <body>
<div id="block9">
<h2>Cell that spans two rows</h2>
<p>To make a cell span more than one row, use the rowspan attribute.</p>

<table style="width:100%">
    <tr>
        <th>Name:</th>
        <td>Bill Gates</td>
    </tr>
    <tr>
        <th rowspan="2">Telephone:</th>
        <td>55577854</td>
    </tr>
    <tr>
        <td>55577855</td>
    </tr>
</table>
</div>
    </body>
</html>

## - A table with cell spacing -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            padding: 5px;}
            table {border-spacing: 15px;}
        </style>
    </head>
    <body>
        <h2>Border Spacing</h2>
        <p>Border spacing specifies the space between the cells.</p>

        <table style="width:100%">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>

        <p><strong>Tip:</strong> Try to change the border-spacing to 5px.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block10 {
                table, th, td { border: 1px solid black;
                                padding: 5px;}
                table {border-spacing: 15px;}
            }
        </style>
    </head>
    <body>
<div id="block10">
<h2>Border Spacing</h2>
<p>Border spacing specifies the space between the cells.</p>

<table style="width:100%">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>

<p><strong>Tip:</strong> Try to change the border-spacing to 5px.</p>
</div>
    </body>
</html>

## - A table with HTML tags inside -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 5px;}
        </style>
    </head>
    <body>
        <table>
            <tr>
                <td>
                    <p>This is a paragraph</p>
                    <p>This is another paragraph</p>
                </td>
                <td>This cell contains a table:
                    <table>
                        <tr>
                            <td>A</td>
                            <td>B</td>
                        </tr>
                        <tr>
                            <td>C</td>
                            <td>D</td>
                        </tr>
                    </table>
                </td>
            </tr>
            <tr>
                <td>This cell contains a list
                    <ul>
                        <li>apples</li>
                        <li>bananas</li>
                        <li>pineapples</li>
                    </ul>
                </td>
                <td>HELLO</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block11{
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 5px;}
            }
        </style>
    </head>
    <body>
<div id="block11">
<table>
    <tr>
        <td>
            <p>This is a paragraph</p>
            <p>This is another paragraph</p>
        </td>
        <td>This cell contains a table:
            <table>
                <tr>
                    <td>A</td>
                    <td>B</td>
                </tr>
                <tr>
                    <td>C</td>
                    <td>D</td>
                </tr>
            </table>
        </td>
    </tr>
    <tr>
        <td>This cell contains a list
            <ul>
                <li>apples</li>
                <li>bananas</li>
                <li>pineapples</li>
            </ul>
        </td>
        <td>HELLO</td>
    </tr>
</table>
</div>
    </body>
</html>

## - Tables with different style using id I -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 15px;
                    text-align: left;}
            #t01 {  width: 100%;    
                    background-color: #f1f1c1;}
        </style>
    </head>
    <body>
        <h2>Styling Tables</h2>

        <table style="width:100%">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
        <br>

        <table id="t01">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block12 {
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 15px;
                        text-align: left;}
                #t01 {  width: 100%;    
                        background-color: #f1f1c1;}
            }
        </style>
    </head>
    <body>
<div id="block12">
<h2>Styling Tables</h2>

<table style="width:100%">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
<br>

<table id="t01">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
</div>
    </body>
</html>

## - Tables with different style using id II -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table {width:100%;}
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 15px;
                    text-align: left;}
            #t01 tr:nth-child(even) {background-color: #eee;}
            #t01 tr:nth-child(odd) {background-color: #fff;}
            #t01 th {   background-color: black;
                        color: white;}
        </style>
    </head>
    <body>
        <h2>Styling Tables</h2>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
        <br>

        <table id="t01">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block13 {
                table {width:100%;}
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 15px;
                        text-align: left;}
                #t01 tr:nth-child(even) {background-color: #eee;}
                #t01 tr:nth-child(odd) {background-color: #fff;}
                #t01 th {   background-color: black;
                            color: white;}
            }
        </style>
    </head>
    <body>
<div id="block13">
<h2>Styling Tables</h2>

<table>
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
<br>

<table id="t01">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
</div>
    </body>
</html>

## - Tables with different style using class I -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 5px;
                    text-align: left;}
            table.names {   width: 100%;    
                            background-color: #f1f1c1;}
        </style>
    </head>
    <body>
        <table style="width:100%">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>

        <br>

        <table class="names">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block14 {
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 5px;
                        text-align: left;}
                table.names {   width: 100%;    
                                background-color: #f1f1c1;}
            }
        </style>
    </head>
    <body>
<div id="block14">
<table style="width:100%">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>

<br>

<table class="names">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
</div>
    </body>
</html>

## - Tables with different style using class II -

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table {width:100%;}
            table, th, td { border: 1px solid black;
                            border-collapse: collapse;}
            th, td {padding: 5px;
                    text-align: left;}
            table.names tr:nth-child(even) {background-color: #eee;}
            table.names tr:nth-child(odd) {background-color:#fff;}
            table.names th {background-color: black;
                            color: white}
        </style>
    </head>
    <body>
        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
        <br>

        <table class="names">
            <tr>
                <th>Firstname</th>
                <th>Lastname</th> 
                <th>Age</th>
            </tr>
            <tr>
                <td>Jill</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
            <tr>
                <td>John</td>
                <td>Doe</td>
                <td>80</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <head>
        <style>
            #block15 {
                table {width:100%;}
                table, th, td { border: 1px solid black;
                                border-collapse: collapse;}
                th, td {padding: 5px;
                        text-align: left;}
                table.names tr:nth-child(even) {background-color: #eee;}
                table.names tr:nth-child(odd) {background-color:#fff;}
                table.names th {background-color: black;
                                color: white}
            }
        </style>
    </head>
    <body>
<div id="block15">
<table>
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
<br>

<table class="names">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th> 
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
    <tr>
        <td>John</td>
        <td>Doe</td>
        <td>80</td>
    </tr>
</table>
</div>
    </body>
</html>