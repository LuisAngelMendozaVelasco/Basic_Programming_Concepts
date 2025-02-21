# Conditions

## The if Statement

Code:

```go
package main
import "fmt"

func main() {
  x:= 20
  y:= 18

  if x > y {
    fmt.Println("x is greater than y")
  }
}
```

Output:

```text
x is greater than y 
```

## The else Statement

Code:

```go
package main
import "fmt"

func main() {
  time := 20

  if (time < 18) {
    fmt.Println("Good day.")
  } else {
    fmt.Println("Good evening.")
  }
}
```

Output:

```text
Good evening. 
```

## The else if Statement

Code:

```go
package main
import "fmt"

func main() {
  time := 22

  if time < 10 {
    fmt.Println("Good morning.")
  } else if time < 20 {
    fmt.Println("Good day.")
  } else {
    fmt.Println("Good evening.")
  }
}
```

Output:

```text
Good evening. 
```

## The Nested if Statement

Code:

```go
package main
import "fmt"

func main() {
  num := 20

  if num >= 10 {
    fmt.Println("Num is more than 10.")
    
    if num > 15 {
      fmt.Println("Num is also more than 15.")
    }
  } else {
    fmt.Println("Num is less than 10.")
  }
}
```

Output:

```text
Num is more than 10.
Num is also more than 15.
```
