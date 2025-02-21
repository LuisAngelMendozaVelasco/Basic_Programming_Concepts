# Data Types

## Float Formatting Verbs

Code:

```go
package main
import "fmt"

func main() {
  var a bool = true     // Boolean
  var b int = 5         // Integer
  var c float32 = 3.14  // Floating point number
  var d string = "Hi!"  // String

  fmt.Println("Boolean: ", a)
  fmt.Println("Integer: ", b)
  fmt.Println("Float:   ", c)
  fmt.Println("String:  ", d)
}
```

Output:

```text
Boolean:  true
Integer:  5
Float:    3.14
String:   Hi!
```

## Boolean Data Type

Code:

```go
package main
import "fmt"

func main() {
  var b1 bool = true // typed declaration with initial value
  var b2 = true // untyped declaration with initial value
  var b3 bool // typed declaration without initial value
  b4 := true // untyped declaration with initial value

  fmt.Println(b1) // Returns true
  fmt.Println(b2) // Returns true
  fmt.Println(b3) // Returns false
  fmt.Println(b4) // Returns true
}
```
Java

Output:

```text
true
true
false
true
```

## Signed and Unsigned Integers

Code:

```go
package main
import "fmt"

func main() {
  var x int = 500
  var y int = -4500
  var a uint = 500
  var b uint = 4500

  fmt.Printf("Type: %T, value: %v", x, x)
  fmt.Printf("Type: %T, value: %v", y, y)
  fmt.Printf("Type: %T, value: %v", a, a)
  fmt.Printf("Type: %T, value: %v", b, b)
}
```

Output:

```text
Type: int, value: 500Type: int, value: -4500Type: uint, value: 500Type: uint, value: 4500
```

## Float Data Types

Code:

```go
package main
import "fmt"

func main() {
  var x float32 = 123.78
  var y float32 = 3.4e+38
  var a float64 = 1.7e+308

  fmt.Printf("Type: %T, value: %v\n", x, x)
  fmt.Printf("Type: %T, value: %v\n", y, y)
  fmt.Printf("Type: %T, value: %v", a, a)
}
```

Output:

```text
Type: float32, value: 123.78
Type: float32, value: 3.4e+38
Type: float64, value: 1.7e+308
```

## String Data Type

Code:

```go
package main
import "fmt"

func main() {
  var txt1 string = "Hello!"
  var txt2 string
  txt3 := "World 1"

  fmt.Printf("Type: %T, value: %v\n", txt1, txt1)
  fmt.Printf("Type: %T, value: %v\n", txt2, txt2)
  fmt.Printf("Type: %T, value: %v\n", txt3, txt3)
}
```

Output:

```text
Type: string, value: Hello!
Type: string, value: 
Type: string, value: World 1
```
