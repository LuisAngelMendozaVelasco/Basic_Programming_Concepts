# Text Effects

## Specify how hidden, overflowed content should be signaled to the user

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            p.test1 {   white-space: nowrap; 
                        width: 200px; 
                        border: 1px solid #000000;
                        overflow: hidden;
                        text-overflow: clip;}

            p.test2 {   white-space: nowrap; 
                        width: 200px; 
                        border: 1px solid #000000;
                        overflow: hidden;
                        text-overflow: ellipsis;}
        </style>
    </head>
    <body>
        <h1>The text-overflow Property</h1>
        <p>The following two paragraphs contains a long text that will not fit in the box.</p>

        <h2>text-overflow: clip:</h2>
        <p class="test1">This is some long text that will not fit in the box</p>

        <h2>text-overflow: ellipsis:</h2>
        <p class="test2">This is some long text that will not fit in the box</p>
    </body>
</html>
```

Output:

[Click here!](./Text_Effects/Example_1.html)

## How to display the overflowed content when hover over the element

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            div.test {  white-space: nowrap; 
                        width: 200px; 
                        overflow: hidden; 
                        border: 1px solid #000000;}

            div.test:hover {overflow: visible;}
        </style>
    </head>
    <body>
        <p>Hover over the two divs below, to see the entire text.</p>
        <div class="test" style="text-overflow:ellipsis;">This is some long text that will not fit in the box</div>
        <br>
        <div class="test" style="text-overflow:clip;">This is some long text that will not fit in the box</div>
    </body>
</html>
```

Output:

[Click here!](./Text_Effects/Example_2.html)

## Allow long words to be able to be broken and wrap onto the next line

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            p.test {width: 11em; 
                    border: 1px solid #000000;
                    word-wrap: break-word;}
        </style>
    </head>
    <body>
        <h1>The word-wrap Property</h1>

        <p class="test">This paragraph contains a very long word: thisisaveryveryveryveryveryverylongword. The long word will break and wrap to the next line.</p>
    </body>
</html>
```

Output:

[Click here!](./Text_Effects/Example_3.html)

## Specify line breaking rules

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style> 
            p.test1 {   width: 140px; 
                        border: 1px solid #000000;
                        word-break: keep-all;}

            p.test2 {   width: 140px; 
                        border: 1px solid #000000;
                        word-break: break-all;}
        </style>
    </head>
    <body>
        <h1>The word-break Property</h1>

        <p class="test1">This paragraph contains some text. This line will-break-at-hyphens.</p>

        <p class="test2">This paragraph contains some text. The lines will break at any character.</p>
    </body>
</html>
```

Output:

[Click here!](./Text_Effects/Example_4.html)