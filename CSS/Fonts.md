# Fonts

## Set the font of a text

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .p1 {font-family: "Times New Roman", Times, serif;}
            .p2 {font-family: Arial, Helvetica, sans-serif;}
            .p3 {font-family: "Lucida Console", "Courier New", monospace;}
        </style>
    </head>
    <body>
        <h1>CSS font-family</h1>
        <p class="p1">This is a paragraph, shown in the Times New Roman font.</p>
        <p class="p2">This is a paragraph, shown in the Arial font.</p>
        <p class="p3">This is a paragraph, shown in the Lucida Console font.</p>
    </body>
</html>
```

Output:

[Click here!](./Fonts/Example_1.html)

## Set the size of the font

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {font-size: 250%;}
            h2 {font-size: 200%;}
            p {font-size: 100%;}
        </style>
    </head>
    <body>
        <h1>This is heading 1</h1>
        <h2>This is heading 2</h2>
        <p>This is a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Fonts/Example_2.html)

## Set the size of the font in px

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {font-size: 40px;}
            h2 {font-size: 30px;}
            p {font-size: 14px;}
        </style>
    </head>
    <body>
        <h1>This is heading 1</h1>
        <h2>This is heading 2</h2>
        <p>This is a paragraph.</p>
        <p>This is another paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Fonts/Example_3.html)

## Set the size of the font in em

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {font-size: 2.5em;} /* 40px/16=2.5em */
            h2 {font-size: 1.875em;} /* 30px/16=1.875em */
            p {font-size: 0.875em;} /* 14px/16=0.875em */
        </style>
    </head>
    <body>
        <h1>This is heading 1</h1>
        <h2>This is heading 2</h2>
        <p>This is a paragraph.</p>
        <p>
            Specifying the font-size in em allows all major browsers to resize the text.
            Unfortunately, there is still a problem with older versions of IE. When resizing the text, it becomes larger/smaller than it should.
        </p>
    </body>
</html>
```

Output:

[Click here!](./Fonts/Example_4.html)

## Set the size of the font in percent and em

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {font-size: 100%;}
            h1 {font-size: 2.5em;}
            h2 {font-size: 1.875em;}
            p {font-size: 0.875em;}
        </style>
    </head>
    <body>
        <h1>This is heading 1</h1>
        <h2>This is heading 2</h2>
        <p>This is a paragraph.</p>
        <p>Specifying the font-size in percent and em displays the same size in all major browsers, and allows all browsers to resize the text!</p>
    </body>
</html>
```

Output:

[Click here!](./Fonts/Example_5.html)

## Set the style of the font

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.normal {font-style: normal;}
            p.italic {font-style: italic;}
            p.oblique {font-style: oblique;}
        </style>
    </head>
    <body>
        <h1>The font-style property</h1>

        <p class="normal">This is a paragraph in normal style.</p>
        <p class="italic">This is a paragraph in italic style.</p>
        <p class="oblique">This is a paragraph in oblique style.</p>
    </body>
</html>
```

Output:

[Click here!](./Fonts/Example_6.html)

## Set the variant of the font

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.normal {font-variant: normal;}
            p.small {font-variant: small-caps;}
        </style>
    </head>
    <body>
        <h1>The font-variant property</h1>

        <p class="normal">My name is Hege Refsnes.</p>
        <p class="small">My name is Hege Refsnes.</p>
    </body>
</html>
```

Output:

[Click here!](./Fonts/Example_7.html)

## Set the boldness of the font

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.normal {font-weight: normal;}
            p.light {font-weight: lighter;}
            p.thick {font-weight: bold;}
            p.thicker {font-weight: 900;}
        </style>
    </head>
    <body>
        <h1>The font-weight property</h1>

        <p class="normal">This is a paragraph.</p>
        <p class="light">This is a paragraph.</p>
        <p class="thick">This is a paragraph.</p>
        <p class="thicker">This is a paragraph.</p>
    </body>
</html>
```

Output:

[Click here!](./Fonts/Example_8.html)

## All the font properties in one declaration

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p.a {font: 20px Arial, sans-serif;}
            p.b {font: italic bold 12px/30px Georgia, serif;}
        </style>
    </head>
    <body>
        <h1>The font Property</h1>

        <p class="a">This is a paragraph. The font size is set to 20 pixels, and the font family is Arial.</p>

        <p class="b">This is a paragraph. The font is set to italic and bold, the font size is set to 12 pixels, the line height is set to 30 pixels, and the font family is Georgia.</p>
    </body>
</html>
```

Output:

[Click here!](./Fonts/Example_9.html)