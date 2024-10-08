# Block and inline elements

## The `<div>` element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p style="border: 1px solid black">Hello World</p>
        <div style="border: 1px solid black">Hello World</div>
        <p>The P and the DIV elements are both block elements, and they will always start on a new line and take up the full width available (stretches out to the left and right as far as it can).</p>
    </body>
</html>
```

Output:

[Click here!](./Block_and_inline_elements/Example_1.html)

## The `<span>` element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p>This is an inline span <span style="border: 1px solid black">Hello World</span> element inside a paragraph.</p>
        <p>The SPAN element is an inline element, and will not start on a new line and only takes up as much width as necessary.</p>
    </body>
</html>
```

Output:

[Click here!](./Block_and_inline_elements/Example_2.html)

## Styling a `<div>` element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <div style="background-color:black;color:white;padding:20px;">
            <h2>London</h2>
            <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
            <p>Standing on the River Thames, London has been a major settlement for two millennia, its history going back to its founding by the Romans, who named it Londinium.</p>
        </div> 
    </body>
</html>
```

Output:

[Click here!](./Block_and_inline_elements/Example_3.html)

## Styling a `<span>` element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The span element</h1>
        <p>My mother has <span style="color:blue;font-weight:bold;">blue</span> eyes and my father has <span style="color:darkolivegreen;font-weight:bold;">dark green</span> eyes.</p>
    </body>
</html>
```

Output:

[Click here!](./Block_and_inline_elements/Example_4.html)