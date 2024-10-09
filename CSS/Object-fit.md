# Object-fit

## Use object-fit: cover

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   width: 200px;
                    height: 300px;
                    object-fit: cover;}
        </style>
    </head>
    <body>
        <h2>Using object-fit: cover</h2>

        <img src="../data/images/paris.jpg" alt="Paris" width="400" height="300">
    </body>
</html>
```

Output:

[Click here!](./Object-fit/Example_1.html)

## Use object-fit: contain

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   width: 200px;
                    height: 300px;
                    object-fit: contain;}
        </style>
    </head>
    <body>
        <h2>Using object-fit: contain</h2>

        <img src="../data/images/paris.jpg" alt="Paris" width="400" height="300">
    </body>
</html>
```

Output:

[Click here!](./Object-fit/Example_2.html)

## Use object-fit: fill

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   width: 200px;
                    height: 300px;
                    object-fit: fill;}
        </style>
    </head>
    <body>
        <h2>Using object-fit: fill</h2>

        <img src="../data/images/paris.jpg" alt="Paris" width="400" height="300">
    </body>
</html>
```

Output:

[Click here!](./Object-fit/Example_3.html)

## Use object-fit: none

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   width: 200px;
                    height: 300px;
                    object-fit: none;}
        </style>
    </head>
    <body>
        <h2>Using object-fit: none</h2>

        <img src="../data/images/paris.jpg" alt="Paris" width="400" height="300">
    </body>
</html>
```

Output:

[Click here!](./Object-fit/Example_4.html)

## Use object-fit: scale-down

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   width: 200px;
                    height: 300px;
                    object-fit: scale-down;}
        </style>
    </head>
    <body>
        <h2>Using object-fit: scale-down</h2>

        <img src="../data/images/paris.jpg" alt="Paris" width="400" height="300">
    </body>
</html>
```

Output:

[Click here!](./Object-fit/Example_5.html)

## All object-fit property values in one example

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .fill {object-fit: fill;}
            .contain {object-fit: contain;}
            .cover {object-fit: cover;}
            .scale-down {object-fit: scale-down;}
            .none {object-fit: none;}
        </style>
    </head>
    <body>
        <h1>The object-fit Property</h1>

        <h2>No object-fit:</h2>
        <img src="../data/images/paris.jpg" alt="Paris" style="width:200px;height:300px">

        <h2>object-fit: fill (this is default):</h2>
        <img class="fill" src="../data/images/paris.jpg" alt="Paris" style="width:200px;height:300px">

        <h2>object-fit: contain:</h2>
        <img class="contain" src="../data/images/paris.jpg" alt="Paris" style="width:200px;height:300px">

        <h2>object-fit: cover:</h2>
        <img class="cover" src="../data/images/paris.jpg" alt="Paris" style="width:200px;height:300px">

        <h2>object-fit: scale-down:</h2>
        <img class="scale-down" src="../data/images/paris.jpg" alt="Paris" style="width:200px;height:300px">

        <h2>object-fit: none:</h2>
        <img class="none" src="../data/images/paris.jpg" alt="Paris" style="width:200px;height:300px">
    </body>
</html>
```

Output:

[Click here!](./Object-fit/Example_6.html)