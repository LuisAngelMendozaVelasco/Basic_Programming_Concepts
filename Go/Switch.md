# Switch

## The switch Statement

Code:

```go
package main
import "fmt"

func main() {
  day := 4

  switch day {
  case 1:
    fmt.Println("Monday")
  case 2:
    fmt.Println("Tuesday")
  case 3:
    fmt.Println("Wednesday")
  case 4:
    fmt.Println("Thursday")
  case 5:
    fmt.Println("Friday")
  case 6:
    fmt.Println("Saturday")
  case 7:
    fmt.Println("Sunday")
  }
}
```

Output:

```text
Thursday
```

## The default Keyword

Code:

```go
package main
import "fmt"

func main() {
  day := 8

  switch day {
  case 1:
    fmt.Println("Monday")
  case 2:
    fmt.Println("Tuesday")
  case 3:
    fmt.Println("Wednesday")
  case 4:
    fmt.Println("Thursday")
  case 5:
    fmt.Println("Friday")
  case 6:
    fmt.Println("Saturday")
  case 7:
    fmt.Println("Sunday")
  default:
    fmt.Println("Not a weekday")
  }
}
```

Output:

```text
Not a weekday
```

## The Multi-case switch Statement

Code:

```go
package main
import "fmt"

func main() {
  day := 5

  switch day {
  case 1,3,5:
    fmt.Println("Odd weekday")
  case 2,4:
    fmt.Println("Even weekday")
  case 6,7:
    fmt.Println("Weekend")
  default:
    fmt.Println("Invalid day of day number")
  }
}
```

Output:

```text
Odd weekday
```
