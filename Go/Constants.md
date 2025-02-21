# Constants

## Declaring a Constant

Code:

```go
package main
import "fmt"

const PI = 3.14

func main() {
  fmt.Println(PI)
}
```

Output:

```text
3.14
```

## Typed and Untyped Constants

Code:

```go
package main
import "fmt"

const A int = 1
const B = 1

func main() {
  fmt.Println(A)
  fmt.Println(B)
} 
```

Output:

```text
1
1
```

## Multiple Constants Declaration

Code:

```go
package main
import "fmt"

const (
  A int = 1
  B = 3.14
  C = "Hi!"
)

func main() {
  fmt.Println(A)
  fmt.Println(B)
  fmt.Println(C)
}
```

Output:

```text
1
3.14
Hi!
```
