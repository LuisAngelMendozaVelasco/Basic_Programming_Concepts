# Multiple Columns

## Create multiple columns

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .newspaper {column-count: 3;}
        </style>
    </head>
    <body>
        <h1>Create Multiple Columns</h1>

        <div class="newspaper">
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Multiple_Columns/Example_1.html)

## Specify the gap between columns

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .newspaper {column-count: 3;
                        column-gap: 40px;}
        </style>
    </head>
    <body>
        <h1>Specify the Gap Between Columns</h1>

        <div class="newspaper">
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum. 
        </div>
    </body>
</html>
```

Output:

[Click here!](./Multiple_Columns/Example_2.html)

## Specify the style of the rule between columns

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .newspaper {column-count: 3;
                        column-gap: 40px;
                        column-rule-style: solid;}
        </style>
    </head>
    <body>
        <h1>Add a Rule Between the Columns</h1>

        <div class="newspaper">
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Multiple_Columns/Example_3.html)

## Specify the width of the rule between columns

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .newspaper {column-count: 3;
                        column-gap: 40px;
                        column-rule-style: solid;
                        column-rule-width: 1px;}
        </style>
    </head>
    <body>
        <h1>Set the Rule Width</h1>

        <div class="newspaper">
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Multiple_Columns/Example_4.html)

## Specify the color of the rule between columns

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .newspaper {column-count: 3;
                        column-gap: 40px;
                        column-rule-style: solid;
                        column-rule-width: 1px;
                        column-rule-color: lightblue;}
        </style>
    </head>
    <body>
        <h1>Set the Rule Color</h1>

        <div class="newspaper">
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Multiple_Columns/Example_5.html)

## Specify the width, style and color of the rule between columns

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .newspaper {column-count: 3;
                        column-gap: 40px;
                        column-rule: 1px solid lightblue;}
        </style>
    </head>
    <body>
        <h1>Use the column-rule Shorthand Property</h1>

        <div class="newspaper">
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Multiple_Columns/Example_6.html)

## Specify how many columns an element should span across

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .newspaper {column-count: 3;
                        column-gap: 40px;
                        column-rule: 1px solid lightblue;}

            h2 {column-span: all;}
        </style>
    </head>
    <body>
        <div class="newspaper">
            <h2>Lorem Ipsum Dolor Sit Amet</h2>
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Multiple_Columns/Example_7.html)

## Specify a suggested, optimal width for the columns

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            .newspaper {column-width: 100px;}
        </style>
    </head>
    <body>
        <h1>Specify The Column Width</h1>

        <div class="newspaper">
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.
        </div>
    </body>
</html>
```

Output:

[Click here!](./Multiple_Columns/Example_8.html)