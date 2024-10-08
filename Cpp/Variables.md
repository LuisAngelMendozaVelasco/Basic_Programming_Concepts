# Variables

## Create an integer variable

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int myNum = 15;

    cout << myNum << endl;

    return 0;
}
```

Output:

```text
15
```

## Create a variable without assigning the value, and assign the value later

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int myNum;

    myNum = 15;
    cout << myNum << endl;

    return 0;
}
```

Output:

```text
15
```

## Assign a new value to an existing value (this will overwrite the previous value)

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int myNum = 15;   // Now myNum is 15

    myNum = 10;       // Now myNum is 10
    cout << myNum << endl;

    return 0;
}
```

Output:

```text
10
```

## Create an unchangeable variable with the const keyword

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    const int myNum = 15;
    cout << myNum << endl;

    return 0;
}
```

Output:

```text

```

## Combine text and a variable on print

Code:

```cpp
15
```

Output:

```text

```

## Add a variable to another variable

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int myAge = 29;

    cout << "I am " << myAge << " years old." << endl;

    return 0;
}
```

Output:

```text
I am 29 years old.
```

## Declare many variables of the same type with a comma-separated list

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int x = 5;
    int y = 6;
    int sum = x + y;

    cout << sum << endl;

    return 0;
}
```

Output:

```text
11
```

## Identifiers

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int x = 5, y = 6, z = 50;

    cout << x + y + z << endl;

    return 0;
}
```

Output:

```text
61
```