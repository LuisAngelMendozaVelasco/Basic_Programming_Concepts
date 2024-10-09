# Lists

## All the different list item markers in lists

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ul.a {list-style-type: circle;}
            ul.b {list-style-type: disc;}
            ul.c {list-style-type: square;}

            ol.d {list-style-type: armenian;}
            ol.e {list-style-type: cjk-ideographic;}
            ol.f {list-style-type: decimal;}
            ol.g {list-style-type: decimal-leading-zero;}
            ol.h {list-style-type: georgian;}
            ol.i {list-style-type: hebrew;}
            ol.j {list-style-type: hiragana;}
            ol.k {list-style-type: hiragana-iroha;}
            ol.l {list-style-type: katakana;}
            ol.m {list-style-type: katakana-iroha;}
            ol.n {list-style-type: lower-alpha;}
            ol.o {list-style-type: lower-greek;}
            ol.p {list-style-type: lower-latin;}
            ol.q {list-style-type: lower-roman;}
            ol.r {list-style-type: upper-alpha;}
            ol.s {list-style-type: upper-latin;}
            ol.t {list-style-type: upper-roman;}
            ol.u {list-style-type: none;}
            ol.v {list-style-type: inherit;}
        </style>
    </head>
    <body>
        <h2>All List Style Types</h2>

        <ul class="a">
            <li>Circle type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ul>

        <ul class="b">
            <li>Disc type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ul>

        <ul class="c">
            <li>Square type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ul>

        <ol class="d">
            <li>Armenian type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="e">
            <li>Cjk-ideographic type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="f">
            <li>Decimal type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="g">
            <li>Decimal-leading-zero type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="h">
            <li>Georgian type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="i">
            <li>Hebrew type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="j">
            <li>Hiragana type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="k">
            <li>Hiragana-iroha type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="l">
            <li>Katakana type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="m">
            <li>Katakana-iroha type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="n">
            <li>Lower-alpha type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="o">
            <li>Lower-greek type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="p">
            <li>Lower-latin type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="q">
            <li>Lower-roman type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="r">
            <li>Upper-alpha type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="s">
            <li>Upper-latin type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="t">
            <li>Upper-roman type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="u">
            <li>None type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ol class="v">
            <li>inherit type</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>
    </body>
</html>
```

Output:

[Click here!](./Lists/Example_1.html)

## Set an image as the list-item marker

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ul {list-style-image: url('../data/images/sqpurple.gif');}
        </style>
    </head>
    <body>
        <h2>The list-style-image Property</h2>

        <p>The list-style-image property specifies an image as the list item marker:</p>

        <ul>
            <li>Coffee</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Lists/Example_2.html)

## Position the list-item marker

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ul.a {list-style-position: outside;}
            ul.b {list-style-position: inside;}
        </style>
    </head>
    <body>
        <h1>The list-style-position Property</h1>

        <h2>list-style-position: outside (default):</h2>
        <ul class="a">
            <li>Coffee - A brewed drink prepared from roasted coffee beans, which are the seeds of berries from the Coffea plant</li>
            <li>Tea - An aromatic beverage commonly prepared by pouring hot or boiling water over cured leaves of the Camellia sinensis, an evergreen shrub (bush) native to Asia</li>
            <li>Coca Cola - A carbonated soft drink produced by The Coca-Cola Company. The drink's name refers to two of its original ingredients, which were kola nuts (a source of caffeine) and coca leaves</li>
        </ul>

        <h2>list-style-position: inside:</h2>
        <ul class="b">
            <li>Coffee - A brewed drink prepared from roasted coffee beans, which are the seeds of berries from the Coffea plant</li>
            <li>Tea - An aromatic beverage commonly prepared by pouring hot or boiling water over cured leaves of the Camellia sinensis, an evergreen shrub (bush) native to Asia</li>
            <li>Coca Cola - A carbonated soft drink produced by The Coca-Cola Company. The drink's name refers to two of its original ingredients, which were kola nuts (a source of caffeine) and coca leaves</li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Lists/Example_3.html)

## Remove default list settings

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ul.demo {   list-style-type: none;
                        margin: 0;
                        padding: 0;}
        </style>
    </head>
    <body>
        <p>Default list:</p>
        <ul>
            <li>Coffee</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ul>

        <p>Remove bullets, margin and padding from list:</p>
        <ul class="demo">
            <li>Coffee</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Lists/Example_4.html)

## All list properties in one declaration

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ul {list-style: square inside url("../data/images/sqpurple.gif");}
        </style>
    </head>
    <body>
        <h2>The list-style Property</h2>

        <p>The list-style property is a shorthand property, which is used to set all the list properties in one declaration.</p>

        <ul>
            <li>Coffee</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Lists/Example_5.html)

## Style lists with colors

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ol {background: #ff9999;
                padding: 20px; }

            ul {background: #3399ff;
                padding: 20px;}

            ol li { background: #ffe5e5;
                    color: darkred;
                    padding: 5px;
                    margin-left: 35px;}

            ul li { background: #cce5ff;
                    color: darkblue;
                    margin: 5px;}
        </style>
    </head>
    <body>
        <h1>Styling Lists With Colors</h1>

        <ol>
            <li>Coffee</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ol>

        <ul>
            <li>Coffee</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Lists/Example_6.html)

## Full-width bordered list

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            ul {list-style-type: none;
                padding: 0;
                border: 1px solid #ddd;}

            ul li { padding: 8px 16px;
                    border-bottom: 1px solid #ddd;}

            ul li:last-child {border-bottom: none}
        </style>
    </head>
    <body>
        <h2>A bordered list</h2>

        <ul>
            <li>Coffee</li>
            <li>Tea</li>
            <li>Coca Cola</li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Lists/Example_7.html)