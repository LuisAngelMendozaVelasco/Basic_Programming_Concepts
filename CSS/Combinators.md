# Combinators

## Descendant selector

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div p {background-color: yellow;}
        </style>
    </head>
    <body>
        <h2>Descendant Selector</h2>

        <p>The descendant selector matches all elements that are descendants of a specified element.</p>

        <div>
            <p>Paragraph 1 in the div.</p>
            <p>Paragraph 2 in the div.</p>
            <section><p>Paragraph 3 in the div.</p></section>
        </div>

        <p>Paragraph 4. Not in a div.</p>
        <p>Paragraph 5. Not in a div.</p>
    </body>
</html>
```

Output:

[Click here!](./Combinators/Example_1.html)

## Child selector

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div > p {background-color: yellow;}
        </style>
    </head>
    <body>
        <h2>Child Selector</h2>

        <p>The child selector (>) selects all elements that are the children of a specified element.</p>

        <div>
            <p>Paragraph 1 in the div.</p>
            <p>Paragraph 2 in the div.</p>
            <section>
                <!-- not Child but Descendant -->
                <p>Paragraph 3 in the div (inside a section element).</p>
            </section>
            <p>Paragraph 4 in the div.</p>
        </div>

        <p>Paragraph 5. Not in a div.</p>
        <p>Paragraph 6. Not in a div.</p>
    </body>
</html>
```

Output:

[Click here!](./Combinators/Example_2.html)

## Adjacent Sibling selector

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div + p {background-color: yellow;}
        </style>
    </head>
    <body>
        <h2>Adjacent Sibling Selector</h2>

        <p>The + selector is used to select an element that is directly after another specific element.</p>
        <p>The following example selects the first p element that are placed immediately after div elements:</p>

        <div>
            <p>Paragraph 1 in the div.</p>
            <p>Paragraph 2 in the div.</p>
        </div>

        <p>Paragraph 3. After a div.</p>
        <p>Paragraph 4. After a div.</p>

        <div>
            <p>Paragraph 5 in the div.</p>
            <p>Paragraph 6 in the div.</p>
        </div>

        <p>Paragraph 7. After a div.</p>
        <p>Paragraph 8. After a div.</p>
    </body>
</html>
```

Output:

[Click here!](./Combinators/Example_3.html)

## General Sibling selector

Code:

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            div ~ p {background-color: yellow;}
        </style>
    </head>
    <body>
        <h2>General Sibling Selector</h2>

        <p>The general sibling selector (~) selects all elements that are next siblings of a specified element.</p>

        <p>Paragraph 1.</p>

        <div>
            <p>Paragraph 2.</p>
        </div>

        <p>Paragraph 3.</p>
        <code>Some code.</code>
        <p>Paragraph 4.</p>
    </body>
</html>
```

Output:

[Click here!](./Combinators/Example_4.html)