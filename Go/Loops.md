# Loops

## for Loop

Code:

```go
package main
import "fmt"

func main() {
  for i:=0; i < 5; i++ {
    fmt.Println(i)
  }
}
```

Output:

```text
0
1
2
3
4
```

## The continue Statement

Code:

```go
package main
import "fmt"

func main() {
  for i:=0; i < 5; i++ {
    if i == 3 {
      continue
    }

    fmt.Println(i)
  }
}
```

Output:

```text
0
1
2
3
4
```

## The break Statement

Code:

```go
package main
import "fmt"

func main() {
  for i:=0; i < 5; i++ {
    if i == 3 {
      break
    }

    fmt.Println(i)
  }
}
```

Output:

```text
0
1
2
```

## Nested Loops

Code:

```go
package main
import "fmt"

func main() {
  adj := [2]string{"big", "tasty"}
  fruits := [3]string{"apple", "orange", "banana"}

  for i:=0; i < len(adj); i++ {
    for j:=0; j < len(fruits); j++ {
      fmt.Println(adj[i],fruits[j])
    }
  }
}
```

Output:

```text
big apple
big orange
big banana
tasty apple
tasty orange
tasty banana
```

## Nested Loops

Code:

```go
package main
import "fmt"

func main() {
  adj := [2]string{"big", "tasty"}
  fruits := [3]string{"apple", "orange", "banana"}

  for i:=0; i < len(adj); i++ {
    for j:=0; j < len(fruits); j++ {
      fmt.Println(adj[i],fruits[j])
    }
  }
}
```

Output:

```text
big apple
big orange
big banana
tasty apple
tasty orange
tasty banana
```

## The Range Keyword

Code:

```go
package main
import "fmt"

func main() {
  fruits := [3]string{"apple", "orange", "banana"}

  for idx, val := range fruits {
    fmt.Printf("%v\t%v\n", idx, val)
  }
}
```

Output:

```text
0      apple
1      orange
2      banana 
```
