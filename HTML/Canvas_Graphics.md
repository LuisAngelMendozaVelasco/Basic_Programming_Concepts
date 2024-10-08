# Canvas Graphics

## - Draw on the canvas with JavaScript -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <canvas id="myCanvas" width="200" height="100" style="border:1px solid #c3c3c3;">
            Your browser does not support the HTML canvas tag.
        </canvas>

        <script>
            var c = document.getElementById("myCanvas");
            var ctx = c.getContext("2d");
            ctx.fillStyle = "#FF0000";
            ctx.fillRect(0, 0, 150, 75);
        </script>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas1" width="200" height="100" style="border:1px solid #c3c3c3;">
    Your browser does not support the HTML canvas tag.
</canvas>

<script>
    var c = document.getElementById("myCanvas1");
    var ctx = c.getContext("2d");
    ctx.fillStyle = "#FF0000";
    ctx.fillRect(0, 0, 150, 75);
</script>
</body>
</html>

## - Draw a line with lineTo() -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <canvas id="myCanvas" width="200" height="100" style="border:1px solid #d3d3d3;">
            Your browser does not support the HTML canvas tag.
        </canvas>

        <script>
            var c = document.getElementById("myCanvas");
            var ctx = c.getContext("2d");
            ctx.moveTo(0, 0);
            ctx.lineTo(200, 100);
            ctx.stroke();
        </script>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas2" width="200" height="100" style="border:1px solid #d3d3d3;">
    Your browser does not support the HTML canvas tag.
</canvas>

<script>
    var c = document.getElementById("myCanvas2");
    var ctx = c.getContext("2d");
    ctx.moveTo(0, 0);
    ctx.lineTo(200, 100);
    ctx.stroke();
</script>
</body>
</html>

## - Draw a circle with arc() -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <canvas id="myCanvas" width="200" height="100" style="border:1px solid #d3d3d3;">
            Your browser does not support the HTML canvas tag.
        </canvas>

        <script>
            var c = document.getElementById("myCanvas");
            var ctx = c.getContext("2d");
            ctx.beginPath();
            ctx.arc(95, 50, 40, 0, 2*Math.PI);
            ctx.stroke();
        </script> 
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas3" width="200" height="100" style="border:1px solid #d3d3d3;">
    Your browser does not support the HTML canvas tag.
</canvas>

<script>
    var c = document.getElementById("myCanvas3");
    var ctx = c.getContext("2d");
    ctx.beginPath();
    ctx.arc(95, 50, 40, 0, 2*Math.PI);
    ctx.stroke();
</script> 
</body>
</html>

## - Draw a text with fillText() -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <canvas id="myCanvas" width="200" height="100" style="border:1px solid #d3d3d3;">
            Your browser does not support the HTML canvas tag.
        </canvas>

        <script>
            var c = document.getElementById("myCanvas");
            var ctx = c.getContext("2d");
            ctx.font = "30px Arial";
            ctx.fillText("Hello World", 10, 50);
        </script>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas4" width="200" height="100" style="border:1px solid #d3d3d3;">
    Your browser does not support the HTML canvas tag.
</canvas>

<script>
    var c = document.getElementById("myCanvas4");
    var ctx = c.getContext("2d");
    ctx.font = "30px Arial";
    ctx.fillText("Hello World", 10, 50);
</script>
</body>
</html>

## - Draw a text with strokeText() -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <canvas id="myCanvas" width="200" height="100" style="border:1px solid #d3d3d3;">
            Your browser does not support the HTML canvas tag.
        </canvas>

        <script>
            var c = document.getElementById("myCanvas");
            var ctx = c.getContext("2d");
            ctx.font = "30px Arial";
            ctx.strokeText("Hello World", 10, 50);
        </script>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas5" width="200" height="100" style="border:1px solid #d3d3d3;">
    Your browser does not support the HTML canvas tag.
</canvas>

<script>
    var c = document.getElementById("myCanvas5");
    var ctx = c.getContext("2d");
    ctx.font = "30px Arial";
    ctx.strokeText("Hello World", 10, 50);
</script>
</body>
</html>

## - Draw a linear gradient -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <canvas id="myCanvas" width="200" height="100" style="border:1px solid #d3d3d3;">
            Your browser does not support the HTML canvas tag.
        </canvas>

        <script>
            var c = document.getElementById("myCanvas");
            var ctx = c.getContext("2d");
            // Create gradient
            var grd = ctx.createLinearGradient(0, 0, 200, 0);
            grd.addColorStop(0, "red");
            grd.addColorStop(1, "white");
            // Fill with gradient
            ctx.fillStyle = grd;
            ctx.fillRect(10, 10, 150, 80);
        </script>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas6" width="200" height="100" style="border:1px solid #d3d3d3;">
    Your browser does not support the HTML canvas tag.
</canvas>

<script>
    var c = document.getElementById("myCanvas6");
    var ctx = c.getContext("2d");
    // Create gradient
    var grd = ctx.createLinearGradient(0, 0, 200, 0);
    grd.addColorStop(0, "red");
    grd.addColorStop(1, "white");
    // Fill with gradient
    ctx.fillStyle = grd;
    ctx.fillRect(10, 10, 150, 80);
</script>
</body>
</html>

## - Draw a circular gradient -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <canvas id="myCanvas" width="200" height="100" style="border:1px solid #d3d3d3;">
            Your browser does not support the HTML canvas tag.
        </canvas>

        <script>
            var c = document.getElementById("myCanvas");
            var ctx = c.getContext("2d");

            // Create gradient
            var grd = ctx.createRadialGradient(75, 50, 5, 90, 60, 100);
            grd.addColorStop(0, "red");
            grd.addColorStop(1, "white");

            // Fill with gradient
            ctx.fillStyle = grd;
            ctx.fillRect(10, 10, 150, 80);
        </script>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas7" width="200" height="100" style="border:1px solid #d3d3d3;">
    Your browser does not support the HTML canvas tag.
</canvas>

<script>
    var c = document.getElementById("myCanvas7");
    var ctx = c.getContext("2d");

    // Create gradient
    var grd = ctx.createRadialGradient(75, 50, 5, 90, 60, 100);
    grd.addColorStop(0, "red");
    grd.addColorStop(1, "white");

    // Fill with gradient
    ctx.fillStyle = grd;
    ctx.fillRect(10, 10, 150, 80);
</script>
</body>
</html>

## - Draw an image with drawImage() -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Image to use:</p>
        <img id="scream" src="../data/images/img_the_scream.jpg" alt="The Scream" width="220" height="277">

        <p>Canvas to fill:</p>
        <canvas id="myCanvas" width="250" height="300"
            style="border:1px solid #d3d3d3;">
            Your browser does not support the HTML canvas tag.
        </canvas>

        <p><button onclick="myCanvas()">Try it</button></p>

        <script>
            function myCanvas() {
                var c = document.getElementById("myCanvas");
                var ctx = c.getContext("2d");
                var img = document.getElementById("scream");
                ctx.drawImage(img, 10, 10);
            }
        </script>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
<body>
<p>Image to use:</p>
<img id="scream" src="./images/img_the_scream.jpg" alt="The Scream" width="220" height="277">

<p>Canvas to fill:</p>
<canvas id="myCanvas8" width="250" height="300"
    style="border:1px solid #d3d3d3;">
    Your browser does not support the HTML canvas tag.
</canvas>

<p><button onclick="myCanvas()">Try it</button></p>

<script>
    function myCanvas() {
        var c = document.getElementById("myCanvas8");
        var ctx = c.getContext("2d");
        var img = document.getElementById("scream");
        ctx.drawImage(img, 10, 10);
    }
</script>
</body>
</html>