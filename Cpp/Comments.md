# Comments

## Single-line comment before a line of code

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    // This is a comment
    cout << "Hello World!" << endl;

    return 0;
}
```

Output:

```text
Hello World!
```

## Single-line comment at the end of a line of code

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello World!" << endl; // This is a comment

    return 0;
}
```

Output:

```text
Hello World!
```

## Multi-line comment

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    /* 
    The code below will print the words Hello World!
    to the screen.
    */  
    cout << "Hello World!" << endl;

    return 0;
}
```

Output:

```text
Hello World!
```