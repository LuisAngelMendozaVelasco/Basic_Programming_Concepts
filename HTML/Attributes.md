# Attributes

## - The title attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2 title="I'm a header">The title Attribute</h2>
        <p title="I'm a tooltip">Mouse over this paragraph, to display the title attribute as a tooltip.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2 title="I'm a header">The title Attribute</h2>
        <p title="I'm a tooltip">Mouse over this paragraph, to display the title attribute as a tooltip.</p>
    </body>
</html>

## - The href attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The href Attribute</h2>
        <p>HTML links are defined with the a tag. The link address is specified in the href attribute:</p>
        <a href="https://www.w3schools.com">Visit W3Schools</a>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>The href Attribute</h2>
        <p>HTML links are defined with the a tag. The link address is specified in the href attribute:</p>
        <a href="https://www.w3schools.com">Visit W3Schools</a>
    </body>
</html>

## - The width and height attributes -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Width and Height Attributes</h2>
        <p>The width and height attributes of the img tag, defines the width and height of the image:</p>
        <img src="./images/img_girl.jpg" width="500" height="600">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>Width and Height Attributes</h2>
        <p>The width and height attributes of the img tag, defines the width and height of the image:</p>
        <img src="./images/img_girl.jpg" width="500" height="600">
    </body>
</html>

## - The alt attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The alt Attribute</h2>
        <p>The alt attribute should reflect the image content, so users who cannot see the image get an understanding of what the image contains:</p>
        <img src="./images/img_girl.jpg" alt="Girl with a jacket" width="500" height="600">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <h2>The alt Attribute</h2>
        <p>The alt attribute should reflect the image content, so users who cannot see the image get an understanding of what the image contains:</p>
        <img src="./images/img_girl.jpg" alt="Girl with a jacket" width="500" height="600">
    </body>
</html>

## - Attribute without quotes -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <a href=https://www.w3schools.com>This is a link</a>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <a href=https://www.w3schools.com>This is a link</a>
    </body>
</html>

## - Attribute without quotes does not work -

Code:

```html
<html>
    <body>
        <h1>About W3Schools</h1>
        <p title=About W3Schools>
            You cannot omit quotes around an attribute value 
            if the value contains spaces.
        </p>
        <p><b>
            If you move the mouse over the paragraph above,
            your browser will only display the first word from the title.
        </b></p>
    </body>
</html>
```

Output:

<html>
    <body>
        <h1>About W3Schools</h1>
        <p title=About W3Schools>
            You cannot omit quotes around an attribute value 
            if the value contains spaces.
        </p>
        <p><b>
            If you move the mouse over the paragraph above,
            your browser will only display the first word from the title.
        </b></p>
    </body>
</html>