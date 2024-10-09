# Form Elements

## A simple drop-down list

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The select Element</h2>

        <p>The select element defines a drop-down list:</p>

        <form action="/action_page.php">
            <label for="cars">Choose a car:</label>
            <select id="cars" name="cars">
                <option value="volvo">Volvo</option>
                <option value="saab">Saab</option>
                <option value="fiat">Fiat</option>
                <option value="audi">Audi</option>
            </select>
            <input type="submit">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Form_Elements/Example_1.html)

## A drop-down list with a pre-selected value

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Pre-selected Option</h2>

        <p>You can preselect an option with the selected attribute:</p>

        <form action="/action_page.php">
            <label for="cars">Choose a car:</label>
            <select id="cars" name="cars">
                <option value="volvo">Volvo</option>
                <option value="saab">Saab</option>
                <option value="fiat" selected>Fiat</option>
                <option value="audi">Audi</option>
            </select>
            <input type="submit">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Form_Elements/Example_2.html)

## A textarea (a multi-line text input field)

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Textarea</h2>
        <p>The textarea element defines a multi-line input field.</p>

        <form action="/action_page.php">
            <textarea name="message" rows="10" cols="30">The cat was playing in the garden.</textarea>
            <br>
            <input type="submit">
        </form>
    </body>
</html>
```

Output:

[Click here!](./Form_Elements/Example_3.html)

## An input button

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The button Element</h2>

        <button type="button" onclick="alert('Hello World!')">Click Me!</button>
    </body>
</html>
```

Output:

[Click here!](./Form_Elements/Example_4.html)

## Using the `<datalist>` Element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The datalist Element</h2>

        <p>The datalist element specifies a list of pre-defined options for an input element.</p>

        <form action="/action_page.php">
            <input list="browsers" name="browser">
            <datalist id="browsers">
                <option value="Internet Explorer">
                <option value="Firefox">
                <option value="Chrome">
                <option value="Opera">
                <option value="Safari">
            </datalist>
            <input type="submit">
        </form>

        <p><b>Note:</b> The datalist tag is not supported in Safari prior version 12.1.</p>
    </body>
</html>
```

Output:

[Click here!](./Form_Elements/Example_5.html)

## Using the `<output>` Element

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The output Element</h2>
        <p>The output element represents the result of a calculation.</p>

        <form action="/action_page.php"
            oninput="x.value=parseInt(a.value)+parseInt(b.value)">
                0
                <input type="range" id="a" name="a" value="50">
                100 +
                <input type="number" id="b" name="b" value="50">
                =
                <output name="x" for="a b"></output>
                <br><br>
                <input type="submit">
        </form>

        <p><strong>Note:</strong> The output element is not supported in Edge prior version 13.</p>
    </body>
</html>
```

Output:

[Click here!](./Form_Elements/Example_6.html)