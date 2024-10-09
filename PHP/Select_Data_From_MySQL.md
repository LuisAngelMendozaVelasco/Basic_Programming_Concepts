# Select Data From MySQL

## Select data with MySQLi (Object-oriented)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $servername = "localhost";
            $username = "root";
            $password = "";
            $dbname = "myDB";

            // Create connection
            $conn = new mysqli($servername, $username, $password, $dbname);

            // Check connection
            if ($conn->connect_error) {
                die("Connection failed: " . $conn->connect_error);
            }

            $sql = "SELECT id, firstname, lastname 
                    FROM MyGuests";
            $result = $conn->query($sql);

            if ($result->num_rows > 0) {
                // Output data of each row
                while($row = $result->fetch_assoc()) {
                    echo "<br> id: ". $row["id"]. " - Name: ". $row["firstname"]. " " . $row["lastname"] . "<br>";
                }
            } 
            else {
                echo "0 results";
            }

            $conn->close();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphpfile.php?filename=demo_db_select_oo)

## Select data with MySQLi (Procedural)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            $servername = "localhost";
            $username = "root";
            $password = "";
            $dbname = "myDB";

            // Create connection
            $conn = mysqli_connect($servername, $username, $password, $dbname);

            // Check connection
            if (!$conn) {
                die("Connection failed: " . mysqli_connect_error());
            }

            $sql = "SELECT id, firstname, lastname 
                    FROM MyGuests";
            $result = mysqli_query($conn, $sql);

            if (mysqli_num_rows($result) > 0) {
                // output data of each row
                while($row = mysqli_fetch_assoc($result)) {
                    echo "id: " . $row["id"]. " - Name: " . $row["firstname"]. " " . $row["lastname"]. "<br>";
                }
            } 
            else {
                echo "0 results";
            }

            mysqli_close($conn);
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphpfile.php?filename=demo_db_select_proc)

## Put the resut in an HTML table (Object-oriented)

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            table, th, td {
                border: 1px solid black;
            }
        </style>
    </head>
    <body>
        <?php
            $servername = "localhost";
            $username = "root";
            $password = "";
            $dbname = "myDB";

            // Create connection
            $conn = new mysqli($servername, $username, $password, $dbname);

            // Check connection
            if ($conn->connect_error) {
                die("Connection failed: " . $conn->connect_error);
            }

            $sql = "SELECT id, firstname, lastname 
                    FROM MyGuests";
            $result = $conn->query($sql);

            if ($result->num_rows > 0) {
                echo "<table><tr><th>ID</th><th>Name</th></tr>";

                // output data of each row
                while($row = $result->fetch_assoc()) {
                    echo "<tr><td>" . $row["id"]. "</td><td>" . $row["firstname"]. " " . $row["lastname"]. "</td></tr>";
                }
                
                echo "</table>";
            } 
            else {
                echo "0 results";
            }

            $conn->close();
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphpfile.php?filename=demo_db_select_oo_table)

## Select data with PDO (+ Prepared statements)

Code: 

```html
<!DOCTYPE html>
<html>
    <body>
        <?php
            echo "<table style='border: solid 1px black;'>";
            echo "<tr><th>Id</th><th>Firstname</th><th>Lastname</th></tr>";

            class TableRows extends RecursiveIteratorIterator {
                function __construct($it) {
                    parent::__construct($it, self::LEAVES_ONLY);
                }

                function current() {
                    return "<td style='width: 150px; border: 1px solid black;'>" . parent::current(). "</td>";
                }

                function beginChildren() {
                    echo "<tr>";
                }

                function endChildren() {
                    echo "</tr>" . "\n";
                }
            }

            $servername = "localhost";
            $username = "root";
            $password = "";
            $dbname = "myDB";

            try {
                $conn = new PDO("mysql:host=$servername;dbname=$dbname", $username, $password);
                $conn->setAttribute(PDO::ATTR_ERRMODE, PDO::ERRMODE_EXCEPTION);
                $stmt = $conn->prepare("SELECT id, firstname, lastname 
                                        FROM MyGuests");
                $stmt->execute();

                // Set the resulting array to associative
                $result = $stmt->setFetchMode(PDO::FETCH_ASSOC);

                foreach(new TableRows(new RecursiveArrayIterator($stmt->fetchAll())) as $k=>$v) {
                    echo $v;
                }
            }
            catch(PDOException $e) {
                echo "Error: " . $e->getMessage();
            }
            
            $conn = null;
            echo "</table>";
        ?>
    </body>
</html>
```

Output:

[Click here!](https://tryphp.w3schools.com/showphpfile.php?filename=demo_db_select_pdo)