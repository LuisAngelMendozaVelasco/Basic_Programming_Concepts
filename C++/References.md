# References

## Create a reference variable

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    /*
    A reference variable is a "reference" to an existing variable, 
    and it is created with the & operator.
    */
    string food = "Pizza";
    string &meal = food;

    /*
    Now, we can use either the variable name food or the reference 
    name meal to refer to the food variable.
    */
    cout << food << "\n";
    cout << meal << "\n";

    return 0;
}
```

Output:

```text
Pizza
Pizza
```

## Access the memory address of a variable

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string food = "Pizza";

    cout << &food << endl;

    return 0;
}
```

Output:

```text
0x7ffcf63f9890
```