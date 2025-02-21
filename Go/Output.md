# Output

## The Print() Function

Code:

```go
package main
import "fmt"

func main() {
  var i,j string = "Hello","World"

  fmt.Print(i)
  fmt.Print(j)
}
```

Output:

```text
HelloWorld
```

## The Println() Function

Code:

```go
package main
import "fmt"

func main() {
  var i,j string = "Hello","World"

  fmt.Println(i,j)
}
```

Output:

```text
HelloWorld
```

## The Printf() Function

Code:

```go
package main
import "fmt"

func main() {
  var i string = "Hello"
  var j int = 15

  fmt.Printf("i has value: %v and type: %T\n", i, i)
  fmt.Printf("j has value: %v and type: %T", j, j)
}
```

Output:

```text
i has value: Hello and type: string
j has value: 15 and type: int
```

## General Formatting Verbs

Code:

```go
package main
import "fmt"

func main() {
  var i = 15.5
  var txt = "Hello World!"

  fmt.Printf("%v\n", i)
  fmt.Printf("%#v\n", i)
  fmt.Printf("%v%%\n", i)
  fmt.Printf("%T\n", i)

  fmt.Printf("%v\n", txt)
  fmt.Printf("%#v\n", txt)
  fmt.Printf("%T\n", txt)
}
```

Output:

```text
15.5
15.5
15.5%
float64
Hello World!
"Hello World!"
string
```

## Integer Formatting Verbs

Code:

```go
package main
import "fmt"

func main() {
  var i = 15
 
  fmt.Printf("%b\n", i)
  fmt.Printf("%d\n", i)
  fmt.Printf("%+d\n", i)
  fmt.Printf("%o\n", i)
  fmt.Printf("%O\n", i)
  fmt.Printf("%x\n", i)
  fmt.Printf("%X\n", i)
  fmt.Printf("%#x\n", i)
  fmt.Printf("%4d\n", i)
  fmt.Printf("%-4d\n", i)
  fmt.Printf("%04d\n", i)
}
```

Output:

```text
1111
15
+15
17
0o17
f
F
0xf
  15
15  
0015
```

## String Formatting Verbs

Code:

```go
package main
import "fmt"

func main() {
  var txt = "Hello"
 
  fmt.Printf("%s\n", txt)
  fmt.Printf("%q\n", txt)
  fmt.Printf("%8s\n", txt)
  fmt.Printf("%-8s\n", txt)
  fmt.Printf("%x\n", txt)
  fmt.Printf("% x\n", txt)
}
```

Output:

```text
Hello
"Hello"
  Hello
Hello   
48656c6c6f
48 65 6c 6c 6f
```

## Boolean Formatting Verbs

Code:

```go
package main
import "fmt"

func main() {
  var i = true
  var j = false

  fmt.Printf("%t\n", i)
  fmt.Printf("%t\n", j)
}
```

Output:

```text
true
false
```

## Float Formatting Verbs

Code:

```go
package main
import "fmt"

func main() {
  var i = 3.141

  fmt.Printf("%e\n", i)
  fmt.Printf("%f\n", i)
  fmt.Printf("%.2f\n", i)
  fmt.Printf("%6.2f\n", i)
  fmt.Printf("%g\n", i)
}
```

Output:

```text
3.141000e+00
3.141000
3.14
  3.14
3.141
```
