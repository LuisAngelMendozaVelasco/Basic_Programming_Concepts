# Pagination

## Simple pagination

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .pagination {display: inline-block;}

            .pagination a { color: black;
                            float: left;
                            padding: 8px 16px;
                            text-decoration: none;}
        </style>
    </head>
    <body>
        <h2>Simple Pagination</h2>

        <div class="pagination">
            <a href="#">&laquo;</a>
            <a href="#">1</a>
            <a href="#">2</a>
            <a href="#">3</a>
            <a href="#">4</a>
            <a href="#">5</a>
            <a href="#">6</a>
            <a href="#">&raquo;</a>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_1.html)

## Active and hoverable pagination

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .pagination {display: inline-block;}

            .pagination a { color: black;
                            float: left;
                            padding: 8px 16px;
                            text-decoration: none;}

            .pagination a.active {  background-color: #4CAF50;
                                    color: white;}

            .pagination a:hover:not(.active) {background-color: #ddd;}
        </style>
    </head>
    <body>
        <h2>Active and Hoverable Pagination</h2>

        <p>Move the mouse over the numbers.</p>

        <div class="pagination">
            <a href="#">&laquo;</a>
            <a href="#">1</a>
            <a class="active" href="#">2</a>
            <a href="#">3</a>
            <a href="#">4</a>
            <a href="#">5</a>
            <a href="#">6</a>
            <a href="#">&raquo;</a>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_2.html)

## Rounded active and hoverable pagination

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .pagination {display: inline-block;}

            .pagination a { color: black;
                            float: left;
                            padding: 8px 16px;
                            text-decoration: none;}

            .pagination a.active {  background-color: #4CAF50;
                                    color: white;
                                    border-radius: 5px;}

            .pagination a:hover:not(.active) {  background-color: #ddd;
                                                border-radius: 5px;}
        </style>
    </head>
    <body>
        <h2>Rounded Active and Hover Buttons</h2>

        <div class="pagination">
            <a href="#">&laquo;</a>
            <a href="#">1</a>
            <a href="#" class="active">2</a>
            <a href="#">3</a>
            <a href="#">4</a>
            <a href="#">5</a>
            <a href="#">6</a>
            <a href="#">&raquo;</a>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_3.html)

## Hoverable transition effect

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .pagination {display: inline-block;}

            .pagination a { color: black;
                            float: left;
                            padding: 8px 16px;
                            text-decoration: none;
                            transition: background-color .3s;}

            .pagination a.active {  background-color: #4CAF50;
                                    color: white;}

            .pagination a:hover:not(.active) {background-color: #ddd;}
        </style>
    </head>
    <body>
        <h2>Transition Effect on Hover</h2>

        <p>Move the mouse over the numbers.</p>

        <div class="pagination">
            <a href="#">&laquo;</a>
            <a href="#">1</a>
            <a href="#" class="active">2</a>
            <a href="#">3</a>
            <a href="#">4</a>
            <a href="#">5</a>
            <a href="#">6</a>
            <a href="#">&raquo;</a>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_4.html)

## Bordered pagination

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .pagination {display: inline-block;}

            .pagination a { color: black;
                            float: left;
                            padding: 8px 16px;
                            text-decoration: none;
                            transition: background-color .3s;
                            border: 1px solid #ddd;}

            .pagination a.active {  background-color: #4CAF50;
                                    color: white;
                                    border: 1px solid #4CAF50;}

            .pagination a:hover:not(.active) {background-color: #ddd;}
        </style>
    </head>
    <body>
        <h2>Pagination with Borders</h2>

        <div class="pagination">
            <a href="#">&laquo;</a>
            <a href="#">1</a>
            <a href="#" class="active">2</a>
            <a href="#">3</a>
            <a href="#">4</a>
            <a href="#">5</a>
            <a href="#">6</a>
            <a href="#">&raquo;</a>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_5.html)

## Rounded bordered pagination

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .pagination {display: inline-block;}

            .pagination a { color: black;
                            float: left;
                            padding: 8px 16px;
                            text-decoration: none;
                            border: 1px solid #ddd;}

            .pagination a.active {  background-color: #4CAF50;
                                    color: white;
                                    border: 1px solid #4CAF50;}

            .pagination a:hover:not(.active) {background-color: #ddd;}

            .pagination a:first-child { border-top-left-radius: 5px;
                                        border-bottom-left-radius: 5px;}

            .pagination a:last-child {  border-top-right-radius: 5px;
                                        border-bottom-right-radius: 5px;}
        </style>
    </head>
    <body>
        <h2>Pagination with Rounded Borders</h2>

        <div class="pagination">
            <a href="#">&laquo;</a>
            <a href="#">1</a>
            <a class="active" href="#">2</a>
            <a href="#">3</a>
            <a href="#">4</a>
            <a href="#">5</a>
            <a href="#">6</a>
            <a href="#">&raquo;</a>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_6.html)

## Pagination with space between links

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .pagination {display: inline-block;}

            .pagination a { color: black;
                            float: left;
                            padding: 8px 16px;
                            text-decoration: none;
                            transition: background-color .3s;
                            border: 1px solid #ddd;
                            margin: 0 4px;}

            .pagination a.active {  background-color: #4CAF50;
                                    color: white;
                                    border: 1px solid #4CAF50;}

            .pagination a:hover:not(.active) {background-color: #ddd;}
        </style>
    </head>
    <body>
        <h2>Pagination with Margins</h2>

        <div class="pagination">
            <a href="#">&laquo;</a>
            <a href="#">1</a>
            <a href="#" class="active">2</a>
            <a href="#">3</a>
            <a href="#">4</a>
            <a href="#">5</a>
            <a href="#">6</a>
            <a href="#">&raquo;</a>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_7.html)

## Pagination size

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .pagination {display: inline-block;}

            .pagination a { color: black;
                            float: left;
                            padding: 8px 16px;
                            text-decoration: none;
                            transition: background-color .3s;
                            border: 1px solid #ddd;
                            font-size: 22px;}

            .pagination a.active {  background-color: #4CAF50;
                                    color: white;
                                    border: 1px solid #4CAF50;}

            .pagination a:hover:not(.active) {background-color: #ddd;}
        </style>
    </head>
    <body>
        <h2>Pagination Size</h2>

        <p>Change the font-size property to make the pagination smaller or bigger.</p>

        <div class="pagination">
            <a href="#">&laquo;</a>
            <a href="#">1</a>
            <a href="#" class="active">2</a>
            <a href="#">3</a>
            <a href="#">4</a>
            <a href="#">5</a>
            <a href="#">6</a>
            <a href="#">&raquo;</a>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_8.html)

## Centered pagination

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .center {text-align: center;}

            .pagination {display: inline-block;}

            .pagination a { color: black;
                            float: left;
                            padding: 8px 16px;
                            text-decoration: none;
                            transition: background-color .3s;
                            border: 1px solid #ddd;
                            margin: 0 4px;}

            .pagination a.active {  background-color: #4CAF50;
                                    color: white;
                                    border: 1px solid #4CAF50;}

            .pagination a:hover:not(.active) {background-color: #ddd;}
        </style>
    </head>
    <body>
        <h2>Centered Pagination</h2>

        <div class="center">
            <div class="pagination">
                <a href="#">&laquo;</a>
                <a href="#">1</a>
                <a href="#" class="active">2</a>
                <a href="#">3</a>
                <a href="#">4</a>
                <a href="#">5</a>
                <a href="#">6</a>
                <a href="#">&raquo;</a>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_9.html)

## Breadcrumbs

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ul.breadcrumb { padding: 8px 16px;
                            list-style: none;
                            background-color: #eee;}

            ul.breadcrumb li {display: inline;}

            ul.breadcrumb li+li:before {padding: 8px;
                                        color: black;
                                        content: "/\00a0";}

            ul.breadcrumb li a {color: green;}
        </style>
    </head>
    <body>
        <h2>Breadcrumb Pagination</h2>

        <ul class="breadcrumb">
            <li><a href="#">Home</a></li>
            <li><a href="#">Pictures</a></li>
            <li><a href="#">Summer 15</a></li>
            <li>Italy</li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_10.html)

## Pagination with space between links

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ul.breadcrumb { padding: 8px 16px;
                            list-style: none;
                            background-color: #eee;}

            ul.breadcrumb li {display: inline;}

            ul.breadcrumb li+li:before {padding: 8px;
                                        color: black;
                                        content: "/\00a0";}

            ul.breadcrumb li a {color: green;}
        </style>
    </head>
    <body>
        <h2>Breadcrumb Pagination</h2>

        <ul class="breadcrumb">
            <li><a href="#">Home</a></li>
            <li><a href="#">Pictures</a></li>
            <li><a href="#">Summer 15</a></li>
            <li>Italy</li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Pagination/Example_11.html)