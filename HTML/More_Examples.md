# More Examples

## HTML drag and drop

Code:

```html
<!DOCTYPE HTML>
<html>
    <head>
        <style>
            #div1 { width: 350px;
                    height: 70px;
                    padding: 10px;
                    border: 1px solid #aaaaaa;}
        </style>
        <script>
            function allowDrop(ev) {
                ev.preventDefault();
            }

            function drag(ev) {
                ev.dataTransfer.setData("text", ev.target.id);
            }

            function drop(ev) {
                ev.preventDefault();
                var data = ev.dataTransfer.getData("text");
                ev.target.appendChild(document.getElementById(data));
            }
        </script>
    </head>
    <body>
        <p>Drag the W3Schools image into the rectangle:</p>

        <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
        <br>
        <img id="drag1" src="../data/images/img_logo.gif" draggable="true" ondragstart="drag(event)" width="336" height="69">
    </body>
</html>
```

Output:

[Click here!](./More_Examples/Example_1.html)

## HTML web workers

Code:

```js
var i = 0;

function timedCount()
{
    i = i+1;
    postMessage(i);                   //posts a message back to the HTML page.
    setTimeout("timedCount()", 500);
}

timedCount();
```

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Count numbers: <output id="result"></output></p>
        <button onclick="startWorker()">Start Worker</button> 
        <button onclick="stopWorker()">Stop Worker</button>

        <p><strong>Note:</strong> Internet Explorer 9 and earlier versions do not support Web Workers.</p>

        <script>
            var w;

            function startWorker() {
                if(typeof(Worker) !== "undefined") {
                    if(typeof(w) == "undefined") {
                        w = new Worker("./demo_workers.js");
                    }
                    w.onmessage = function(event) {
                        document.getElementById("result").innerHTML = event.data;
                    };
                } 
                else {
                    document.getElementById("result").innerHTML = "Sorry, your browser does not support Web Workers...";
                }
            }

            function stopWorker() { 
                w.terminate();
                w = undefined;
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./More_Examples/Example_2.html)

## HTML server sent events

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Getting server updates</h1>
        <div id="result"></div>

        <script>
            if(typeof(EventSource) !== "undefined") {
                var source = new EventSource("./demo_sse.php");
                source.onmessage = function(event) {
                    document.getElementById("result").innerHTML += event.data + "<br>";
                };
            } 
            else {
                document.getElementById("result").innerHTML = "Sorry, your browser does not support server-sent events...";
            }
        </script>
    </body>
</html>
```

Output:

[Click here!](./More_Examples/Example_3.html)