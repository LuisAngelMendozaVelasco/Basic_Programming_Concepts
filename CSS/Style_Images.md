# Style Images

## Rounded image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {border-radius: 8px;}
        </style>
    </head>
    <body>
        <h2>Rounded Image</h2>

        <p>Use the border-radius property to create rounded images:</p>

        <img src="../data/images/paris.jpg" alt="Paris" width="300" height="300">
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_1.html)

## Circled image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {border-radius: 50%;}
        </style>
    </head>
    <body>
        <h2>Circled Image</h2>

        <p>Use the border-radius property to create circled images:</p>

        <img src="../data/images/paris.jpg" alt="Paris" width="300" height="300">
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_2.html)

## Thumbnail image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   border: 1px solid #ddd;
                    border-radius: 4px;
                    padding: 5px;
                    width: 150px;}
        </style>
    </head>
    <body>
        <h2>Thumbnail Image</h2>

        <p>Use the border property to create thumbnail images:</p>

        <img src="../data/images/paris.jpg" alt="Paris" style="width:150px">
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_3.html)

## Thumbnail image as link

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   border: 1px solid #ddd;
                    border-radius: 4px;
                    padding: 5px;
                    width: 150px;}

            img:hover {box-shadow: 0 0 2px 1px rgba(0, 140, 186, 0.5);}
        </style>
    </head>
    <body>
        <h2>Thumbnail Image as Link</h2>

        <p>Use the border property to create thumbnail images. Wrap an anchor around the image to use it as a link.</p>
        <p>Hover over the image and click on it to see the effect.</p>

        <a target="_blank" href="../data/images/paris.jpg">
            <img src="../data/images/paris.jpg" alt="Paris" style="width:150px">
        </a>
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_4.html)

## Responsive image

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   max-width: 100%;
                    height: auto;}
        </style>
    </head>
    <body>
        <h2>Responsive Image</h2>

        <p>Responsive images will automatically adjust to fit the size of the screen.</p>
        <p>Resize the browser window to see the effect:</p>

        <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_5.html)

## Image text (top left corner)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .topleft {  position: absolute;
                        top: 8px;
                        left: 16px;
                        font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>
        <p>Add some text to an image in the top left corner:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="topleft">Top Left</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_6.html)

## Image text (top right corner)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .topright { position: absolute;
                        top: 8px;
                        right: 16px;
                        font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>
        <p>Add some text to an image in the top right corner:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="topright">Top Right</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_7.html)

## Image text (bottom left corner)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .bottomleft {   position: absolute;
                            bottom: 8px;
                            left: 16px;
                            font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>
        <p>Add some text to an image in the bottom left corner:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="bottomleft">Bottom Left</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_8.html)

## Image text (bottom right corner)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .bottomright {  position: absolute;
                            bottom: 8px;
                            right: 16px;
                            font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>
        <p>Add some text to an image in the bottom right corner:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="bottomright">Bottom Right</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_9.html)

## Image text (centered)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            .container {position: relative;}

            .center {   position: absolute;
                        top: 50%;
                        width: 100%;
                        text-align: center;
                        font-size: 18px;}

            img {   width: 100%;
                    height: auto;
                    opacity: 0.3;}
        </style>
    </head>
    <body>
        <h2>Image Text</h2>

        <p>Center text in image:</p>

        <div class="container">
            <img src="../data/images/img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="center">Centered</div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_10.html)

## Polaroid images

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {margin:25px;}

            div.polaroid {  width: 80%;
                            background-color: white;
                            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
                            margin-bottom: 25px;}

            div.container { text-align: center;
                            padding: 10px 20px;}
        </style>
    </head>
    <body>
        <h2>Responsive Polaroid Images / Cards</h2>

        <div class="polaroid">
            <img src="../data/images/img_5terre.jpg" alt="5 Terre" style="width:100%">
            <div class="container">
                <p>Cinque Terre</p>
            </div>
        </div>

        <div class="polaroid">
            <img src="../data/images/lights600x400.jpg" alt="Norther Lights" style="width:100%">
            <div class="container">
                <p>Northern Lights</p>
            </div>
        </div>
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_11.html)

## Grayscale image filter

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            img {   -webkit-filter: grayscale(100%); /* Chrome, Safari, Opera */
                    filter: grayscale(100%);}
        </style>
    </head>
    <body>
        <p>Convert the image to grayscale:</p>

        <img src="../data/images/pineapple.jpg" alt="Pineapple" width="300" height="300">

        <p><strong>Note:</strong> The filter property is not supported in Internet Explorer.</p>
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_12.html)

## Advanced - Image Modal with CSS and JavaScript

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #myImg {border-radius: 5px;
                    cursor: pointer;
                    transition: 0.3s;}

            #myImg:hover {opacity: 0.7;}

            /* The Modal (background) */
            .modal {display: none; /* Hidden by default */
                    position: fixed; /* Stay in place */
                    z-index: 1; /* Sit on top */
                    padding-top: 100px; /* Location of the box */
                    left: 0;
                    top: 0;
                    width: 100%; /* Full width */
                    height: 100%; /* Full height */
                    overflow: auto; /* Enable scroll if needed */
                    background-color: rgb(0,0,0); /* Fallback color */
                    background-color: rgba(0,0,0,0.9);} /* Black w/ opacity */
            
            /* Modal Content (image) */
            .modal-content {margin: auto;
                            display: block;
                            width: 80%;
                            max-width: 700px;}

            /* Caption of Modal Image */
            #caption {  margin: auto;
                        display: block;
                        width: 80%;
                        max-width: 700px;
                        text-align: center;
                        color: #ccc;
                        padding: 10px 0;
                        height: 150px;}

            /* Add Animation */
            .modal-content, #caption {  animation-name: zoom;
                                        animation-duration: 0.6s;}

            @keyframes zoom {   from {transform: scale(0.1)} 
                                to {transform: scale(1)}}

            /* The Close Button */
            .close {position: absolute;
                    top: 15px;
                    right: 35px;
                    color: #f1f1f1;
                    font-size: 40px;
                    font-weight: bold;
                    transition: 0.3s;}

            .close:hover, .close:focus {color: #bbb;
                                        text-decoration: none;
                                        cursor: pointer;}

            /* 100% Image Width on Smaller Screens */
            @media only screen and (max-width: 700px){.modal-content {width: 100%;}}
        </style>
    </head>
    <body>
        <h2>Image Modal</h2>

        <p>Here, we use CSS to create a modal (dialog box) that is hidden by default.</p>
        <p>We use JavaScript to trigger the modal and to display the current image inside the modal when it is clicked on. Also note that we use the value from the image's "alt" attribute as an image caption text inside the modal.</p>
        <p>Don't worry if you do not understand the code right away. When you are done with CSS, go to our JavaScript Tutorial to learn more.</p>

        <img id="myImg" src="../data/images/img_lights.jpg" alt="Northern Lights, Norway" width="300" height="200">

        <!-- The Modal -->
        <div id="myModal" class="modal">
            <span class="close">&times;</span>
            <img class="modal-content" id="img01">
            <div id="caption"></div>
        </div>

        <script>
            // Get the modal
            var modal = document.getElementById('myModal');

            // Get the image and insert it inside the modal - use its "alt" text as a caption
            var img = document.getElementById('myImg');
            var modalImg = document.getElementById("img01");
            var captionText = document.getElementById("caption");
            img.onclick = function(){
                modal.style.display = "block";
                modalImg.src = this.src;
                captionText.innerHTML = this.alt;
            }

            // Get the <span> element that closes the modal
            var span = document.getElementsByClassName("close")[0];

            // When the user clicks on <span> (x), close the modal
            span.onclick = function() { 
                modal.style.display = "none";
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./Style_Images/Example_13.html)