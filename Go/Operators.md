# Operators

## Arithmetic

Code:

```go
package main
import "fmt"

func main() {
  var (
    sum1 = 100 + 50 // 150 (100 + 50)
    sum2 = sum1 + 250 // 400 (150 + 250)
    sum3 = sum2 + sum2 // 800 (400 + 400)
  )

  fmt.Println(sum3)
}
```

Output:

```text
800
```

## Assignment

Code:

```go
package main
import "fmt"

func main() {
  var x = 10

  fmt.Println(x)
}
```

Output:

```text
10
```

## Comparison

Code:

```go
package main
import "fmt"

func main() {
  var x = 5
  var y = 3

  fmt.Println(x>y) // returns 1 (true) because 5 is greater than 3
}
```

Output:

```text
true
```
