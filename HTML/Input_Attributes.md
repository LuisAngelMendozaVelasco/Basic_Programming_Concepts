# Input Attributes

## - The autocomplete attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The autocomplete attribute</h1>

        <p>The autocomplete attribute specifies whether or not an input field should have autocomplete enabled.</p>

        <p>Fill in and submit the form, then reload the page to see how autocomplete works.</p>

        <p>Notice that autocomplete is "on" for the form, but "off" for the e-mail field!</p>

        <form action="/action_page.php" autocomplete="on">
            <label for="fname">First name:</label>
            <input type="text" id="fname" name="fname"><br><br>
            <label for="lname">Last name:</label>
            <input type="text" id="lname" name="lname"><br><br>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" autocomplete="off"><br><br>
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The autocomplete attribute</h1>

<p>The autocomplete attribute specifies whether or not an input field should have autocomplete enabled.</p>

<p>Fill in and submit the form, then reload the page to see how autocomplete works.</p>

<p>Notice that autocomplete is "on" for the form, but "off" for the e-mail field!</p>

<form action="/action_page.php" autocomplete="on">
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <label for="lname">Last name:</label>
    <input type="text" id="lname" name="lname"><br><br>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" autocomplete="off"><br><br>
    <input type="submit" value="Submit">
</form>
    </body>
</html>

## - The novalidate attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The form novalidate attribute</h1>

        <p>The novalidate attribute specifies that the form data should not be validated when submitted.</p>

        <form action="/action_page.php" novalidate>
            <label for="email">Enter your email:</label>
            <input type="email" id="email" name="email" required><br><br>
            <input type="submit" value="Submit">
        </form>

        <p><strong>Note:</strong> The novalidate attribute of the form tag is not supported in Safari 10 (or earlier).</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The form novalidate attribute</h1>

<p>The novalidate attribute specifies that the form data should not be validated when submitted.</p>

<form action="/action_page.php" novalidate>
    <label for="email">Enter your email:</label>
    <input type="email" id="email" name="email" required><br><br>
    <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> The novalidate attribute of the form tag is not supported in Safari 10 (or earlier).</p>
    </body>
</html>

## - The autofocus_attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input autofocus attribute</h1>

        <p>The autofocus attribute specifies that the input field should automatically get focus when the page loads.</p>

        <form action="/action_page.php">
            <label for="fname">First name:</label><br>
            <input type="text" id="fname" name="fname" autofocus><br>
            <label for="lname">Last name:</label><br>
            <input type="text" id="lname" name="lname"><br><br>
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input autofocus attribute</h1>

<p>The autofocus attribute specifies that the input field should automatically get focus when the page loads.</p>

<form action="/action_page.php">
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" autofocus><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname"><br><br>
    <input type="submit" value="Submit">
</form>
    </body>
</html>

## - The form attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input form attribute</h1>

        <p>The form attribute specifies the form an input element belongs to.</p>

        <form action="/action_page.php" id="form1">
            <label for="fname">First name:</label>
            <input type="text" id="fname" name="fname"><br><br>
            <input type="submit" value="Submit">
        </form>

        <p>The "Last name" field below is outside the form element, but still part of the form.</p>

        <label for="lname">Last name:</label>
        <input type="text" id="lname" name="lname" form="form1">
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input form attribute</h1>

<p>The form attribute specifies the form an input element belongs to.</p>

<form action="/action_page.php" id="form1">
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <input type="submit" value="Submit">
</form>

<p>The "Last name" field below is outside the form element, but still part of the form.</p>

<label for="lname">Last name:</label>
<input type="text" id="lname" name="lname" form="form1">
    </body>
</html>

## - The formaction attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input formaction attribute</h1>

        <p>The formaction attribute specifies the URL of a file that will process the input when the form is submitted.</p>

        <form action="/action_page.php">
            <label for="fname">First name:</label>
            <input type="text" id="fname" name="fname"><br><br>
            <label for="lname">Last name:</label>
            <input type="text" id="lname" name="lname"><br><br>
            <input type="submit" value="Submit">
            <input type="submit" formaction="/action_page2.php" value="Submit as Admin">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input formaction attribute</h1>

<p>The formaction attribute specifies the URL of a file that will process the input when the form is submitted.</p>

<form action="/action_page.php">
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <label for="lname">Last name:</label>
    <input type="text" id="lname" name="lname"><br><br>
    <input type="submit" value="Submit">
    <input type="submit" formaction="/action_page2.php" value="Submit as Admin">
</form>
    </body>
</html>

## - The formenctype attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input formenctype attribute</h1>

        <p>The formenctype attribute specifies how the form data should be encoded when submitted.</p>

        <form action="/action_page_binary.asp" method="post">
            <label for="fname">First name:</label>
            <input type="text" id="fname" name="fname"><br><br>
            <input type="submit" value="Submit">
            <input type="submit" formenctype="multipart/form-data" value="Submit as Multipart/form-data">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input formenctype attribute</h1>

<p>The formenctype attribute specifies how the form data should be encoded when submitted.</p>

<form action="/action_page_binary.asp" method="post">
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <input type="submit" value="Submit">
    <input type="submit" formenctype="multipart/form-data" value="Submit as Multipart/form-data">
</form>
    </body>
</html>

## - The formmethod attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input formmethod Attribute</h1>

        <p>The formmethod attribute defines the HTTP method for sending form-data to the action URL.</p>

        <form action="/action_page.php" method="get" target="_blank">
            <label for="fname">First name:</label>
            <input type="text" id="fname" name="fname"><br><br>
            <label for="lname">Last name:</label>
            <input type="text" id="lname" name="lname"><br><br>
            <input type="submit" value="Submit using GET">
            <input type="submit" formmethod="post" value="Submit using POST">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input formmethod Attribute</h1>

<p>The formmethod attribute defines the HTTP method for sending form-data to the action URL.</p>

<form action="/action_page.php" method="get" target="_blank">
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <label for="lname">Last name:</label>
    <input type="text" id="lname" name="lname"><br><br>
    <input type="submit" value="Submit using GET">
    <input type="submit" formmethod="post" value="Submit using POST">
</form>
    </body>
</html>

## - The formnovalidate attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input formnovalidate attribute</h1>

        <form action="/action_page.php">
            <label for="email">Enter your email:</label>
            <input type="email" id="email" name="email" required><br><br>
            <input type="submit" value="Submit">
            <input type="submit" formnovalidate="formnovalidate" value="Submit without validation">
        </form>

        <p><strong>Note:</strong> The formnovalidate attribute of the input tag is not supported in Safari 10 (or earlier).</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input formnovalidate attribute</h1>

<form action="/action_page.php">
    <label for="email">Enter your email:</label>
    <input type="email" id="email" name="email" required><br><br>
    <input type="submit" value="Submit">
    <input type="submit" formnovalidate="formnovalidate" value="Submit without validation">
</form>

<p><strong>Note:</strong> The formnovalidate attribute of the input tag is not supported in Safari 10 (or earlier).</p>
    </body>
</html>

## - The formtarget attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input formtarget attribute</h1>

        <p>The formtarget attribute specifies a name or a keyword that indicates where to display the response that is received after submitting the form.</p>

        <form action="/action_page.php">
            <label for="fname">First name:</label>
            <input type="text" id="fname" name="fname"><br><br>
            <label for="lname">Last name:</label>
            <input type="text" id="lname" name="lname"><br><br>
            <input type="submit" value="Submit">
            <input type="submit" formtarget="_blank" value="Submit to a new window/tab">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input formtarget attribute</h1>

<p>The formtarget attribute specifies a name or a keyword that indicates where to display the response that is received after submitting the form.</p>

<form action="/action_page.php">
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <label for="lname">Last name:</label>
    <input type="text" id="lname" name="lname"><br><br>
    <input type="submit" value="Submit">
    <input type="submit" formtarget="_blank" value="Submit to a new window/tab">
</form>
    </body>
</html>

## - The height and width attributes -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input height and width attributes</h1>

        <p>The height and width attributes specify the height and width of an input type="image" element.</p>

        <form action="/action_page.php">
            <label for="fname">First name:</label>
            <input type="text" id="fname" name="fname"><br><br>
            <label for="lname">Last name:</label>
            <input type="text" id="lname" name="lname"><br><br>
            <input type="image" src="../data/images/img_submit.gif" alt="Submit" width="48" height="48">
        </form>

        <p><b>Note:</b> The input type="image" sends the X and Y coordinates of the click that activated the image button.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input height and width attributes</h1>

<p>The height and width attributes specify the height and width of an input type="image" element.</p>

<form action="/action_page.php">
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <label for="lname">Last name:</label>
    <input type="text" id="lname" name="lname"><br><br>
    <input type="image" src="./images/img_submit.gif" alt="Submit" width="48" height="48">
</form>

<p><b>Note:</b> The input type="image" sends the X and Y coordinates of the click that activated the image button.</p>
    </body>
</html>

## - The list attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <form action="/action_page.php">
            Webpage: <input type="url" list="url_list" name="link">
            <datalist id="url_list">
                <option label="W3Schools" value="https://www.w3schools.com">
                <option label="Google" value="http://www.google.com">
                <option label="Microsoft" value="http://www.microsoft.com">
            </datalist>
            <input type="submit">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <form action="/action_page.php">
            Webpage: <input type="url" list="url_list" name="link">
            <datalist id="url_list">
                <option label="W3Schools" value="https://www.w3schools.com">
                <option label="Google" value="http://www.google.com">
                <option label="Microsoft" value="http://www.microsoft.com">
            </datalist>
            <input type="submit">
        </form>
    </body>
</html>

## - The min and max attributes -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input min and max attributes</h1>

        <p>The min and max attributes specify the minimum and maximum values for an input element.</p>

        <form action="/action_page.php">
            <label for="datemax">Enter a date before 1980-01-01:</label>
            <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

            <label for="datemin">Enter a date after 2000-01-01:</label>
            <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>
            
            <label for="quantity">Quantity (between 1 and 5):</label>
            <input type="number" id="quantity" name="quantity" min="1" max="5"><br><br>

            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input min and max attributes</h1>

<p>The min and max attributes specify the minimum and maximum values for an input element.</p>

<form action="/action_page.php">
<label for="datemax">Enter a date before 1980-01-01:</label>
<input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

<label for="datemin">Enter a date after 2000-01-01:</label>
<input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>

<label for="quantity">Quantity (between 1 and 5):</label>
<input type="number" id="quantity" name="quantity" min="1" max="5"><br><br>

<input type="submit" value="Submit">
</form>
    </body>
</html>

## - The multiple attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input multiple attributes</h1>

        <p>The multiple attribute specifies that the user is allowed to enter more than one value in an input field.</p>

        <form action="/action_page.php">
            <label for="files">Select files:</label>
            <input type="file" id="files" name="files" multiple><br><br>
            <input type="submit" value="Submit">
        </form>

        <p>To select multiple files, hold down the CTRL or SHIFT key while selecting.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input multiple attributes</h1>

<p>The multiple attribute specifies that the user is allowed to enter more than one value in an input field.</p>

<form action="/action_page.php">
    <label for="files">Select files:</label>
    <input type="file" id="files" name="files" multiple><br><br>
    <input type="submit" value="Submit">
</form>

<p>To select multiple files, hold down the CTRL or SHIFT key while selecting.</p>
    </body>
</html>

## - The pattern attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input pattern attribute</h1>

        <p>The pattern attribute specifies a regular expression that the input element's value is checked against.</p>

        <form action="/action_page.php">
            <label for="country_code">Country code:</label>
            <input type="text" id="country_code" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code"><br><br>
            <input type="submit" value="Submit">
        </form>

        <p><strong>Note:</strong> The pattern attribute of the input tag is not supported in Safari 10 (or earlier).</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input pattern attribute</h1>

<p>The pattern attribute specifies a regular expression that the input element's value is checked against.</p>

<form action="/action_page.php">
    <label for="country_code">Country code:</label>
    <input type="text" id="country_code" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code"><br><br>
    <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> The pattern attribute of the input tag is not supported in Safari 10 (or earlier).</p>
    </body>
</html>

## - The placeholder attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input placeholder attribute</h1>

        <p>The placeholder attribute specifies a short hint that describes the expected value of an input field.</p>

        <form action="/action_page.php">
            <label for="phone">Enter a phone number:</label>
            <input type="tel" id="phone" name="phone" placeholder="123-45-678" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}"><br><br>
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input placeholder attribute</h1>

<p>The placeholder attribute specifies a short hint that describes the expected value of an input field.</p>

<form action="/action_page.php">
    <label for="phone">Enter a phone number:</label>
    <input type="tel" id="phone" name="phone" placeholder="123-45-678" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}"><br><br>
    <input type="submit" value="Submit">
</form>
    </body>
</html>

## - The required attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input required attribute</h1>

        <p>The required attribute specifies that an input field must be filled out before submitting the form.</p>

        <form action="/action_page.php">
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" required>
            <input type="submit" value="Submit">
        </form>

        <p><strong>Note:</strong> The required attribute of the input tag is not supported in Safari prior version 10.1.</p>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input required attribute</h1>

<p>The required attribute specifies that an input field must be filled out before submitting the form.</p>

<form action="/action_page.php">
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" required>
    <input type="submit" value="Submit">
</form>

<p><strong>Note:</strong> The required attribute of the input tag is not supported in Safari prior version 10.1.</p>
    </body>
</html>

## - The step attribute -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>The input step attribute</h1>

        <p>The step attribute specifies the legal number intervals for an input element.</p>

        <form action="/action_page.php">
            <label for="points">Points:</label>
            <input type="number" id="points" name="points" step="3">
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
<h1>The input step attribute</h1>

<p>The step attribute specifies the legal number intervals for an input element.</p>

<form action="/action_page.php">
    <label for="points">Points:</label>
    <input type="number" id="points" name="points" step="3">
    <input type="submit" value="Submit">
</form>
    </body>
</html>