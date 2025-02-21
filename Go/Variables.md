# Variables

## Variable Declaration With Initial Value

Code:

```go
package main
import "fmt"

func main() {
  var student1 string = "John" //type is string
  var student2 = "Jane" //type is inferred
  x := 2 //type is inferred

  fmt.Println(student1)
  fmt.Println(student2)
  fmt.Println(x)
}
```

Output:

```text
John
Jane
2
```

## Variable Declaration Without Initial Value

Code:

```go
package main
import "fmt"

func main() {
  var a string
  var b int
  var c bool

  fmt.Println(a)
  fmt.Println(b)
  fmt.Println(c)
}
```

Output:

```text

0
false
```

## Value Assignment After Declaration

Code:

```go
package main
import "fmt"

func main() {
  var student1 string
  student1 = "John"
  
  fmt.Println(student1)
}
```

Output:

```text
John
```

## Multiple Variable Declaration

Code:

```go
package main
import "fmt"

func main() {
  var a, b, c, d int = 1, 3, 5, 7

  fmt.Println(a)
  fmt.Println(b)
  fmt.Println(c)
  fmt.Println(d)
}
```

Output:

```text
1
3
5
7
```

## Variable Declaration in a Block

Code:

```go
package main
import "fmt"

func main() {
  var (
    a int
    b int = 1
    c string = "hello"
  )

  fmt.Println(a)
  fmt.Println(b)
  fmt.Println(c)
}
```

Output:

```text
0
1
hello
```
