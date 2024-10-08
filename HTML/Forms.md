# Forms

## - Form with text input -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Text input fields</h2>

        <form>
            <label for="fname">First name:</label><br>
            <input type="text" id="fname" name="fname" value="John"><br>
            <label for="lname">Last name:</label><br>
            <input type="text" id="lname" name="lname" value="Doe">
        </form>

        <p>Note that the form itself is not visible.</p>

        <p>Also note that the default width of text input fields is 20 characters.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h2>Text input fields</h2>

<form>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe">
</form>

<p>Note that the form itself is not visible.</p>

<p>Also note that the default width of text input fields is 20 characters.</p>
    </body>
</html>

## - Form with radio button input -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Radio Buttons</h2>

        <p>Choose your favorite Web language:</p>

        <form>
            <input type="radio" id="html" name="fav_language" value="HTML">
            <label for="html">HTML</label><br>
            <input type="radio" id="css" name="fav_language" value="CSS">
            <label for="css">CSS</label><br>
            <input type="radio" id="javascript" name="fav_language" value="JavaScript">
            <label for="javascript">JavaScript</label>
        </form> 
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h2>Radio Buttons</h2>

<p>Choose your favorite Web language:</p>

<form>
    <input type="radio" id="html" name="fav_language" value="HTML">
    <label for="html">HTML</label><br>
    <input type="radio" id="css" name="fav_language" value="CSS">
    <label for="css">CSS</label><br>
    <input type="radio" id="javascript" name="fav_language" value="JavaScript">
    <label for="javascript">JavaScript</label>
</form> 
    </body>
</html>

## - Form with text fields and a submit button -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>HTML Forms</h2>

        <form action="./action_page.php">
            <label for="fname">First name:</label><br>
            <input type="text" id="fname" name="fname" value="John"><br>
            <label for="lname">Last name:</label><br>
            <input type="text" id="lname" name="lname" value="Doe"><br><br>
            <input type="submit" value="Submit">
        </form> 

        <p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h2>HTML Forms</h2>

<form action="./action_page.php">
<label for="fname">First name:</label><br>
<input type="text" id="fname" name="fname" value="John"><br>
<label for="lname">Last name:</label><br>
<input type="text" id="lname" name="lname" value="Doe"><br><br>
<input type="submit" value="Submit">
</form> 

<p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>
    </body>
</html>

## - Form with a text fields without a name attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>The name Attribute</h2>

        <form action="./action_page.php">
            <label for="fname">First name:</label><br>
            <input type="text" id="fname" value="John"><br><br>
            <input type="submit" value="Submit">
        </form> 

        <p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>

        <p>Notice that the value of the "First name" field will not be submitted, because the input element does not have a name attribute.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h2>The name Attribute</h2>

<form action="./action_page.php">
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" value="John"><br><br>
    <input type="submit" value="Submit">
</form> 

<p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>

<p>Notice that the value of the "First name" field will not be submitted, because the input element does not have a name attribute.</p>
    </body>
</html>

## - Grouping Form Data -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Grouping Form Data with Fieldset</h2>

        <p>The fieldset element is used to group related data in a form, and the legend element defines a caption for the fieldset element.</p>

        <form action="/action_page.php">
            <fieldset>
                <legend>Personalia:</legend>
                <label for="fname">First name:</label><br>
                <input type="text" id="fname" name="fname" value="John"><br>
                <label for="lname">Last name:</label><br>
                <input type="text" id="lname" name="lname" value="Doe"><br><br>
                <input type="submit" value="Submit">
            </fieldset>
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h2>Grouping Form Data with Fieldset</h2>

<p>The fieldset element is used to group related data in a form, and the legend element defines a caption for the fieldset element.</p>

<form action="/action_page.php">
    <fieldset>
        <legend>Personalia:</legend>
        <label for="fname">First name:</label><br>
        <input type="text" id="fname" name="fname" value="John"><br>
        <label for="lname">Last name:</label><br>
        <input type="text" id="lname" name="lname" value="Doe"><br><br>
        <input type="submit" value="Submit">
    </fieldset>
</form>
    </body>
</html>