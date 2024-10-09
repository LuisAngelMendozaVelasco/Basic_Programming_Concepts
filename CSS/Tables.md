# Tables

## Specify a black border for table, th, and td elements

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td {border: 1px solid;}
        </style>
    </head>
    <body>
        <h2>Add a border to a table:</h2>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_1.html)

## Use of border-collapse

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, td, th {border: 1px solid;}

            table { width: 100%;
                    border-collapse: collapse;}
        </style>
    </head>
    <body>
        <h2>Let the table borders collapse</h2>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_2.html)

## Single border around the table

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table { width: 100%;
                    border: 1px solid;}
        </style>
    </head>
    <body>
        <h2>Single Border Around The Table</h2>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_3.html)

## Specify the width and height of a table

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, td, th {border: 1px solid black;}

            table { border-collapse: collapse;
                    width: 100%;}

            th {height: 70px;}
        </style>
    </head>
    <body>
        <h2>The width and height Properties</h2>

        <p>Set the width of the table, and the height of the table header row:</p>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
                <th>Savings</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
                <td>$150</td>
            </tr>
            <tr>
                <td>Joe</td>
                <td>Swanson</td>
                <td>$300</td>
            </tr>
            <tr>
                <td>Cleveland</td>
                <td>Brown</td>
                <td>$250</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_4.html)

## Set the horizontal alignment of content (text-align)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, td, th {border: 1px solid black;}

            table { border-collapse: collapse;
                    width: 100%;}

            th {text-align: left;}
        </style>
    </head>
    <body>
        <h2>The text-align Property</h2>

        <p>This property sets the horizontal alignment (like left, right, or center) of the content in th or td.</p>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
                <th>Savings</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
                <td>$150</td>
            </tr>
            <tr>
                <td>Joe</td>
                <td>Swanson</td>
                <td>$300</td>
            </tr>
            <tr>
                <td>Cleveland</td>
                <td>Brown</td>
                <td>$250</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_5.html)

## Set the vertical alignment of content (vertical-align)

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, td, th {border: 1px solid black;}

            table { border-collapse: collapse;
                    width: 100%;}

            td {height: 50px;
                vertical-align: bottom;}
        </style>
    </head>
    <body>
        <h2>The vertical-align Property</h2>

        <p>This property sets the vertical alignment (like top, bottom, or middle) of the content in th or td.</p>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
                <th>Savings</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
                <td>$150</td>
            </tr>
            <tr>
                <td>Joe</td>
                <td>Swanson</td>
                <td>$300</td>
            </tr>
            <tr>
                <td>Cleveland</td>
                <td>Brown</td>
                <td>$250</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_6.html)

## Specify the padding for th and td elements

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, td, th { border: 1px solid #ddd;
                            text-align: left;}

            table { border-collapse: collapse;
                    width: 100%;}

            th, td {padding: 15px;}
        </style>
    </head>
    <body>
        <h2>The padding Property</h2>

        <p>This property adds space between the border and the content in a table.</p>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
                <th>Savings</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
                <td>$150</td>
            </tr>
            <tr>
                <td>Joe</td>
                <td>Swanson</td>
                <td>$300</td>
            </tr>
            <tr>
                <td>Cleveland</td>
                <td>Brown</td>
                <td>$250</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_7.html)

## Horizontal dividers

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table { border-collapse: collapse;
                    width: 100%;}

            th, td {padding: 8px;
                    text-align: left;
                    border-bottom: 1px solid #ddd;}
        </style>
    </head>
    <body>
        <h2>Bordered Table Dividers</h2>
        <p>Add the border-bottom property to th and td for horizontal dividers:</p>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
                <th>Savings</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
                <td>$150</td>
            </tr>
            <tr>
                <td>Joe</td>
                <td>Swanson</td>
                <td>$300</td>
            </tr>
            <tr>
                <td>Cleveland</td>
                <td>Brown</td>
                <td>$250</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_8.html)

## Hoverable table

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table { border-collapse: collapse;
                    width: 100%;}

            th, td {padding: 8px;
                    text-align: left;
                    border-bottom: 1px solid #ddd;}

            tr:hover {background-color: coral;}
        </style>
    </head>
    <body>
        <h2>Hoverable Table</h2>

        <p>Move the mouse over the table rows to see the effect.</p>

        <table>
            <tr>
                <th>First Name</th>
                <th>Last Name</th>
                <th>Points</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
                <td>$150</td>
            </tr>
            <tr>
                <td>Joe</td>
                <td>Swanson</td>
                <td>$300</td>
            </tr>
            <tr>
                <td>Cleveland</td>
                <td>Brown</td>
                <td>$250</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_9.html)

## Striped tables

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table { border-collapse: collapse;
                    width: 100%;}

            th, td {text-align: left;
                    padding: 8px;}

            tr:nth-child(even) {background-color: #f2f2f2;}
        </style>
    </head>
    <body>
        <h2>Striped Table</h2>

        <p>For zebra-striped tables, use the nth-child() selector and add a background-color to all even (or odd) table rows:</p>

        <table>
            <tr>
                <th>First Name</th>
                <th>Last Name</th>
                <th>Points</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
                <td>$150</td>
            </tr>
            <tr>
                <td>Joe</td>
                <td>Swanson</td>
                <td>$300</td>
            </tr>
            <tr>
                <td>Cleveland</td>
                <td>Brown</td>
                <td>$250</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_10.html)

## Specify the color of the table borders

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table { border-collapse: collapse;
                    width: 100%;}

            th, td {text-align: left;
                    padding: 8px;}

            tr:nth-child(even){background-color: #f2f2f2}

            th {background-color: #04AA6D;
                color: white;}
        </style>
    </head>
    <body>
        <h2>Colored Table Header</h2>

        <table>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
                <th>Savings</th>
            </tr>
            <tr>
                <td>Peter</td>
                <td>Griffin</td>
                <td>$100</td>
            </tr>
            <tr>
                <td>Lois</td>
                <td>Griffin</td>
                <td>$150</td>
            </tr>
            <tr>
                <td>Joe</td>
                <td>Swanson</td>
                <td>$300</td>
            </tr>
            <tr>
                <td>Cleveland</td>
                <td>Brown</td>
                <td>$250</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_11.html)

## Set the position of the table caption

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, td, th {border: 1px solid black;}
            caption {caption-side: bottom;}
        </style>
    </head>
    <body>
        <table>
            <caption>Table 1.1 Customers</caption>
            <tr>
                <th>Company</th>
                <th>Contact</th>
                <th>Country</th>
            </tr>
            <tr>
                <td>Alfreds Futterkiste</td>
                <td>Maria Anders</td>
                <td>Germany</td>
            </tr>
            <tr class="alt">
                <td>Berglunds snabbköp</td>
                <td>Christina Berglund</td>
                <td>Sweden</td>
            </tr>
            <tr>
                <td>Centro comercial Moctezuma</td>
                <td>Francisco Chang</td>
                <td>Mexico</td>
            </tr>
            <tr class="alt">
                <td>Ernst Handel</td>
                <td>Roland Mendel</td>
                <td>Austria</td>
            </tr>
            <tr>
                <td>Island Trading</td>
                <td>Helen Bennett</td>
                <td>UK</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_12.html)

## Responsive Table

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table { border-collapse: collapse;
                    width: 100%;}

            th, td {text-align: left;
                    padding: 8px;}

            tr:nth-child(even) {background-color: #f2f2f2;}
        </style>
    </head>
    <body>
        <h2>Responsive Table</h2>
        <p>
            A responsive table will display a horizontal scroll bar if the screen is too 
            small to display the full content. Resize the browser window to see the effect:
        </p>
        <p>To create a responsive table, add a container element (like div) with <strong>overflow-x:auto</strong> around the table element:</p>

        <div style="overflow-x: auto;">
            <table>
                <tr>
                    <th>First Name</th>
                    <th>Last Name</th>
                    <th>Points</th>
                    <th>Points</th>
                    <th>Points</th>
                    <th>Points</th>
                    <th>Points</th>
                    <th>Points</th>
                    <th>Points</th>
                    <th>Points</th>
                    <th>Points</th>
                    <th>Points</th>
                </tr>
                <tr>
                    <td>Jill</td>
                    <td>Smith</td>
                    <td>50</td>
                    <td>50</td>
                    <td>50</td>
                    <td>50</td>
                    <td>50</td>
                    <td>50</td>
                    <td>50</td>
                    <td>50</td>
                    <td>50</td>
                    <td>50</td>
                </tr>
                <tr>
                    <td>Eve</td>
                    <td>Jackson</td>
                    <td>94</td>
                    <td>94</td>
                    <td>94</td>
                    <td>94</td>
                    <td>94</td>
                    <td>94</td>
                    <td>94</td>
                    <td>94</td>
                    <td>94</td>
                    <td>94</td>
                </tr>
                <tr>
                    <td>Adam</td>
                    <td>Johnson</td>
                    <td>67</td>
                    <td>67</td>
                    <td>67</td>
                    <td>67</td>
                    <td>67</td>
                    <td>67</td>
                    <td>67</td>
                    <td>67</td>
                    <td>67</td>
                    <td>67</td>
                </tr>
            </table>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_13.html)

## Create a fancy table

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #customers {font-family: Arial, Helvetica, sans-serif;
                        border-collapse: collapse;
                        width: 100%;}

            #customers td, #customers th {  border: 1px solid #ddd;
                                            padding: 8px;}

            #customers tr:nth-child(even){background-color: #f2f2f2;}

            #customers tr:hover {background-color: #ddd;}

            #customers th { padding-top: 12px;
                            padding-bottom: 12px;
                            text-align: left;
                            background-color: #04AA6D;
                            color: white;}
        </style>
    </head>
    <body>
        <h1>A Fancy Table</h1>

        <table id="customers">
            <tr>
                <th>Company</th>
                <th>Contact</th>
                <th>Country</th>
            </tr>
            <tr>
                <td>Alfreds Futterkiste</td>
                <td>Maria Anders</td>
                <td>Germany</td>
            </tr>
            <tr>
                <td>Berglunds snabbköp</td>
                <td>Christina Berglund</td>
                <td>Sweden</td>
            </tr>
            <tr>
                <td>Centro comercial Moctezuma</td>
                <td>Francisco Chang</td>
                <td>Mexico</td>
            </tr>
            <tr>
                <td>Ernst Handel</td>
                <td>Roland Mendel</td>
                <td>Austria</td>
            </tr>
            <tr>
                <td>Island Trading</td>
                <td>Helen Bennett</td>
                <td>UK</td>
            </tr>
            <tr>
                <td>Königlich Essen</td>
                <td>Philip Cramer</td>
                <td>Germany</td>
            </tr>
            <tr>
                <td>Laughing Bacchus Winecellars</td>
                <td>Yoshi Tannamuri</td>
                <td>Canada</td>
            </tr>
            <tr>
                <td>Magazzini Alimentari Riuniti</td>
                <td>Giovanni Rovelli</td>
                <td>Italy</td>
            </tr>
            <tr>
                <td>North/South</td>
                <td>Simon Crowther</td>
                <td>UK</td>
            </tr>
            <tr>
                <td>Paris spécialités</td>
                <td>Marie Bertrand</td>
                <td>France</td>
            </tr>
        </table>
    </body>
</html>
```

Output:

[Click here!](./Tables/Example_14.html)