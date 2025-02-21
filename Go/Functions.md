# Functions

## Call a Function

Code:

```go
package main
import "fmt"

func myMessage() {
  fmt.Println("I just got executed!")
}

func main() {
  myMessage() // call the function
}
```

Output:

```text
I just got executed!
```

## Function With Parameter

Code:

```go
package main
import "fmt"

func familyName(fname string) {
  fmt.Println("Hello", fname, "Refsnes")
}

func main() {
  familyName("Liam")
  familyName("Jenny")
  familyName("Anja")
}
```

Output:

```text
Hello Liam Refsnes
Hello Jenny Refsnes
Hello Anja Refsnes 
```

## Multiple Parameters

Code:

```go
package main
import "fmt"

func familyName(fname string, age int) {
  fmt.Println("Hello", age, "year old", fname, "Refsnes")
}

func main() {
  familyName("Liam", 3)
  familyName("Jenny", 14)
  familyName("Anja", 30)
}
```

Output:

```text
Hello 3 year old Liam Refsnes
Hello 14 year old Jenny Refsnes
Hello 30 year old Anja Refsnes
```

## Function Return

Code:

```go
package main
import "fmt"

func myFunction(x int, y int) int {
  return x + y
}

func main() {
  fmt.Println(myFunction(1, 2))
}
```

Output:

```text
3
```

## Named Return Values

Code:

```go
package main
import "fmt"

func myFunction(x int, y int) (result int) {
  result = x + y

  return
}

func main() {
  fmt.Println(myFunction(1, 2))
}
```

Output:

```text
3
```

## Store the Return Value in a Variable

Code:

```go
package main
import "fmt"

func myFunction(x int, y int) (result int) {
  result = x + y

  return
}

func main() {
  total := myFunction(1, 2)
  fmt.Println(total)
}
```

Output:

```text
3
```

## Multiple Return Values

Code:

```go
package main
import "fmt"

func myFunction(x int, y string) (result int, txt1 string) {
  result = x + x
  txt1 = y + " World!"

  return
}

func main() {
  fmt.Println(myFunction(5, "Hello"))
}
```

Output:

```text
10 Hello World!
```

## Recursion Functions

Code:

```go
package main
import "fmt"

func testcount(x int) int {
  if x == 11 {
    return 0
  }
  
  fmt.Println(x)

  return testcount(x + 1)
}

func main(){
  testcount(1)
} 
```

Output:

```text
1
2
3
4
5
6
7
8
9
10
```
