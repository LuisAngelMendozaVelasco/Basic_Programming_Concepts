# Pointers

## Create a pointer variable

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string food = "Pizza";  // A string variable
    string* ptr = &food;  // A pointer variable that stores the address of food

    // Output the value of food
    cout << food << "\n";

    // Output the memory address of food
    cout << &food << "\n";

    // Output the memory address of food with the pointer
    cout << ptr << "\n";

    return 0;
}
```

Output:

```text
Pizza
0x7ffe95781c40
0x7ffe95781c40
```

## Get the value of a variable with the dereference operator *

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string food = "Pizza";  // Variable declaration
    string* ptr = &food;    // Pointer declaration

    // Reference: Output the memory address of food with the pointer
    cout << ptr << "\n";

    // Dereference: Output the value of food with the pointer
    cout << *ptr << "\n";

    return 0;
}
```

Output:

```text
0x7ffe7d982780
Pizza
```

## Modify the pointer value

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string food = "Pizza";
    string* ptr = &food;

    // Output the value of food
    cout << food << "\n";

    // Output the memory address of food
    cout << &food << "\n";

    // Access the memory address of food and output its value
    cout << *ptr << "\n";

    // Change the value of the pointer
    *ptr = "Hamburger";

    // Output the new value of the pointer
    cout << *ptr << "\n";

    // Output the new value of the food variable
    cout << food << "\n";

    return 0;
}
```

Output:

```text
Pizza
0x7ffc31404af0
Pizza
Hamburger
Hamburger
```