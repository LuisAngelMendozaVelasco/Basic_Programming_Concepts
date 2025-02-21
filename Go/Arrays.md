# Arrays

## Declare an Array

Code:

```go
package main
import "fmt"

func main() {
  var arr1 = [3]int{1,2,3}
  arr2 := [5]int{4,5,6,7,8}
  var cars = [4]string{"Volvo", "BMW", "Ford", "Mazda"}

  fmt.Println(arr1)
  fmt.Println(arr2)
  fmt.Print(cars)
}
```

Output:

```text
[1 2 3]
[4 5 6 7 8]
[Volvo BMW Ford Mazda]
```

## Access Elements of an Array

Code:

```go
package main
import "fmt"

func main() {
  prices := [3]int{10,20,30}

  fmt.Println(prices[0])
  fmt.Println(prices[2])
}
```

Output:

```text
10
30 
```

## Change Elements of an Array

Code:

```go
package main
import "fmt"

func main() {
  prices := [3]int{10,20,30}

  prices[2] = 50
  fmt.Println(prices)
}
```

Output:

```text
[10 20 50] 
```

## Array Initialization

Code:

```go
package main
import "fmt"

func main() {
  arr1 := [5]int{} //not initialized
  arr2 := [5]int{1,2} //partially initialized
  arr3 := [5]int{1,2,3,4,5} //fully initialized

  fmt.Println(arr1)
  fmt.Println(arr2)
  fmt.Println(arr3)
}
```

Output:

```text
[0 0 0 0 0]
[1 2 0 0 0]
[1 2 3 4 5] 
```

## Initialize Only Specific Elements

Code:

```go
package main
import "fmt"

func main() {
  arr1 := [5]int{1:10,2:40}

  fmt.Println(arr1)
}
```

Output:

```text
[0 10 40 0 0]
```

## Find the Length of an Array

Code:

```go
package main
import "fmt"

func main() {
  arr1 := [4]string{"Volvo", "BMW", "Ford", "Mazda"}
  arr2 := [...]int{1,2,3,4,5,6}

  fmt.Println(len(arr1))
  fmt.Println(len(arr2))
}
```

Output:

```text
4
6 
```
